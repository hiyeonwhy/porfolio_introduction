<div align="center">

# Hi 👋, I'm Hiyeon Woo

### Embedded Systems · Robotics · Autonomous Driving

하드웨어와 소프트웨어의 경계를 이해하고,
실제 환경에서 안정적으로 동작하는 시스템을 만드는 개발자입니다.

`Embedded` `FPGA` `ROS` `Computer Vision` `System Verification`

</div>

---

## 🌱 About Me

* 경북대학교 **전자공학부**에서 임베디드 시스템, 제어, 디지털 시스템을 공부했습니다.
* ARM Processor, FPGA, MCU부터 ROS 기반 자율주행까지 경험했습니다.
* 단순히 기능을 구현하는 것에 그치지 않고, **로그와 데이터를 기반으로 오류의 원인을 추적하고 개선하는 과정**을 중요하게 생각합니다.
* 실험, 실차 테스트, RMSE 분석과 rosbag 비교를 통해 시스템의 안정성과 성능을 검증해 왔습니다.
* 임베디드 시스템과 로보틱스를 기반으로 시스템 검증 및 신뢰성 개선 분야에 관심이 있습니다.

---

## 🔭 Interests

* **Embedded Systems**

  * ARM MCU, Peripheral Control, Device Driver
  * Real-time System, Hardware Interface

* **HW/SW Co-design**

  * Zynq SoC, ARM Processor, FPGA
  * AXI4-Lite, Custom IP, Memory-mapped I/O

* **Robotics & Autonomous Driving**

  * ROS1 / ROS2, SLAM, Navigation
  * AMCL, Costmap, Sensor Fusion, Collision Avoidance

* **Computer Vision**

  * ArUco Marker Detection, Pose Estimation
  * Camera Calibration, LiDAR–Camera Calibration

* **System Verification**

  * Log-based Debugging
  * RMSE Analysis, Repeated Testing, Parameter Tuning

---

## 🛠 Tech Stack

### Languages

`C` `C++` `Python` `Verilog HDL`

### Embedded Systems & SoC

`Zynq-7000` `ARM Cortex-A9` `ARM Cortex-M4F` `S32K144`
`AXI4-Lite` `Memory-mapped I/O` `BRAM` `Bare-metal`
`GPIO` `UART` `External Interrupt` `LPIT Timer` `FATFS`

### Robotics & Autonomous Systems

`ROS1 Noetic` `ROS2 Humble` `SLAM` `slam_toolbox`
`Navigation Stack` `Nav2` `AMCL` `Costmap`
`robot_localization` `EKF` `ros2_control` `TF / TF2`
`Odometry` `LiDAR` `IMU`

### Computer Vision & Calibration

`OpenCV` `ArUco` `cv_bridge` `image_transport`
`Camera Calibration` `Pose Estimation` `solvePnP`
`LiDAR–Camera Calibration` `PCL`

### Verification & Analysis

`rosbag` `rosbag2` `RMSE Analysis`
`Log-based Debugging` `Repeated Testing` `Parameter Tuning`
`RViz` `RViz2` `rqt`

### Web Development

`Django` `Django REST Framework` `Vue 3`
`Vite` `Pinia` `REST API` `Django ORM`

### Development Environment

`Linux` `Git` `GitHub` `CMake` `catkin` `colcon`
`Vivado` `Xilinx SDK` `S32 Design Studio` `Gazebo`

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

* **기간:** 2025.05 ~ 2025.06
* **역할:** 팀장 및 HW/SW 통합 개발
* Zynq-7000의 PS와 PL을 **AXI4-Lite Custom Peripheral**로 연동했습니다.
* 도형 판별, 색칠 상태 관리, 완료 검출과 화면 출력 연산을 FPGA의 Custom IP로 구현했습니다.
* TFT-LCD, TextLCD, 7-Segment, UART, SD Card를 하나의 시스템으로 통합했습니다.
* BRAM과 FATFS를 활용하여 RGB565 이미지를 TFT-LCD에 출력했습니다.
* 사용자 로그인, 게임 선택, 제한 시간 및 점수 관리 기능을 ARM 기반 소프트웨어로 구현했습니다.
* 메모리 주소 충돌, XDC 핀 중복, I/O 배치 오류 등의 HW/SW 통합 문제를 해결했습니다.

**Tech Stack**

`Zynq-7000` `ARM Cortex-A9` `FPGA` `Verilog HDL`
`C` `AXI4-Lite` `BRAM` `Memory-mapped I/O`
`UART` `FATFS` `Vivado` `Xilinx SDK`

**Repository:** [hiyeonwhy/zync_draw_game](https://github.com/hiyeonwhy/zync_draw_game)

---

### 2. 공장 내 안전사고 감지 UGV

> ROS2 기반 UGV가 공장 내부를 자율주행하며 위험 상황을 감지하는 안전 순찰 시스템

* **형태:** WENS 기업 연계 팀 프로젝트
* **역할:** UGV 자율주행 및 위치 추정 성능 개선
* `slam_toolbox`를 활용하여 공장 내부의 2D 점유 격자 지도를 생성했습니다.
* Nav2와 AMCL을 기반으로 목표 지점까지 이동하는 자율주행 시스템을 구성했습니다.
* Wheel Odometry와 IMU 데이터를 EKF로 융합하여 `/odom/filtered`를 생성했습니다.
* 주행 속도가 증가할 때 발생하는 Odometry Drift와 SLAM 지도 오차를 분석했습니다.
* ROS2 Bag으로 주행 데이터를 기록하고 센서 융합 적용 전후의 위치 추정 결과를 비교했습니다.
* Nav2, Costmap 및 EKF 파라미터를 조정하며 반복 주행 테스트를 수행했습니다.

**Tech Stack**

`ROS2 Humble` `C++` `Python` `slam_toolbox`
`Nav2` `AMCL` `Costmap` `robot_localization` `EKF`
`ros2_control` `TF2` `rosbag2` `LiDAR` `IMU` `RViz2`

**Repository:** [hiyeonwhy/ros2-ugv-factory-safety](https://github.com/hiyeonwhy/ros2-ugv-factory-safety)

---

### 3. TurtleBot 미로 자율주행 및 ArUco 정밀 도킹

> 좁은 미로를 자율주행한 뒤 ArUco 마커를 기반으로 목표 지점에 정밀 도킹하는 시스템

* ROS1 기반 SLAM, AMCL 및 Navigation Stack을 구성했습니다.
* 좁은 통로에서 발생하는 경로 생성 실패와 벽 충돌 문제를 분석했습니다.
* 로봇의 실제 크기에 맞게 `footprint`, `inflation_radius`, `cost_scaling_factor` 등의 Costmap 파라미터를 조정했습니다.
* ArUco 마커의 위치와 자세를 추정하여 로봇의 방향과 접근 거리를 제어했습니다.
* `INITIAL_FORWARD → AUTO_MODE → STRAIGHT-ONLY MODE` 상태 머신으로 도킹 과정을 구현했습니다.
* 마커가 보이지 않는 근거리에서는 Odometry 기반 직진 제어로 전환했습니다.
* 카메라 내부 파라미터와 LiDAR–카메라 외부 파라미터를 직접 캘리브레이션했습니다.

**Tech Stack**

`ROS1 Noetic` `C++` `Python` `Navigation Stack`
`SLAM` `AMCL` `Costmap` `Odometry` `TF`
`OpenCV` `ArUco` `cv_bridge` `solvePnP`
`LiDAR` `PCL` `Camera Calibration`

**Repository:** [hiyeonwhy/turtlebot-maze-docking](https://github.com/hiyeonwhy/turtlebot-maze-docking)

---

### 4. S32K144 암호 입력 장치

> ARM Cortex-M4F MCU의 주변장치와 인터럽트를 통합한 베어메탈 임베디드 시스템

* S32K144의 SDK 드라이버 대신 레지스터를 직접 제어하는 방식으로 구현했습니다.
* GPIO 외부 인터럽트를 활용하여 다중 스위치 조합 인증 기능을 구현했습니다.
* 난수를 생성해 Character LCD에 표시하고, 정해진 위치의 숫자를 조합해 암호를 생성했습니다.
* LPIT Timer 인터럽트로 4×3 Matrix Keypad를 주기적으로 스캔했습니다.
* 입력한 최근 네 자리를 4-digit 7-Segment에 동적으로 표시했습니다.
* 입력값이 암호와 일치하면 LCD와 RGB LED를 통해 결과를 출력하도록 구현했습니다.
* GPIO, Timer, Keypad, LCD, 7-Segment, RGB LED와 부저를 하나의 상태 기반 시스템으로 통합했습니다.

**Tech Stack**

`S32K144` `ARM Cortex-M4F` `C` `Bare-metal`
`GPIO` `External Interrupt` `LPIT Timer`
`Matrix Keypad` `7-Segment` `Character LCD` `RGB LED`

**Repository:** [hiyeonwhy/s32k144-cipher-lock](https://github.com/hiyeonwhy/s32k144-cipher-lock)

---

## 🎓 Education & Experience

* **경북대학교 IT대학 전자공학부**

  * Embedded System, Automatic Control, Digital System Design
  * Microprocessor, Circuit Theory, Electronics

* **SSAFY 15기**

  * Python Algorithm
  * Django / Django REST Framework
  * Vue 3 / Vite / Pinia
  * Team-based Web Project

* **WENS 기업 연계 프로젝트**

  * ROS2 기반 공장 안전 순찰 UGV 개발
  * 자율주행 및 위치 추정 성능 개선 담당

* **미래모빌리티 자율주행 운영 실습 프로그램**

  * ROS2 및 F1TENTH 기반 충돌 방지 시스템 개발

* **스마트 모빌리티 트랙**

  * 자동차 시스템 및 부품
  * 전기차, 하이브리드 및 자율주행 기술
  * 자동차 개발 프로세스

---

## ⚡ Leadership & Activities

* **SoC 기반 실시간 색칠 게임 프로젝트 팀장**

  * 개발 일정 관리 및 역할 분담
  * HW/SW 통합 문제 해결
  * 팀원 간 개발 인터페이스 조율

* **중앙 봉사동아리 한울회 집행부**

  * 청소년 활동 진행 및 인솔
  * 교내 봉사활동 기획 및 운영

* **경제동아리 ACE 기획국장 및 부회장**

  * 동아리 행사 기획
  * 구성원 간 협업 및 일정 관리

---

