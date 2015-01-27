# Interactive components of the DCF software

This package provides software with an interactive component for the DCF course, using `manipulate` and `shiny`.  

It's separate from DCF so that students don't accidentally use the interactive functions inside an Rmd document.

## mWrangle Command Helper

A package providing the function `mWrangle()`, which allows you to edit interactively potentially complex chains of `dplyr` commands.

For instance

    require( mosaicData )
    mWrangle(
      KidsFeet %>%
        group_by(sex) 
    )

On return, `mWrangle()` opens an editor with the completed command.  You can run this, or cut and paste it into a script or Rmd file.
