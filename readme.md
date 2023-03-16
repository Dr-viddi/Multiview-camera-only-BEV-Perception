# About this project
Here is a list of current papers for bird's eye view perception from only multi camera input. The approaches can be divided based on how the transformation from camera Image 2D (perspective view) to BEV persepective is done:
* Transformer based: projects the perspective view features onto the BEV plane using transformers and more precisley the attention mechanism. This method first designs a set of BEV queries using positional encoding, then performs the view  ransformation through cross attention between BEV queries and the image features
* MLP based: utilize MLP as a general mapping function to model the transformation from perspective view to bird’s eye view
* Depth based:  built on an explicit 3D representation, quantized voxels, or point clouds scattering in continuous 3D space (via depth predictions). Point-based methods directly use the depth estimation to convert pixels to point clouds (pseudo lidar) wheras voxel-Based methods scatters 2D features (instead of points) at the corresponding 3D locations directly with the depth guidance
* Homograph based: rely on physical mapping of the flat ground between perspective view and bird’s eye view

## Transformer based approaches
### 2023
* [Tri-Perspective View for Vision-Based 3D Semantic Occupancy Prediction](https://arxiv.org/abs/2302.07817)
* [OA-BEV: Bringing Object Awareness to Bird's-Eye-View Representation for Multi-Camera 3D Object Detection](https://arxiv.org/abs/2301.05711)
* [FrustumFormer: Adaptive Instance-aware Resampling for Multi-view 3D Detection](https://arxiv.org/abs/2301.04467)
### 2022
* [BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers](https://arxiv.org/abs/2203.17270)
* [BEVFormer v2: Adapting Modern Image Backbones to Bird's-Eye-View Recognition via Perspective Supervision](https://arxiv.org/abs/2211.10439)
* [Delving into the Devils of Bird's-eye-view Perception: A Review, Evaluation and Recipe](https://arxiv.org/abs/2209.05324)
* [Cross-view Transformers for real-time Map-view Semantic Segmentation](https://arxiv.org/abs/2205.02833)
* [PETRv2: A Unified Framework for 3D Perception from Multi-Camera Images](https://arxiv.org/abs/2206.01256)
* [Learning Ego 3D Representation as Ray Tracing](https://arxiv.org/abs/2206.04042)
* [Efficient and Robust 2D-to-BEV Representation Learning via Geometry-guided Kernel Transformer](https://arxiv.org/abs/2206.04584)
* [LaRa: Latents and Rays for Multi-Camera Bird's-Eye-View Semantic Segmentation](https://arxiv.org/abs/2206.13294)
* [PolarFormer: Multi-camera 3D Object Detection with Polar Transformer](https://arxiv.org/abs/2206.15398)
* [PETR: Position Embedding Transformation for Multi-View 3D Object Detection](https://arxiv.org/abs/2203.05625)
* [CoBEVT: Cooperative Bird's Eye View Semantic Segmentation with Sparse Transformers](https://arxiv.org/abs/2207.02202)
* [BEVSegFormer: Bird's Eye View Semantic Segmentation From Arbitrary Camera Rigs](https://arxiv.org/abs/2203.04050)
* [UniFormer: Unified Multi-view Fusion Transformer for Spatial-Temporal Representation in Bird's-Eye-View](https://arxiv.org/abs/2207.08536)
* [BEVDepth: Acquisition of Reliable Depth for Multi-view 3D Object Detection](https://arxiv.org/abs/2206.10092)
* [DETR4D: Direct Multi-View 3D Object Detection with Sparse Attention](https://arxiv.org/abs/2212.07849)
* [Multi-Camera Calibration Free BEV Representation for 3D Object Detection](https://arxiv.org/abs/2210.17252)
* [MapTR: Structured Modeling and Learning for Online Vectorized HD Map Construction](https://arxiv.org/abs/2208.14437)
### 2021
* [DETR3D: 3D Object Detection from Multi-view Images via 3D-to-2D Queries](https://arxiv.org/abs/2110.06922)

## MLP based approaches
### 2021
* [HDMapNet: An Online HD Map Construction and Evaluation Framework](https://arxiv.org/abs/2107.06307)

## Depth based approaches
### 2023
* [Fast-BEV: A Fast and Strong Bird's-Eye View Perception Baseline](https://arxiv.org/abs/2301.12511)
### 2022
* [M2BEV: Multi-Camera Joint 3D Detection and Segmentation with Unified Birds-Eye View Representation](https://arxiv.org/abs/2204.05088)
* [BEVerse: Unified Perception and Prediction in Birds-Eye-View for Vision-Centric Autonomous Driving](https://arxiv.org/abs/2205.09743)
* [ST-P3: End-to-end Vision-based Autonomous Driving via Spatial-Temporal Feature Learning](https://arxiv.org/abs/2207.07601)
* [BEVStereo: Enhancing Depth Estimation in Multi-view 3D Object Detection with Dynamic Temporal Stereo](https://arxiv.org/abs/2209.10248)
* [MatrixVT: Efficient Multi-Camera to BEV Transformation for 3D Perception](https://arxiv.org/abs/2211.10593)
* [BEV-Seg: Bird's Eye View Semantic Segmentation Using Geometry and Semantic Point Cloud](https://arxiv.org/abs/2006.11436)
### 2021
* [FIERY: Future Instance Prediction in Bird's-Eye View from Surround Monocular Cameras](https://arxiv.org/abs/2104.10490)
### 2020
* [Lift, Splat, Shoot: Encoding Images From Arbitrary Camera Rigs by Implicitly Unprojecting to 3D](https://arxiv.org/abs/2008.05711)

## Homograph based approaches
### 2020
* [A Sim2Real Deep Learning Approach for the Transformation of Images from Multiple Vehicle-Mounted Cameras to a Semantically Segmented Image in Bird's Eye View](https://arxiv.org/abs/2005.04078)
