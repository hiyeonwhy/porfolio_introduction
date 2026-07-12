<div align="center">

# Hi 👋, I'm Hiyeon Woo

### Embedded Systems · Robotics · Autonomous Driving

하드웨어와 소프트웨어의 경계를 이해하고,  
실제 환경에서 안정적으로 동작하는 시스템을 만드는 개발자입니다.

`Embedded` `FPGA` `ROS` `Computer Vision` `System Verification`

</div>

---

## 🌱 About Me

- 경북대학교 **전자공학부**에서 임베디드 시스템, 제어, 디지털 시스템을 공부했습니다.
- ARM Processor, FPGA, MCU부터 ROS 기반 자율주행과 AI 영상 분석까지 경험했습니다.
- 단순히 기능을 구현하는 것에 그치지 않고, **로그와 데이터를 기반으로 오류의 원인을 추적하고 개선하는 과정**을 중요하게 생각합니다.
- 실험·실차 테스트·RMSE 분석·rosbag 비교를 통해 시스템의 안정성과 성능을 검증해 왔습니다.
- 임베디드 및 로보틱스 개발을 기반으로 **시험평가, 검증, 신뢰성 및 품질 개선 분야**에 관심이 있습니다.

---

## 🔭 Interests

- **Embedded Systems**
  - ARM MCU, Peripheral Control, Device Driver
  - Real-time System, Hardware Interface

- **HW/SW Co-design**
  - Zynq SoC, ARM Processor, FPGA
  - AXI4-Lite, Custom IP, Memory-mapped I/O

- **Robotics & Autonomous Driving**
  - ROS1 / ROS2, SLAM, Navigation
  - AMCL, Costmap, Sensor Fusion, Collision Avoidance

- **Computer Vision**
  - Object Detection, Pose Estimation
  - YOLO, OpenCV, PyTorch

- **System Verification**
  - Log-based Debugging
  - RMSE Analysis, Repeated Testing, Parameter Tuning

---

## 🛠 Tech Stack

### Embedded & Hardware

`C` `C++` `Verilog HDL` `Zynq-7000` `ARM Cortex-A9`  
`ARM Cortex-M4F` `S32K144` `FPGA` `AXI4-Lite`  
`UART` `GPIO` `Interrupt` `Timer` `FATFS`

### Robotics

`ROS1` `ROS2` `Nav2` `SLAM` `AMCL`  
`Costmap` `Gazebo` `rosbag` `TF` `LiDAR` `IMU`

### AI & Computer Vision

`Python` `YOLOv11` `YOLO Pose` `OpenCV`  
`PyTorch` `NumPy` `Computer Vision`

### Web & Data

`Django` `Django REST Framework` `Vue 3`  
`Vite` `Pinia` `REST API` `JSON` `RDBMS`

### Development Tools

`Linux` `Git` `GitHub` `Vivado` `Xilinx SDK`  
`Jetson Nano` `Jetson Orin Nano` `MATLAB`

---
## 📊 Language Statistics

<p align="center">
  <img
    src="https://github-stats-extended.vercel.app/api/top-langs/?username=hiyeonwhy&layout=compact&langs_count=8&custom_title=Most%20Used%20Languages&title_color=2f80ed&text_color=434d58&bg_color=ffffff&border_color=d8dee4&card_width=380"
    alt="hiyeonwhy Most Used Languages"
  />
  <br/><br/>
  <img
    src="https://komarev.com/ghpvc/?username=hiyeonwhy&label=Profile%20views&color=0e75b6&style=flat"
    alt="hiyeonwhy Profile Views"
  />
</p>
---

## 🚀 Featured Projects

### 1. SoC 기반 실시간 색칠 게임 시스템

> Zynq SoC의 ARM Processor와 FPGA를 연동한 HW/SW 통합 시스템

- **기간:** 2025.05 ~ 2025.06
- **역할:** 팀장 및 HW/SW 통합 개발
- Zynq-7000의 PS와 PL을 **AXI4-Lite Custom Peripheral**로 연동했습니다.
- TFT-LCD, TextLCD, 7-Segment, UART, SD Card를 하나의 시스템으로 통합했습니다.
- BRAM과 FATFS를 활용하여 RGB565 이미지 데이터를 TFT-LCD에 출력했습니다.
- 사용자 로그인, 게임 선택, 색칠 판정, 완료 검출 및 점수 관리 기능을 구현했습니다.
- 메모리 주소 충돌, XDC 핀 중복, IO 배치 오류와 같은 HW/SW 통합 문제를 해결했습니다.

**Tech Stack**

`Zynq-7000` `ARM Cortex-A9` `FPGA` `Verilog`  
`C` `AXI4-Lite` `Vivado` `Xilinx SDK` `FATFS`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

### 2. 공장 내 안전사고 감지 UGV

> 자율주행 로봇이 공장 내부를 순찰하며 작업자 쓰러짐과 연기를 감지하는 시스템

- 기업 연계 팀 프로젝트로 진행했습니다.
- ROS2 기반 UGV에 YOLO 영상 분석 노드를 연동했습니다.
- YOLO Pose 모델을 활용하여 작업자의 **쓰러짐 자세**를 감지했습니다.
- Custom YOLO 모델을 활용하여 공장 내부의 **연기 발생 상황**을 감지했습니다.
- 감지 결과를 ROS2 Topic으로 발행하여 관리자 시스템으로 전달했습니다.
- 단일 프레임 오검출을 줄이기 위해 Sliding Window 기반 필터링 로직을 적용했습니다.
- Camera Topic 불일치, Launch Remapping, OpenCV 처리 지연 문제를 분석하고 개선했습니다.

**Tech Stack**

`ROS2` `Jetson Nano` `Python` `YOLOv11 Pose`  
`OpenCV` `PyTorch` `CvBridge` `v4l2_camera`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

### 3. F1TENTH 충돌 예측 및 긴급 제동

> LiDAR 데이터를 활용한 ROS2 기반 자율주행 차량 충돌 방지 시스템

- LiDAR 거리와 차량 속도를 기반으로 TTC(Time To Collision)를 계산했습니다.
- 충돌 위험이 기준값 이하로 판단되면 차량을 즉시 정지하도록 구현했습니다.
- 불필요한 장애물 데이터를 제외하기 위해 ROI 기반 LiDAR 필터링을 적용했습니다.
- 주행 환경에 따라 제동 기준을 조절하는 Adaptive Threshold 방식을 적용했습니다.
- 시뮬레이션과 실차 테스트를 반복하며 제동 안정성을 검증했습니다.

**Tech Stack**

`ROS2` `F1TENTH` `LiDAR` `TTC`  
`Python` `C++` `Gazebo`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

### 4. TurtleBot SLAM 및 Navigation 성능 개선

> 지도 오차와 반복 충돌 문제를 분석하여 자율주행 안정성을 개선한 프로젝트

- ROS1 기반 Mapping, AMCL, Navigation을 구성했습니다.
- 특정 구간에서 반복적으로 발생하는 위치 오차와 벽 충돌 문제를 분석했습니다.
- 로그와 지도 데이터를 확인하여 초기 지도 생성 과정의 누적 오차를 원인으로 판단했습니다.
- 지도를 재생성하고 AMCL 및 Costmap 파라미터를 조정했습니다.
- rosbag을 활용하여 주행 데이터를 기록하고 경로 및 RMSE를 비교했습니다.
- 속도 변화와 IMU 적용 여부가 SLAM 정확도에 미치는 영향을 분석했습니다.

**Tech Stack**

`ROS1` `TurtleBot` `SLAM` `AMCL`  
`Navigation` `Costmap` `rosbag` `LiDAR` `IMU`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

### 5. GotYA 문화 콘텐츠 추천 서비스

> 사용자의 취향을 기반으로 영화, 도서, 문화행사를 추천하는 웹 서비스

- Django REST Framework와 Vue 3를 활용한 웹 서비스를 개발했습니다.
- 영화, 도서, 문화행사 데이터를 JSON으로 정제하여 Django ORM으로 적재했습니다.
- 외부 콘텐츠 ID를 기준으로 기존 데이터는 갱신하고 신규 데이터는 추가하는 Upsert 구조를 구현했습니다.
- 콘텐츠 검색, 필터링, 좋아요, 다시 보지 않기, 마이페이지 기능을 구현했습니다.
- Custom User 모델과 서비스 요구사항을 기준으로 ERD를 개선했습니다.
- 반복적인 데이터 적재 작업을 개선하기 위한 데이터 파이프라인 구조를 설계했습니다.

**Tech Stack**

`Django` `Django REST Framework` `Vue 3`  
`Vite` `Pinia` `REST API` `Django ORM`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

### 6. S32K144 암호 통신 장치

> ARM Cortex-M4F MCU의 주변장치를 통합한 임베디드 시스템

- S32K144 기반 GPIO, UART, LPIT Timer, Keypad, TextLCD, 7-Segment를 제어했습니다.
- Keypad 입력과 UART 통신을 활용한 암호 입력 및 출력 시스템을 구현했습니다.
- 다중 외부 인터럽트 사용 시 발생하던 과도한 Interrupt Trigger 문제를 분석했습니다.
- 입력 처리 방식을 Timer 기반 Polling 구조로 변경하여 시스템 안정성을 개선했습니다.

**Tech Stack**

`S32K144` `ARM Cortex-M4F` `C`  
`GPIO` `UART` `LPIT` `Keypad` `TextLCD`

<!-- Repository: https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY -->

---

## 🎓 Education & Experience

- **경북대학교 IT대학 전자공학부**
  - Embedded System, Automatic Control, Digital System Design
  - Microprocessor, Circuit Theory, Electronics

- **SSAFY 15기**
  - Python Algorithm
  - Django / Django REST Framework
  - Vue 3 / Vite / Pinia
  - Team-based Web Project

- **WENS 기업 연계 프로젝트**
  - ROS2 기반 공장 안전사고 감지 UGV 개발

- **Future Mobility 자율주행 교육**
  - ROS2 및 F1TENTH 기반 충돌 방지 시스템 개발

- **Smart Mobility Track**
  - 자동차 시스템 및 부품
  - 전기차, 하이브리드, 자율주행 기술
  - 자동차 개발 프로세스

---

## ⚡ Leadership & Activities

- SoC 기반 실시간 색칠 게임 프로젝트 **팀장**
  - 개발 일정 관리 및 역할 분담
  - HW/SW 통합 문제 해결
  - 팀원 간 개발 인터페이스 조율

- 중앙 봉사동아리 **한울회 집행부**
  - 청소년 활동 진행 및 인솔
  - 교내 봉사활동 기획 및 운영

- 경제동아리 **ACE 기획국장 및 부회장**
  - 동아리 행사 기획
  - 구성원 간 협업 및 일정 관리

---

## 🧩 My Development Approach

```text
문제 발생
   ↓
로그 및 데이터 수집
   ↓
HW / SW / 통신 계층 분리
   ↓
원인 가설 수립
   ↓
파라미터 수정 및 반복 테스트
   ↓
수치와 결과를 통한 개선 검증
