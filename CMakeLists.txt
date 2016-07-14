#
# CMakeLists.txt
# date: July 10, 2016
#

# Specify the minimum CMake version required.  If the cmake version 
# minimum is not met, cmake will fail.
cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

# Set the name of the project
project(ldmx-cdr NONE)

# Include the file containing the CMake LaTeX macros required to build the
# document.
include(cmake/UseLATEX.cmake)

# Add the document to the build
add_latex_document(ldmx_cdr.tex
    INPUTS sections/overview.tex
           sections/goals.tex
           sections/detector.tex
           sections/detector/overview.tex
           sections/detector/beamline.tex
           sections/detector/tagger_tracker.tex
           sections/detector/target.tex
           sections/detector/recoil_tracker.tex
           sections/detector/ecal.tex
           sections/detector/hcal.tex
           sections/detector/wide_cal.tex
           sections/detector/trigger.tex
           sections/detector/daq.tex
           sections/simulation.tex
           sections/performance.tex
           sections/performance/signal.tex
           sections/performance/tracking.tex
           sections/performance/ecal.tex
           sections/performance/hcal.tex
           sections/performance/trigger.tex
           sections/budget.tex
    IMAGE_DIRS images
)
