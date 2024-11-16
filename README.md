<aside>
💡

**OverView of the Project**

프로젝트 개요

- Opening background information (내 프로젝트의 전반적인 문맥을 위해서 필요!)

- General description of the current project (프로젝트의 전반적인 설명)

- Proposed idea for enhancements to the project (제안하고 싶은 프로젝트의 강점)

- Value and significance of this project (중요성)

- Current limitations (직면하고 있는 한계)

- Literature review (전반적인 프로젝트의 배경지식 공유를 위해서!)

</aside>

# Title

[주제]

카메라를 활용한 시각장애인 횡단보도 보조기능

---

**Crosswalk assistance function for the visually impaired using cameras**

# Opening background information

[ 배경 정보 ]

<aside>
✅ 시각장애인들은 일상생활에서 다양한 장애물을 마주하며, 특히 교차로와 신호등을 안전하게 통과하는 것이 큰 도전이 됩니다. 현재 많은 도시에서는 음성 안내 신호등을 설치하고 있지만, 이 시스템은 설치 비용과 지역적 한계로 인해 충분히 보급되지 못하고 있습니다. 따라서 보조 기술의 필요성이 지속적으로 증가하고 있으며, 보다 저비용으로 접근 가능한 솔루션이 요구됩니다.

</aside>

---

- Visually impaired individuals face numerous challenges in their daily lives, particularly when navigating intersections and traffic lights safely. While some cities have implemented audio signal systems at traffic lights, the high installation costs and regional limitations have prevented widespread adoption. As a result, there is a growing demand for assistive technologies that are both affordable and accessible to address these issues.

# General description of the current project

[프로젝트 전반적인 설명]

<aside>
✅ 본 프로젝트는 YOLOv5(Object Detection 알고리즘)을 활용하여 신호등을 실시간으로 인식하고, 시각장애인들에게 적합한 방식으로 정보를 제공하는 시스템을 개발하는 것을 목표로 합니다.

- YOLOv5를 사용하여 신호등의 상태(녹색, 적색, 황색)를 감지합니다.
- 신호등 데이터를 기반으로 음성 출력 및 진동 피드백 등의 인터페이스를 통해 시각장애인에게 정보를 전달합니다.
- 시스템은 저비용 하드웨어(예: Raspberry Pi, 스마트폰)와 연동하여 현장 배포가 용이하도록 설계됩니다.
</aside>

---

This project leverages YOLOv5 (a state-of-the-art object detection algorithm) to detect traffic lights in real time and convey relevant information to visually impaired individuals.

- The system uses YOLOv5 to identify the status of traffic lights (green, red, yellow).
- Information is relayed to users through auditory outputs (voice notifications) and haptic feedback (vibrations).
- The solution is designed to operate on cost-effective hardware (e.g., Raspberry Pi or smartphones) to enable easy deployment.

# **Proposed idea for enhancements to the project**

[제안하고 싶은 프로젝트의 강점]

<aside>
✅

- YOLOv5의 경량화된 모델을 활용해 시스템의 연산 속도를 개선하고, 저사양 기기에서도 실행 가능하도록 최적화합니다.
- 신호등 외에도 차량의 움직임이나 보행자 신호를 추가로 감지하는 멀티태스킹 기능을 통합하여 안전성을 높입니다.
- 클라우드 기반 데이터 업데이트 시스템을 구축해 다양한 교차로 환경에 맞게 모델을 지속적으로 학습 및 개선할 수 있도록 합니다.
- **세부 판단 기능**: 단순히 초록불인지 여부를 판단하는 것을 넘어, **숫자가 깜빡이는 경우에도 이를 인식하여 사용자가 건너서는 안 되는 상황을 안내**할 수 있는 고급 학습 모델을 포함.
</aside>

---

- Optimize the system by employing a lightweight version of YOLOv5 to enhance processing speed and compatibility with low-spec devices.
- Incorporate multitasking capabilities to detect additional elements, such as vehicle movement and pedestrian signals, to improve safety.
- Develop a cloud-based data update mechanism to continuously train and improve the model for diverse traffic environments.
- **Detailed Decision-Making**: Beyond simply detecting green lights, the system is trained to **recognize when a countdown timer is flashing**, indicating that it is unsafe to cross, and provide appropriate guidance to the user.

# Value and signifiance of the project

[ 프로젝트의 중요성] 

<aside>
✅

- **사회적 가치:** 시각장애인의 이동 안전성을 크게 향상시키며, 교통사고를 예방할 수 있습니다.
- **기술적 혁신:** YOLOv5를 활용한 실시간 객체 감지 기술을 장애인 보조기기에 효과적으로 접목합니다.
- **경제적 이점:** 대규모 인프라를 변경하지 않고 개인용 기기로 구현 가능해 비용 효율적입니다.
</aside>

---

- **Social Impact:** Significantly improves the safety and mobility of visually impaired individuals while reducing pedestrian accidents.
- **Technological Innovation:** Effectively integrates YOLOv5-based real-time object detection technology into assistive devices.
- **Economic Feasibility:** Provides a cost-efficient solution without requiring large-scale infrastructure changes.

# **Current limitations**

[직면하고 있는 한계]

<aside>
✅

- **환경 변화**: 날씨, 조명 조건, 복잡한 배경 등에서 객체 탐지의 성능이 감소할 가능성.
- **데이터 부족**: 다양한 신호등 상태와 환경을 포괄하는 훈련 데이터 부족.
- **하드웨어 제약**: 저사양 장치에서 실시간 탐지 성능을 유지하기 위한 최적화 필요.
- **사용자 피드백 부족**: 초기 단계에서는 실제 시각장애인의 요구사항 반영이 제한될 수 있음.
</aside>

---

- Variations in the position and size of traffic lights pose challenges in dataset collection and model generalization.
- Environmental factors (e.g., weather conditions, lighting changes, obstructions) may affect detection accuracy.
- Real-time processing may require high-performance hardware, which poses a challenge to achieving cost-efficiency.

# **Literature review**

[문헌 고찰]

<aside>
✅

- **YOLOv5 관련 연구**: YOLO(You Only Look Once) 모델의 최신 버전으로, 실시간 객체 탐지에 최적화된 경량 알고리즘. 다양한 응용 분야에서 높은 정확성과 속도를 자랑함.
    - Redmon et al., "YOLO: Real-Time Object Detection," CVPR, 2016.
    - Jocher et al., "YOLOv5 Documentation," Ultralytics, 2020.
- **시각장애인을 위한 교통 보조 기술**: 기존 연구에서는 진동 신호, 음성 안내 시스템, RFID 기반의 신호등 탐지 등이 주요 기술로 사용됨.
    - Sharma et al., "Assistive Devices for Visually Impaired," IJERT, 2019.
    - Kim et al., "Smart Crosswalk System for Visually Impaired Pedestrians," IEEE Access, 2020.
- **환경적 요인과 객체 탐지**: 조도 변화와 객체 occlusion(가림 효과) 문제 해결을 위한 데이터 증강 기술 및 앙상블 학습에 대한 연구가 진행 중.
</aside>

---

- **YOLOv5 Research:** The latest version of the YOLO (You Only Look Once) model, optimized for real-time object detection, offers exceptional accuracy and speed across various applications.
    - Redmon et al., "YOLO: Real-Time Object Detection," CVPR, 2016.
    - Jocher et al., "YOLOv5 Documentation," Ultralytics, 2020.
- **Assistive Technology for the Visually Impaired:** Prior studies highlight the use of vibration signals, audio guidance systems, and RFID-based traffic light detection as key technologies.
    - Sharma et al., "Assistive Devices for Visually Impaired," IJERT, 2019.
    - Kim et al., "Smart Crosswalk System for Visually Impaired Pedestrians," IEEE Access, 2020.
- **Object Detection under Environmental Variability:** Studies on data augmentation techniques and ensemble learning have addressed challenges posed by lighting changes and object occlusion.

[]()

# yolo5 학습 종료 /결과

[]()![image](https://github.com/user-attachments/assets/7277e144-46e9-4635-b51b-90e57b8abd30)


![image (1)](https://github.com/user-attachments/assets/0977cf9a-6d87-4548-b892-82eb048261ee)


[]()

[]()

# 영상 취득 방법

1. 보행자 신호 영상이 들어있는 영상을 다운로드한다.
2. https://www.zaivhub.com/ko/yolov5
    
    해당 사이트를 통하여 DarkLabel 프로그램과 data.yaml 파일을 다운 받은 후에 사용하여 수집한 영상 및 이미지에 대해 라벨이 달린 이미지로 변환이 가능합니다.
    
3. DarkLabel.yml 파일을 열고 수정을 한다. 

```python
traffic_signal: ["red_sign","yellow_sign","count"]

format10:    # bird detection yolo (predefined format]
  fixed_filetype: 1                 # if specified as true, save setting isn't changeable in GUI
  data_fmt: [classid, ncx, ncy, nw, nh]
  gt_file_ext: "txt"                 # if not specified, default setting is used
  gt_merged: 0                    # if not specified, default setting is used
  delimiter: " "                     # if not spedified, default delimiter(',') is used
  classes_set: "traffic_signal"     # if not specified, default setting is used
  name: "traffic_signal"
```
![image (2)](https://github.com/user-attachments/assets/2026aac9-ef18-40ae-b7b0-6398d30bda81)



1. 라벨링을 진행 해준뒤 images 와 gt를 저장해준다.

1. data .yaml 파일을수정해준다. 

```python
names:  # Classes name
- red_sign
- yellow_sign
- count

train: /content/drive/MyDrive/yolov5/Train/images  # train images 경로
val: /content/drive/MyDrive/yolov5/Val # val images 경로
```

```python
sudo apt-get install git
glt clone https://github.com/ultralytics/yolov5.git

sudo apt-get install pip
cd yolov5
pip install -r requiremets.txt
```

1. 이미지와 라벨링한 사진을 yolov5 → train→  안에 넣어준다.

```python
python3 detect.py --source <입력 경로> --weights <가중치 파일 경로> --conf <신뢰도 임계값> --save-txt --save-conf --img-size <이미지 크기>

```

1. 모델 학습검증 결과 검증

```python
python3 detect.py --source /path/to/input --weights /home/amap/yolov5/runs/train/lane_1000/weights/best.pt --img 64 --conf 0.4 --save-txt --save-conf

```

