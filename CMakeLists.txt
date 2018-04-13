#
# project: fips-lodepng
#
cmake_minimum_required(VERSION 2.8)
get_filename_component(FIPS_ROOT_DIR "../fips" ABSOLUTE)
include("${FIPS_ROOT_DIR}/cmake/fips.cmake")

include_directories(src)
fips_setup()
fips_project(fips-lodepng)

fips_begin_module(lodepng)
fips_vs_warning_level(3)
fips_dir(lodepng)
fips_files(
        lodepng.h lodepng.cpp
        lodepng_util.h lodepng_util.cpp
        pngdetail.cpp
)
fips_end_module()

fips_finish()