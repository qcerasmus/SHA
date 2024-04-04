# SHA
C++ implementation of the SHA512, SHA384 and SHA256 hashing algorithms. Requires the messages to be of size `< size_t` bytes.

## Usage example
```c++
#include "sha/SHA512.h" //include SHA512 definition

SHA512 sha512; //instantiate a SHA512 object
sha512.hash("Example"); //returns the hash as a string
```

## Manual compile and run
1. Clone the repository.
2. Run the build.sh script.
3. The compiled output will be in xbuild/Debug/

## Using CMake
1. Add this to your CMakeLists.txt file:
```cmake
include(FetchContent)

FetchContent_Declare(
		sha
		GIT_REPOSITORY https://github.com/qcerasmus/SHA.git
		GIT_TAG master
)
FetchContent_MakeAvailable(sha)
```
2. Check the usage :)

