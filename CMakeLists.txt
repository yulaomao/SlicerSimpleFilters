cmake_minimum_required(VERSION 3.13.0)

project(SimpleFilters)

#-----------------------------------------------------------------------------
set(EXTENSION_HOMEPAGE "http://www.cjyx.org/cjyxWiki/index.php/Documentation/Nightly/Extensions/SimpleFilters")
set(EXTENSION_CATEGORY "Filtering")
set(EXTENSION_CONTRIBUTORS "Bradley Lowekamp (MSC/NLM), Steve Pieper (Isomics), Jean-Christophe Fillion-Robin (Kitware)" )
set(EXTENSION_DESCRIPTION "This is a meta module which contains interfaces for many Simple ITK image filters.")
set(EXTENSION_ICONURL "http://viewvc.cjyx.org/viewvc.cgi/Cjyx4/trunk/Extensions/Testing/SimpleFilters/SimpleFilters.png?revision=21747&view=co")
set(EXTENSION_SCREENSHOTURLS "http://wiki.cjyx.org/cjyxWiki/images/e/e2/Cjyx-r19441-SimpleFilters-screenshot.png")

#-----------------------------------------------------------------------------
find_package(Cjyx REQUIRED)
include(${Cjyx_USE_FILE})

#-----------------------------------------------------------------------------
add_subdirectory(SimpleFilters)

#-----------------------------------------------------------------------------
include(${Cjyx_EXTENSION_CPACK})
