# IsaacSim_apple_image_generator
Code that changed object to apple in generating synthetic data code provided by IsaacSIm ~~2022.2.1~~ ~~2023.1.0~~ 2023.1.1
https://developer.nvidia.com/isaac-sim

IsaacSim이 설치된 폴더에서 붙여넣기 후 아래와 같이 터미널에서 입력해주면 됩니다.  
--num_mesh와 --num_dome은 각각 얻는 사진의 개수로, mesh는 YCB-Video Dataset의 data_syn과 같은 검은 화면에 오브젝트만 있는 이미지, dome은 배경이 포함되어 현실에서 촬영한 사진과 유사한 이미지입니다.
```
./python.sh standalone_examples/replicator/offline_pose_generation/apple_offline_pose_generation.py --num_mesh 2500 --num_dome 2500
```

사과, MESH의 모델파일(.usd)의 경우 직접 blender에서 만들거나 구할 수 있습니다.  
코드 내 경로, 모델파일 이름은 환경에 맞게 수정해야합니다.  

*IsaacSim2022.2.1 버전에서 만들어지는 정답 pose 데이터가 잘못되어 2023.1.0 버전으로 업데이트 후 이에 맞게 코드를 수정하였습니다.
