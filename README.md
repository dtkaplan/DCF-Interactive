# Interactive components of the DCF software

This package provides software with an interactive component for the DCF course, using `manipulate` and `shiny`.  

It's separate from DCF so that students don't accidentally use the interactive functions inside an Rmd document.

## Command Helper

A package providing the function `lintr()`, which allows you to edit interactively potentially complex chains of `dplyr` commands.

For instance

    require( mosaicData )
    lintr(
    KidsFeet %>%
      group_by( sex ) 
    )

On return, `lintr()` opens an editor with the completed command.  You can run this, or cut and paste it into a script or Rmd file.
