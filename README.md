<aside>
💡

**OverView of the Project**


- Opening background information 

- General description of the current project 

- Proposed idea for enhancements to the project

- Value and significance of this project 

- Current limitations 

- Literature review 

</aside>

# Title

[Topic]

Camera-based assistance feature for visually impaired pedestrians at crosswalks

---

**Crosswalk assistance function for the visually impaired using cameras**

# Opening background information

[ 배경 정보 ]

<aside>
✅ - Visually impaired individuals face numerous challenges in their daily lives, particularly when navigating intersections and traffic lights safely. While some cities have implemented audio signal systems at traffic lights, the high installation costs and regional limitations have prevented widespread adoption. As a result, there is a growing demand for assistive technologies that are both affordable and accessible to address these issues.

</aside>

---



# General description of the current project

[Overall project description]

<aside>
✅This project leverages YOLOv5 (a state-of-the-art object detection algorithm) to detect traffic lights in real time and convey relevant information to visually impaired individuals.

- The system uses YOLOv5 to identify the status of traffic lights (green, red, yellow).
- Information is relayed to users through auditory outputs (voice notifications) and haptic feedback (vibrations).
- The solution is designed to operate on cost-effective hardware (e.g., Raspberry Pi or smartphones) to enable easy deployment
</aside>

---

.

# **Proposed idea for enhancements to the project**



<aside>
✅- Optimize the system by employing a lightweight version of YOLOv5 to enhance processing speed and compatibility with low-spec devices.
- Incorporate multitasking capabilities to detect additional elements, such as vehicle movement and pedestrian signals, to improve safety.
- Develop a cloud-based data update mechanism to continuously train and improve the model for diverse traffic environments.
- **Detailed Decision-Making**: Beyond simply detecting green lights, the system is trained to **recognize when a countdown timer is flashing**, indicating that it is unsafe to cross, and provide appropriate guidance to the user.


</aside>

---



# Value and signifiance of the project


<aside>
✅- **Social Impact:** Significantly improves the safety and mobility of visually impaired individuals while reducing pedestrian accidents.
- **Technological Innovation:** Effectively integrates YOLOv5-based real-time object detection technology into assistive devices.
- **Economic Feasibility:** Provides a cost-efficient solution without requiring large-scale infrastructure changes.



</aside>

---


# **Current limitations**



<aside>
✅- Variations in the position and size of traffic lights pose challenges in dataset collection and model generalization.
- Environmental factors (e.g., weather conditions, lighting changes, obstructions) may affect detection accuracy.
- Real-time processing may require high-performance hardware, which poses a challenge to achieving cost-efficiency.


</aside>

---



# **Literature review**


<aside>
✅
- **YOLOv5 Research:** The latest version of the YOLO (You Only Look Once) model, optimized for real-time object detection, offers exceptional accuracy and speed across various applications.
    - Redmon et al., "YOLO: Real-Time Object Detection," CVPR, 2016.
    - Jocher et al., "YOLOv5 Documentation," Ultralytics, 2020.
- **Assistive Technology for the Visually Impaired:** Prior studies highlight the use of vibration signals, audio guidance systems, and RFID-based traffic light detection as key technologies.
    - Sharma et al., "Assistive Devices for Visually Impaired," IJERT, 2019.
    - Kim et al., "Smart Crosswalk System for Visually Impaired Pedestrians," IEEE Access, 2020.
- **Object Detection under Environmental Variability:** Studies on data augmentation techniques and ensemble learning have addressed challenges posed by lighting changes and object occlusion.

</aside>

---



[]()

# YOLOv5 training completed / results

[]()![image](https://github.com/user-attachments/assets/7277e144-46e9-4635-b51b-90e57b8abd30)


![image (1)](https://github.com/user-attachments/assets/0977cf9a-6d87-4548-b892-82eb048261ee)


[]()

[]()

# Methods of obtaining video

1. "Pedestrian signal video is included in the video to download."
2. https://www.zaivhub.com/ko/yolov5
     "Through the site, you can download the DarkLabel program and the data.yaml file, and then use them to convert the collected videos and images into labeled images."





    
3. "Open and edit the DarkLabel.yml file." 

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



1. After completing the labeling, save the images and gt.

1. Edit the data.yaml file.

```python
names:  # Classes name
- red_sign
- yellow_sign
- count

train: /content/drive/MyDrive/yolov5/Train/images  
val: /content/drive/MyDrive/yolov5/Val 
```

```python
sudo apt-get install git
glt clone https://github.com/ultralytics/yolov5.git

sudo apt-get install pip
cd yolov5
pip install -r requiremets.txt
```

1. Place the images and labeled photos inside yolov5 → train →

```python
python3 detect.py --source <input_path> --weights <weight_file_path> --conf <confidence_threshold> --save-txt --save-conf --img-size <image_size>


```

1. Verification of model training and validation results

```python
python3 detect.py --source /path/to/input --weights /home/amap/yolov5/runs/train/lane_1000/weights/best.pt --img 64 --conf 0.4 --save-txt --save-conf

```

