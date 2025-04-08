# ROS2-Tutrial
Tutorial and exercising for ROS2 and its simulation


**이 페이지는 Ubuntu 22.04 LTS 버전 기준으로 작성되었으며, ROS2 Humble 개발 환경을 구성하는 것을 설명하는 wiki 입니다.**

[ROS2 Humble 설치 가이드](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html)

ROS2 필수 패키지 설치
---
``` shell
sudo apt update && sudo apt install -y \
  build-essential \
  cmake \
  git \
  libbullet-dev \
  python3-colcon-common-extensions \
  python3-flake8 \
  python3-pip \
  python3-pytest-cov \
  python3-rosdep \
  python3-setuptools \
  python3-vcstool \
  wget
```
``` shell
python3 -m pip install -U \
  argcomplete \
  flake8-blind-except \
  flake8-builtins \
  flake8-class-newline \
  flake8-comprehensions \
  flake8-deprecated \
  flake8-docstrings \
  flake8-import-order \
  flake8-quotes \
  pytest-repeat \
  pytest-rerunfailures \
  pytest
```
``` shell
sudo apt install --no-install-recommends -y \
    libasio-dev \
    libtinyxml2-dev \
    libcunit1-dev
```
Recommended [Visual Studio Code](https://code.visualstudio.com/) Extensions
---
- C/C++
- CMake
- CMake Tools
- Python
- ROS
- URDF
- Colcon Tasks
- XML Tools
- YAML
- Markdown All in One

VSCode development environment settings
---
`settings.json` 파일은 VSCode의 사용자별 글로벌 환경설정을 지정하는 파일. 이 파일에 기술된 설정들은 모든 workspace에서 적용됨. 
```
~/.config/Code/User/settings.json
```
```
{
    "cmake.configureOnOpen": false,
    "editor.minimap.enabled": false,
    "editor.mouseWheelZoom": true,
    "editor.renderControlCharacters": true,
    "editor.rulers": [100],
    "editor.tabSize": 2,
    "files.associations": {
        "*.repos": "yaml",
        "*.world": "xml",
        "*.xacro": "xml"
    },
    "ros.distro": "humble",
    "colcon.provideTasks": true,
    "files.insertFinalNewline": true,
    "files.trimTrailingWhitespace": true,
    "terminal.integrated.scrollback": 1000000,
    "workbench.iconTheme": "vscode-icons",
    "workbench.editor.pinnedTabSizing": "compact"
}
``` 
