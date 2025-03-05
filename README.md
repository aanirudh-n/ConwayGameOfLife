# ConwayGameOfLife

Conway's Game of Life (CUDA Implementation)

A parallelized implementation of Conway's Game of Life using CUDA.

🖥️ Overview
This project implements Conway's Game of Life using CUDA to leverage parallel computing on GPUs. It demonstrates how cellular automata can be efficiently simulated using CUDA's parallel processing capabilities.

🚀 Features
Parallel execution of Game of Life rules using CUDA kernels.
Supports a 2D grid with periodic boundary conditions.
Uses randomly initialized cells as the starting state.
Displays iteration-based evolution of cells.
Optimized memory management using CUDA.
🛠️ Installation & Compilation
Prerequisites
CUDA Toolkit (Ensure nvcc is installed)
NVIDIA GPU with CUDA support
Linux/macOS/Windows (WSL2) with GPU drivers installed
Compilation
sh
Copy
Edit
nvcc -o game_of_life game_of_life.cu
Running the Simulation
sh
Copy
Edit
./game_of_life
📝 Rules of Conway's Game of Life
Each cell in the grid follows these simple rules:

🟩 Survival: A live cell with 2 or 3 live neighbors stays alive.
☠️ Underpopulation: A live cell with fewer than 2 live neighbors dies.
🚀 Overpopulation: A live cell with more than 3 live neighbors dies.
🌱 Reproduction: A dead cell with exactly 3 live neighbors becomes alive.
📜 Code Structure
bash
Copy
Edit
📂 Conway-Game-Of-Life-CUDA
│── game_of_life.cu  # Main CUDA implementation
│── README.md        # Project documentation
🖼️ Sample Output
Example of the evolving grid:

Copy
Edit
█   █ █    
█ █     █ 
  █ █ █   
█     █ █ 
███  █  █ 
  █   █ █ 
The grid updates every iteration, displaying dynamic changes.

🏗️ Future Enhancements
📏 Customizable grid sizes
🎨 Visualization using OpenGL
🏎️ Performance benchmarking with different block sizes
🤝 Contributing
Pull requests and contributions are welcome! Feel free to fork and improve the project.

📜 License
This project is licensed under the MIT License.
