# Awesome-Automotive-Radar-SLAM [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated collection of high-quality resources, papers, and tools dedicated to Automotive Radar SLAM (Simultaneous Localization and Mapping) and odometry. This repository is designed to assist researchers and engineers in discovering leading materials for radar-based localization, mapping, and sensor fusion in autonomous vehicles. While many SLAM methods exist for Navtech radar, this list specifically highlights <font color=red>**on-chip automotive radar**</font> SLAM and odometry—a fast-growing area with significant recent advancements.

---

## Table of Contents

- [Overview](#overview)
- [Radar Only](#radar-only)
- [Radar Inertial Fusion](#radar-inertial-fusion)
- [Radar and Other Sensors Fusion](#radar-and-other-sensors-fusion)
- [Radar Tensors](#radar-tensors)
- [Related Surveys](#papers--surveys)
- [Contributing](#contributing)
- [License](#license)



## Overview

Automotive radar is robust to adverse weather and lighting, making it a key sensor for autonomous vehicles. Radar SLAM and odometry enable accurate localization and mapping using radar data, often in combination with other sensors. This list covers:

- Pure radar-based SLAM and odometry
- Radar-inertial fusion
- Multi-sensor fusion (radar, lidar, camera, GNSS, etc.)
- Radar data representations and learning (tensors, deep learning)

Feel free to suggest additions !!!

## Radar Only

**Papers focused on radar-only SLAM and odometry.**
* <font color=DarkBlue><big>2025</big></font> - Ground-Aware Automotive Radar Odometry __`ICRA`__ [[Paper](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/casado-herraez2025icra.pdf)]

* <font color=DarkBlue><big>2024</big></font> - **Radar4Motion**: IMU-Free 4D Radar Odometry with Robust Dynamic Filtering and RCS-Weighted Matching __`T-IV`__ [[Paper](https://ieeexplore.ieee.org/document/10685149)] 

* <font color=DarkBlue><big>2024</big></font> - Radar-Only Odometry and Mapping for Autonomous Vehicles __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/document/10610311)]

* <font color=DarkBlue><big>2024</big></font> - Doppler-only Single-scan 3D Vehicle Odometry __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/document/10611199)] 

* <font color=DarkBlue><big>2024</big></font> - **EFEAR-4D**: Ego-Velocity Filtering for Efficient and Accurate 4D radar Odometry __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10685149)]

* <font color=DarkBlue><big>2023</big></font> - 4D Radar-Based Pose Graph SLAM With Ego-Velocity Pre-Integration Factor __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10173499)]

* <font color=DarkBlue><big>2022</big></font> - A Credible and Robust Approach to Ego-Motion Estimation Using an Automotive Radar __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/9743799)]

* <font color=DarkBlue><big>2022</big></font> - **DC-Loc**: Accurate Automotive Radar Based Metric Localization with Explicit Doppler Compensation __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/document/9811561)]

* <font color=DarkBlue><big>2019</big></font> - Real-Time Pose Graph SLAM based on Radar __`IV`__ [[Paper](https://ieeexplore.ieee.org/document/8813841)]

* <font color=DarkBlue><big>2017</big></font> - Increasing FastSLAM accuracy for radar data by integrating the Doppler information __`ICMIM`__ [[Paper](https://ieeexplore.ieee.org/document/7918867)]

* <font color=DarkBlue><big>2016</big></font> - Landmark based Radar SLAM Using Graph Optimization __`ITSC`__ [[Paper](https://ieeexplore.ieee.org/document/7795967)]

## Radar Inertial Fusion

**Combining radar with inertial sensors (IMU) for improved localization.**

* <font color=DarkBlue><big>2025</big></font> - **RaI-SLAM**: Radar-Inertial SLAM for Autonomous Vehicles
 __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10947322)]

* <font color=DarkBlue><big>2025</big></font> - Learning Point Correspondences In Radar 3D Point Clouds For Radar-Inertial Odometry __`IROS`__ [[Paper](https://arxiv.org/pdf/2506.18580)]

* <font color=DarkBlue><big>2025</big></font> - **VGC-RIO**: A Tightly Integrated Radar-Inertial Odometry with Spatial Weighted Doppler Velocity and Local Geometric Constrained RCS Histograms __`Arxiv Preprint`__ [[Paper](https://www.arxiv.org/pdf/2505.09103)]

* <font color=DarkBlue><big>2025</big></font> - **Doppler-SLAM**: Doppler-Aided Radar-Inertial and LiDAR-Inertial
Simultaneous Localization and Mapping __`Arxiv Preprint`__ [[Paper](https://arxiv.org/pdf/2504.11634)]

* <font color=DarkBlue><big>2025</big></font> - Impact of Temporal Delay on Radar-Inertial Odometry __`Arxiv Preprint`__ [[Paper](http://arxiv.org/pdf/2503.02509)]

* <font color=DarkBlue><big>2025</big></font> - Ground-Optimized 4D Radar-Inertial Odometry via Continuous Velocity Integration using Gaussian Process __`ICRA`__ [[Paper](https://www.arxiv.org/pdf/2502.08093)]

* <font color=DarkBlue><big>2025</big></font> - EKF-Based Radar-Inertial Odometry with Online Temporal Calibration __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/11018354)]

* <font color=DarkBlue><big>2024</big></font> - 4D Radar-Inertial Odometry based on Gaussian Modeling and Multi-Hypothesis Scan Matching __`Arxiv Preprint`__ [[Paper](http://arxiv.org/pdf/2412.13639)]

* <font color=DarkBlue><big>2024</big></font> - Loosely coupled 4D-Radar-Inertial Odometry for Ground Robots __`Arxiv Preprint`__ [[Paper](https://arxiv.org/pdf/2411.17289)]

* <font color=DarkBlue><big>2024</big></font> - **RIV-SLAM**: Radar-Inertial-Velocity optimization based graph SLAM
 __`CASE`__ [[Paper](https://ieeexplore.ieee.org/document/10711511)]

 * <font color=DarkBlue><big>2024</big></font> - **River**: A Tightly-Coupled Radar-Inertial Velocity Estimator Based on Continuous-Time Optimization __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10529532)]

 * <font color=DarkBlue><big>2024</big></font> - Robust Radar Inertial Odometry in Dynamic 3D Environments __`Drones`__ [[Paper](https://www.mdpi.com/2504-446X/8/5/197)]

 * <font color=DarkBlue><big>2024</big></font> - Radar-Based Localization For Autonomous Ground Vehicles In Suburban Neighborhoods __`T-FR`__ [[Paper](https://ieeexplore.ieee.org/document/10601541)]

 * <font color=DarkBlue><big>2024</big></font> - Towards introspective loop closure in 4D radar SLAM __`Arxiv Preprint`__ [[Paper](https://arxiv.org/pdf/2404.03940)]

 * <font color=DarkBlue><big>2024</big></font> - Incorporating Point Uncertainty in Radar SLAM
 __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10833750)]

 * <font color=DarkBlue><big>2024</big></font> - **Less is More**: Physical-enhanced Radar-Inertial Odometry __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/document/10611471)]

 * <font color=DarkBlue><big>2023</big></font> - **DRIO**: Robust Radar-Inertial Odometry in Dynamic Environments __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10207713)]

 * <font color=DarkBlue><big>2023</big></font> - Multi-State Tightly-Coupled EKF-Based Radar-Inertial Odometry With Persistent Landmarks __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/abstract/document/10160482)]

 * <font color=DarkBlue><big>2023</big></font> - **4D iRIOM**: 4D Imaging Radar Inertial Odometry and Mapping __`RA-L`__ [[Paper](https://ieeexplore.ieee.org/document/10100861)]

 * <font color=DarkBlue><big>2022</big></font> - Tightly-Coupled EKF-Based Radar-Inertial Odometry __`IROS`__ [[Paper](https://ieeexplore.ieee.org/document/9981396)]

 * <font color=DarkBlue><big>2022</big></font> - Radar-Inertial State-Estimation for UAV Motion in Highly Agile Manoeuvres __`ICUAS`__ [[Paper](https://ieeexplore.ieee.org/document/9836130)]

 * <font color=DarkBlue><big>2021</big></font> - Continuous-time Radar-inertial Odometry for Automotive Radars __`IROS`__ [[Paper](https://ieeexplore.ieee.org/document/9636014)]

 * <font color=DarkBlue><big>2021</big></font> - Yaw aided Radar Inertial Odometry using Manhattan World Assumptions __`ICINS`__ [[Paper](https://ieeexplore.ieee.org/document/9470842)]

 * <font color=DarkBlue><big>2021</big></font> - **Milli-RIO**: Ego-Motion Estimation With Low-Cost Millimetre-Wave Radar __`Sensors`__ [[Paper](https://ieeexplore.ieee.org/document/9193901)]

 * <font color=DarkBlue><big>2020</big></font> - Radar Inertial Odometry With Online Calibration __`ENC`__ [[Paper](https://ieeexplore.ieee.org/document/9317343)]

 * <font color=DarkBlue><big>2020</big></font> - An EKF Based Approach to Radar Inertial Odometry __`MFI`__ [[Paper](https://ieeexplore.ieee.org/document/9235254)]

 * <font color=DarkBlue><big>2020</big></font> - Radar-Inertial Ego-Velocity Estimation for Visually Degraded Environments __`ICRA`__ [[Paper](https://ieeexplore.ieee.org/document/9196666)]

 * <font color=DarkBlue><big>2019</big></font> - Environment Mapping and Vehicle Localization with a High-Resolution Radar Prototype __`FAST-zero`__ [[Paper](https://www.researchgate.net/publication/344951866_Environment_Mapping_and_Vehicle_Localization_with_a_High-Resolution_Radar_Prototype)]

## Radar and Other Sensors Fusion

**Fusion of radar with lidar, camera, GNSS, and other sensors.**

- [ ] Add relevant resources.

## Radar Tensors

**Radar data representations, deep learning, and tensor-based methods.**

- [ ] Add relevant resources.

---

## Related Surveys

- [ ] List key papers and survey articles.

## Contributing

Contributions are welcome! Please open an issue or pull request to add new resources, fix errors, or suggest improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.