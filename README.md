# LiDAR-Enabled Spatial Awareness for IRS-Assisted Wireless Communication

This repository contains the implementation of a LiDAR-enabled spatial awareness system for beamforming in Intelligent Reflecting Surface (IRS) assisted wireless communication networks. Focuses on enhancing vehicular communications through real-time environmental awareness and optimized beamforming strategies.

## Project Overview

Modern wireless networks face significant challenges in maintaining reliable connectivity in dynamic urban environments, particularly in vehicular networks with high mobility. We introduce a novel approach that combines LiDAR technology with IRS-assisted communication systems to provide robust and efficient wireless connectivity.

### Key Features

- Integration of real-time LiDAR data for dynamic beamforming
- Advanced phase shift optimization algorithm with reduced computational complexity
- IRS element grouping strategies for enhanced performance
- Comprehensive analysis of achievable rates in various scenarios

## System Architecture

The system consists of the following components:

- **Base Station**: 4×2 antenna array configuration
- **IRS**: 256-element array with configurable grouping strategies
- **LiDAR**: Co-located with IRS, providing real-time environmental sensing
- **Vehicle (UE)**: Mobile user equipment with dynamic positioning

### Technical Specifications

- **LiDAR Parameters**:
  - Scanning range: 16 meters
  - Frequency: 10Hz
  - Resolution: 111ms between scans

## Implementation Details

### LiDAR Data Processing Pipeline

1. Raw data collection and temporal aggregation
2. Blockage pattern analysis
3. Vehicle position extraction
4. Coordinate transformation for beamforming

### Phase Shift Optimization

We implement an efficient algorithm for optimizing IRS phase shifts based on vectorized computations are follows:

1. Initialize phase shifts
2. Calculate achievable rate
3. Iteratively optimize individual elements
4. Update phase configuration until convergence

## Results

Our implementation demonstrates:

- 10.5% average improvement in achievable rates across all UE positions
- Enhanced performance of 16×16 IRS arrays with 2×2 grouping compared to 8×8 full CSI configurations

## References

1. A. Alkhateeb et al., "[DeepSense 6G: A Large-Scale Real-World Multi-Modal Sensing and Communication Dataset](https://doi.org/10.1109/MCOM.006.2200730)," *IEEE Communications Magazine*, vol. 61, no. 9, pp. 122-128, Sept. 2023.

2. D. Dampahalage, S. K. Badalge, N. Rajatheva and M. Latva-aho, "[Intelligent Reflecting Surface Aided Vehicular Communications](https://doi.org/10.1109/GCWkshps50303.2020.9367569)," *2020 IEEE Globecom Workshops*, pp. 1-6, 2020.
