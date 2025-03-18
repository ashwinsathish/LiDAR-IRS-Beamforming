# LiDAR-Enabled Spatial Awareness for IRS-Assisted Wireless Communication

This repository contains an implementation of the paper - 'LiDAR-Enabled Spatial Awareness for Beamforming in IRS-Assisted Wireless Communication System'. 

## Project Overview

Modern wireless networks face significant challenges in maintaining reliable connectivity in dynamic urban environments, particularly in vehicular networks with high mobility. We introduce a novel approach that combines LiDAR technology with IRS-assisted communication systems to provide robust and efficient wireless connectivity. This focuses on enhancing vehicular communications through real-time environmental awareness and optimized beamforming strategies.

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

## Citation

A. S. Kumar and S. Joshi, "LiDAR-Enabled Spatial Awareness for Beamforming in IRS-Assisted Wireless Communication System," *2024 IEEE International Conference on Advanced Networks and Telecommunications Systems (ANTS)*, Guwahati, India, 2024, pp. 1-6, doi: [10.1109/ANTS63515.2024.10898544](https://doi.org/10.1109/ANTS63515.2024.10898544).
