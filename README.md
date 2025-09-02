# RF-PGS
RF-PGS is a novel framework for fully-structured spatial wireless channel representation based on Planar Gaussian Splatting, enabling accurate and efficient modeling of full radio propagation paths. 
[**[2508.16849] RF-PGS: A Fully-Structured Radio Propagation Representation with Planar Gaussian Splatting**](https://arxiv.org/abs/2508.16849)

Code will be released upon paper acceptance.

https://github.com/user-attachments/assets/164d5419-922c-4ba8-a04b-2f810a4ab9f0

## RF-PGS Demonstration

- **Raw demonstration video**: [Google Drive](https://drive.google.com/file/d/1J0dnE6pWZOmRf1BrkckxNSQiCJIZQPS6/view?usp=sharing)  
- **Measured MPC visualization**: Based on field measurements conducted by **NIST USA**, details available in [this paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10501217).  
- **Ground truth**: Simulation results generated with the [Sionna simulator](https://nvlabs.github.io/sionna/), serving as the training and test data source for RF-PGS.  

### Improvements over RF-3DGS
As the successor of our previous work [RF-3DGS](https://github.com/SunLab-UGA/RF-3DGS), **RF-PGS** introduces several key enhancements:

1. **Greatly simplified training requirements**:  
   The RF training stage now requires only the Rx-side path loss spectra while still enabling reconstruction of the time-of-flight (ToF) and angle-of-departure (AoD) for each multipath component (MPC).  

2. **Fully-structured radio radiance field**:  
   RF-PGS explicitly incorporates propagation distance into the model, allowing direct querying at the Tx-side (AoD domain) without transformation from the Rx-side (AoA domain).  

3. **RF-specific enhancements**:  
   By introducing Planar Gaussians with RF-oriented modifications, RF-PGS achieves more accurate environment representation and enables the extraction of surface-level RF parameters.  

