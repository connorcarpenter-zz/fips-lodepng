fips_begin_module(lodepng)
fips_vs_warning_level(3)
fips_files(
        lodepng/lodepng.h lodepng/lodepng.cpp
        lodepng/lodepng_util.h lodepng/lodepng_util.cpp
        lodepng/pngdetail.cpp
)
fips_end_module()