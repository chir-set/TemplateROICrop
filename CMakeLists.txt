cmake_minimum_required(VERSION 3.5)

project(TemplateROICrop)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/TemplateROICrop")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "SET (No Corp.)")
set(EXTENSION_DESCRIPTION "Crop a volume from a template ROI")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/TemplateROICrop.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/TemplateROICrop/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(TemplateROICrop)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
