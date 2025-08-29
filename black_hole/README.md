Sure! I’ve added proper Markdown headings using `##` and cleaned it up so it’s ready for `README.md`. You can copy-paste this directly:

---

# Black Hole Simulation Project

I worked on a black hole simulation project and wanted to share the journey. I managed to get most of it running in about a week. It was a mix of learning, experimenting, and problem-solving, and it gave me a much better understanding of how physics simulations work behind the scenes. All the code is in the `src` folder, so you can explore or reuse it easily.

## What I Set Out to Do

When I started, I had a few goals in mind:

**Ray Tracing** – I wanted to simulate how light bends around a black hole. This part was tricky because getting the visuals to look realistic required a lot of trial and error.

**Accretion Disk** – I wanted to show the glowing disk around the black hole. Combining it with ray tracing and halo effects took a lot of tweaking to get right.

**Spacetime Curvature** – I tried to visually show how a black hole warps spacetime using a grid. It’s fascinating to see the “trapdoor” effect in action.

**Real-Time Simulation** – I experimented with making the simulation run faster. It pushed my GPU and helped me learn a lot about optimization.

## Challenges and Learning

The biggest challenges were figuring out the GPU computations for the 3D simulation and debugging the ray tracing. Some days the halos or light bending didn’t look right, and I had to go back and adjust the models.

This project taught me how to turn physics concepts into code, how to optimize calculations for speed, and how to match visuals to the underlying simulation. Doing this in one week showed me how much planning and testing goes into even a small simulation project.

## What I Built

* A 2D simulation of gravitational lensing.
* A 3D simulation using GPU computations for faster calculations.
* A visualization of spacetime curvature and the accretion disk.

The focus wasn’t just on the visuals but also on the physics model and how the simulation calculates everything step by step.

## Takeaways

* Learned ray tracing, GPU-based computation, and physics simulation in practice.
* Gained hands-on experience with C++17, CMake, and Vcpkg.
* Learned to translate real-world physics into working, efficient code.

This project was short but intense and rewarding. By the end, I felt confident tackling more physics-based simulations and understood the challenges of optimizing and debugging complex systems.

## How to Run

**Clone the repository:**

```bash
git clone https://github.com/haripriyatripathi/Black-Hole-Simulation-using-cpp-.git
```

**Go into the project folder:**

```bash
cd Black-Hole-Simulation-using-cpp-
```

**Install dependencies using Vcpkg:**

```bash
vcpkg install
```

**Integrate Vcpkg with CMake:**

```bash
vcpkg integrate install
```

This will give you a path to the CMake toolchain, like:

```
-DCMAKE_TOOLCHAIN_FILE=/path/to/vcpkg/scripts/buildsystems/vcpkg.cmake
```

**Create a build folder:**

```bash
mkdir build
```

**Configure the project with CMake:**

```bash
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE=/path/to/vcpkg/scripts/buildsystems/vcpkg.cmake
```

**Build the project:**

```bash
cmake --build build
```

**Run the simulation:**
The executables will be inside the `build` folder.

## How the Code Works

For 2D simulations, run `2D_lensing.cpp`.
For 3D simulations, `black_hole.cpp` and `geodesic.comp` work together. The CPU sends data to the GPU, which handles the heavy calculations to make the simulation faster.

I mainly tested this on Windows with a GPU, so results may vary on other systems. If anyone is curious, I can explain more about the models, optimizations, and how the GPU calculations work in detail, dm me: haripriyatripathix@gmail.com :)


