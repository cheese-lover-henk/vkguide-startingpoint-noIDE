# VKguide Starting Point (No IDE)

> ⚠️ **Tested only on Windows**  
> A Linux version might come later – no promises.

## 📦 Prerequisites

Before building the project, make sure you have the following installed and configured:

1. **Vulkan SDK** – Download and install it from https://vulkan.lunarg.com/sdk/home
2. **vcpkg** – Install from https://github.com/microsoft/vcpkg. Take note of its install path.
3. **SDL2 (with Vulkan support)** – Use vcpkg to install:  
	./vcpkg install sdl2[vulkan]
4. **CMake** – Available at https://cmake.org/download/
5. **Environment Variables** – Ensure all the above tools are added to your system PATH

> 🗂 All other required libraries should be included in this repository.  
> If something is missing, feel free to reach out via Discord: `.henk.`

---

## 🛠️ Building the Project

Open a terminal (CMD) in the project’s root folder and run the following:

cmake -S . -B build -DCMAKE_TOOLCHAIN_FILE=C:/path/to/vcpkg/scripts/buildsystems/vcpkg.cmake  
cmake --build build

> Replace `C:/path/to/vcpkg` with the actual path to your vcpkg installation.

The resulting .exe will be located in build/Debug/

---

## 📝 Notes

I'm currently following https://vkguide.dev/  
If I realize anything critical is missing from this starter, I’ll update the repo accordingly.

If you run into any issues or notice missing dependencies, please reach out to me on Discord: `.henk.`

---
