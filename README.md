# awesome-pose
* curated list for pose estimation
* 3DPW models : https://paperswithcode.com/sota/3d-human-pose-estimation-on-3dpw

## Human Mesh Recovery
* comment : 3DPW 데이터셋에서 정확도가 높은 모델들은 거의가 이미지 기반이라 중간에 튀는 경우가 다소 있습니다. 영상 기반 모델인 TCMR 같은 경우는 대체적으로 무난한 결과가 출력되지만 정확도가 아쉽습니다.
* frankmocap(3d body+hand motion capture) : Fast Monocular 3D Hand and Body Motion Capture by Regression and Integration(2020-08) [[paper]](https://arxiv.org/abs/2008.08324)[[code]](https://github.com/facebookresearch/frankmocap)[[skeleton info]](https://github.com/facebookresearch/frankmocap/blob/master/docs/joint_order.md)
* I2L-MeshNet : Image-to-Lixel Prediction Network for Accurate 3D Human Pose and Mesh Estimation from a Single RGB Image(2020-08) [[paper]](https://arxiv.org/abs/2008.03713)[[code]](https://github.com/mks0601/I2L-MeshNet_RELEASE)
* Out-of-Domain Human Mesh Reconstruction via Dynamic Bilevel Online Adaptation(2021-11) 
[[paper]](https://arxiv.org/abs/2111.04017) [[code]](https://github.com/syguan96/dynaboa) [[project]](https://sites.google.com/view/dynaboa) : 2021/12 기준 3DPW SOTA,unsupervised online adaption 기반의 모델이라는 점에서 개념적으로 좋지만, 해당 도메인에 대한 skeleton 데이터가 항상 필요하고, 해당 데이터로 학습 진행 후 추론하는 느낌입니다. 실데이터로 확인 시 결과가 좋지 않고, 속도가 너무 오래걸렸습니다.
* MeshGraphormer (2021-04) [[paper]](https://arxiv.org/abs/2104.00272) [[code]](https://github.com/microsoft/meshgraphormer) : Microsoft의 이전 논문인 METRO 논문에 GCNN을 추가하여 성능을 향상시킨 논문입니다. 실데이터로 확인 시 폐색에 취약한 결과를 나타냈습니다.
* PARE: Part Attention Regressor for 3D Human Body Estimation (2021-04) [[paper]](https://arxiv.org/abs/2104.08527) [[code]](https://github.com/mkocabas/PARE) : 실데이터 확인 시 준수한 성능을 보입니다.
* ROMP: Monocular, One-stage, Regression of Multiple 3D People (2020-08) [[paper]](https://arxiv.org/abs/2008.12272) [[code]](https://github.com/Arthur151/ROMP) : 실데이터 확인 시 준수한 성능을 보입니다.

## 3d Pose estimation (3d skeleton)
* VideoPose3D : 3D human pose estimation in video with temporal convolutions and semi-supervised training(2018-11) [[paper]](https://arxiv.org/abs/1811.11742)[[code]](https://github.com/facebookresearch/VideoPose3D)
* ColorHandPose3D : Learning to Estimate 3D Hand Pose from Single RGB Images(2017-05)
 [[code]](https://github.com/lmb-freiburg/hand3d)

## dataset
* Human Foot Keypoint Dataset(2d) : [[url]](https://cmu-perceptual-computing-lab.github.io/foot_keypoint_dataset/)[[code]](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train)
* Coco Whole Body : Whole-Body Human Pose Estimation in the Wild(2020-07) [[paper]](https://arxiv.org/abs/2007.11858)[[code]](https://github.com/jin-s13/COCO-WholeBody)

## etc
* PoseFix : Model-agnostic General Human Pose Refinement Network(2018-12) [[paper]](https://arxiv.org/abs/1812.03595)[[code]](https://github.com/mks0601/PoseFix_RELEASE)
* Bodyvisualizer(3d mesh by gender, height, weight, etc) : [[url]](https://bodyvisualizer.com/male.html)

