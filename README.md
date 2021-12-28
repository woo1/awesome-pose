# awesome-pose
* curated list for pose estimation
* 3DPW models : https://paperswithcode.com/sota/3d-human-pose-estimation-on-3dpw

## Human Mesh Recovery
* comment : 3DPW 데이터셋에서 정확도가 높은 모델들은 거의가 이미지 기반이라 중간에 튀는 경우가 다소 있습니다. 영상 기반 모델인 TCMR 같은 경우는 대체적으로 무난한 결과가 출력되지만 정확도가 아쉽습니다.
* <b>2020/08</b> frankmocap(3d body+hand motion capture) : Fast Monocular 3D Hand and Body Motion Capture by Regression and Integration [[paper]](https://arxiv.org/abs/2008.08324)[[code]](https://github.com/facebookresearch/frankmocap)[[skeleton info]](https://github.com/facebookresearch/frankmocap/blob/master/docs/joint_order.md)
* <b>2020/08</b> I2L-MeshNet : Image-to-Lixel Prediction Network for Accurate 3D Human Pose and Mesh Estimation from a Single RGB Image [[paper]](https://arxiv.org/abs/2008.03713)[[code]](https://github.com/mks0601/I2L-MeshNet_RELEASE)
* <b>2020/08</b> ROMP: Monocular, One-stage, Regression of Multiple 3D People [[paper]](https://arxiv.org/abs/2008.12272) [[code]](https://github.com/Arthur151/ROMP) : 실데이터 확인 시 준수한 성능을 보입니다.
* <b>2021/04</b> MeshGraphormer [[paper]](https://arxiv.org/abs/2104.00272) [[code]](https://github.com/microsoft/meshgraphormer) : Microsoft의 이전 논문인 METRO 논문에 GCNN을 추가하여 성능을 향상시킨 논문입니다. 실데이터로 확인 시 폐색에 취약한 결과를 나타냈습니다.
* <b>2021/04</b> PARE: Part Attention Regressor for 3D Human Body Estimation [[paper]](https://arxiv.org/abs/2104.08527) [[code]](https://github.com/mkocabas/PARE) : 실데이터 확인 시 준수한 성능을 보입니다.
* <b>2021/10</b> Learning to Regress Bodies from Images using Differentiable Semantic Rendering
 [[code]](https://github.com/saidwivedi/DSR) [[paper]](https://arxiv.org/abs/2110.03480)
* <b>2021/11</b> Out-of-Domain Human Mesh Reconstruction via Dynamic Bilevel Online Adaptation 
[[paper]](https://arxiv.org/abs/2111.04017) [[code]](https://github.com/syguan96/dynaboa) [[project]](https://sites.google.com/view/dynaboa) : 2021/12 기준 3DPW SOTA, unsupervised online adaption 기반의 모델이라는 점에서 개념적으로 좋지만, 해당 도메인에 대한 skeleton 데이터가 항상 필요하고, 해당 데이터로 학습 진행 후 추론하는 느낌입니다. 실데이터로 확인 시 결과가 좋지 않고, 시간이 너무 오래걸립니다.

## Human Mesh Recovery + Texture
* <b>2021/09</b> Texformer: 3D Human Texture Estimation from a Single Image with Transformers
 [[paper]](https://arxiv.org/abs/2109.02563) [[code]](https://github.com/xuxy09/Texformer)
* <b>2021/12</b> ICON: Implicit Clothed humans Obtained from Normals [[paper]](https://arxiv.org/pdf/2112.09127.pdf) [[code]](https://github.com/YuliangXiu/ICON)
* <b>2021/05</b> Animated 3D Human Avatars from a Single Image with GAN-based Texture Inference [[paper]](https://www.researchgate.net/profile/Zhong-Li-16/publication/348875382_Animated_3D_Human_Avatars_from_a_Single_Image_with_GAN-based_Texture_Inference/links/60a692cb299bf1031f06f4c9/Animated-3D-Human-Avatars-from-a-Single-Image-with-GAN-based-Texture-Inference.pdf) : 단일 이미지에서 GAN을 이용해 Texture를 만들도록 하는 논문

## SMPL Clothes
* <b>2021/03</b> SMPLicit: Topology-aware Generative Model for Clothed People
 [[paper]](https://arxiv.org/pdf/2103.06871.pdf) [[code]](https://github.com/enriccorona/SMPLicit) : 기존 SMPL 모델의 top에 clothes layer를 얹어서 만든 모델로 기존 SMPL과 별개의 모델 파일이 따로 있음. pifuHD, tex2Shape에 비해 더 정교한 옷의 질감 표현 가능. image에 fitting하는 코드([[fit_SMPLicit]](https://github.com/enriccorona/SMPLicit/tree/main/fit_SMPLicit))가 Repo 내에 별도로 존재함.

## 3d Pose estimation (3d skeleton)
* <b>2017/05</b> ColorHandPose3D : Learning to Estimate 3D Hand Pose from Single RGB Images
 [[code]](https://github.com/lmb-freiburg/hand3d)
* <b>2018/11</b> VideoPose3D : 3D human pose estimation in video with temporal convolutions and semi-supervised training [[paper]](https://arxiv.org/abs/1811.11742)[[code]](https://github.com/facebookresearch/VideoPose3D)

## 2d Pose estimation
* <b>2018/12</b> OpenPose: Real-time multi-person keypoint detection library for body, face, hands, and foot estimation [[paper]](https://arxiv.org/abs/1812.08008) [[code]](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
* <b>2020/12</b> TransPose: Keypoint Localization via Transformer [[paper]](https://arxiv.org/pdf/2012.14214.pdf) [[code]](https://github.com/yangsenius/TransPose) : Transformer 기반의 2D Pose Estimation (Openpose보다 성능 좋음)

## dataset
* Human Foot Keypoint Dataset(2d) : [[url]](https://cmu-perceptual-computing-lab.github.io/foot_keypoint_dataset/)[[code]](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train)
* <b>2020/07</b> Coco Whole Body : Whole-Body Human Pose Estimation in the Wild [[paper]](https://arxiv.org/abs/2007.11858)[[code]](https://github.com/jin-s13/COCO-WholeBody)

## etc
* <b>2018/12</b> PoseFix : Model-agnostic General Human Pose Refinement Network [[paper]](https://arxiv.org/abs/1812.03595)[[code]](https://github.com/mks0601/PoseFix_RELEASE)
* Bodyvisualizer(3d mesh by gender, height, weight, etc) : [[url]](https://bodyvisualizer.com/male.html)

