# I2C library

Interface for implementing code for I<sup>2</sup>C controllers

## The What

This is a header only library interface that includes common non-platform specific functionality meant for I<sup>2</sup>C controllers.

## The Why

The goal is to make cross platform implementation easier for I<sup>2</sup>C functionality.

## The How

Because the library is header only, it only needs to be included.

```c++
#include "I2C.h"

class PlatformSpecificI2C : public I2C {
    ...
}
```

### Using cmake

```cmake
add_subdirectory(${i2cDir})
target_link_libraries(${PROJECT_NAME} I2C)
```

## The Who

Einar Arnason  
<https://github.com/EinarArnason>  
<https://www.linkedin.com/in/einararnason/>
