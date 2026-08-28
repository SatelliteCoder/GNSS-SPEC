# GNSS-SPEC: GNSS Signal Processing & Education Center

**GNSS-SPEC** is an open-source education platform focused on GNSS signal processing and algorithm implementation. This project provides complete signal processing chain from simulation to positioning solution.

## ✨ Features
- 📡 **Multi-constellation Support**: GPS L1 C/A and BDS B1I signals
- ⚙️ **Complete Processing Chain**: Signal generation, error modeling, acquisition, tracking, and positioning
- 📊 **Error Channel Simulation**: Ionospheric delay, tropospheric delay, and multipath effects
- 🎨 **Visualization Tools**: Signal spectrum, correlation peaks, skyplot, and positioning results
- 📖 **Detailed Documentation**: Learning notes and theoretical explanations

## 🗂️ Project Structure
```text
GNSS-SPEC/
├── src/                    # Source code
│   ├── simulation/        # Signal generation and error modeling
│   ├── processing/        # Acquisition and tracking algorithms
│   └── positioning/       # LSQ and EKF solutions
├── notebooks/             # Jupyter notebooks for learning
├── docs/                  # Detailed documentation
├── data/                  # Sample data files
└── tools/                 # Visualization and analysis tools
```

## 🚀 Getting Started

### Prerequisites
- C++17 compatible compiler
- CMake (≥3.10)
- Python 3.8+ with numpy and matplotlib

### Installation
```bash
# Clone the repository
git clone https://github.com/your-username/GNSS-SPEC.git
cd GNSS-SPEC

# Build with CMake
mkdir build && cd build
cmake .. && make

# Run simulation
./bin/gnss_simulator
```

## 📖 Documentation
Explore our detailed learning notes:
- Signal Generation Principles
- Error Modeling Methods
- Acquisition & Tracking Algorithms
- Positioning Solutions

## 📎 ICD Reference Documents
Large-size ICD specification files are hosted via Baidu Netdisk:
- **Download link:** [https://pan.baidu.com/s/165mR0DUQotHC6FXu7rDKJw?pwd=ncmd](https://pan.baidu.com/s/165mR0DUQotHC6FXu7rDKJw?pwd=ncmd)
- **Extract code:** `ncmd`

## 👥 Contributing
We welcome contributions! Please feel free to submit:
- Bug reports and feature requests
- Documentation improvements
- New algorithm implementations
- Learning notes and examples

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
- RTKLIB for inspiration
- GPSTk for reference implementations

⭐ If you find this project helpful, please give it a star!
