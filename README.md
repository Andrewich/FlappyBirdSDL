Flappy Bird SDL
===============

Build
-----

```
conan install . --output-folder=build --build=missing --conf=tools.env.virtualenv:powershell=True
cd build
# conanbuild.ps
cmake .. -G "Visual Studio 16 2019" -DCMAKE_TOOLCHAIN_FILE="conan_toolchain.cmake"
cmake --build . --config Release
```

Links
-----

- https://docs.conan.io/2.0/tutorial/consuming_packages/different_configurations.html
- https://docs.conan.io/2.0/tutorial/consuming_packages/use_tools_as_conan_packages.html
- https://blog.conan.io/2023/07/20/introduction-to-game-dev-with-sdl2.html