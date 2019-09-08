A collection of large C++ projects for running clang-tidy with different purposes.

All projects from this collection have no external dependencies (or minimal additional dependencies) and all can be compiled with Clang.

Current projects:
* LLVM
* CMake
* VTK
* PX4/Firmware
* Bullet Physics SDK
* Cppcheck

How to use it for testing C++ proposals for backward compatibility:
* Write your own Clang-Tidy check
* Use prepared projects from this repo for running your clang-tidy check over projects
* Collect some statistics

How script should work:
* Download specified versions of specified in file projects. File possibly will be in JSON format
* For every project prepare compilation database
* Run 'run_clang_tidy' on every compilation database

