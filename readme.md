# ML DL

### jupyter  notbook install

#### 1. python 설치

[파이썬 주피터 노트북 설치 (jupyter notebook)](https://zidarn87.tistory.com/314)

#### 2. Jupyter 노트북 설치

```
D:\code\MLDL>python3 --version
Python 3.11.

D:\code\MLDL>pip3 install jupyter6
```

#### 3. 실행

```
D:\code\MLDL>python -m notbook
```

#### 4. library

```
pip install scikit-learn
pip install matplotlib 
pip install jupyterlab
```

[conda and pip 그리고 아나콘다 가상환경 셋팅](https://jenny-jo55.tistory.com/60)

```
C:\Users\jhyunlee>nvidia-smi
Sun Nov  5 00:24:45 2023
+---------------------------------------------------------------------------------------+
| NVIDIA-SMI 536.23                 Driver Version: 536.23       CUDA Version: 12.2     |
|-----------------------------------------+----------------------+----------------------+
| GPU  Name                     TCC/WDDM  | Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp   Perf          Pwr:Usage/Cap |         Memory-Usage | GPU-Util  Compute M. |
|                                         |                      |               MIG M. |
|=========================================+======================+======================|
|   0  NVIDIA GeForce GTX 1060 3GB  WDDM  | 00000000:23:00.0 Off |                  N/A |
| 25%   34C    P8               5W / 120W |   1306MiB /  3072MiB |      3%      Default |
|                                         |                      |                  N/A |
+-----------------------------------------+----------------------+----------------------+

+---------------------------------------------------------------------------------------+
| Processes:                                                                            |
|  GPU   GI   CI        PID   Type   Process name                            GPU Memory |
|        ID   ID                                                             Usage      |
|=======================================================================================|
|    0   N/A  N/A      6316    C+G   ...e Stream\83.0.2.0\GoogleDriveFS.exe    N/A      |
|    0   N/A  N/A      8136    C+G   ...5n1h2txyewy\ShellExperienceHost.exe    N/A      |
|    0   N/A  N/A      9256    C+G   ...CBS_cw5n1h2txyewy\TextInputHost.exe    N/A      |
|    0   N/A  N/A     10076    C+G   ...81.0_x64__8wekyb3d8bbwe\GameBar.exe    N/A      |
|    0   N/A  N/A     17400    C+G   C:\Windows\explorer.exe                   N/A      |
|    0   N/A  N/A     17928    C+G   ....Search_cw5n1h2txyewy\SearchApp.exe    N/A      |
|    0   N/A  N/A     18276    C+G   ...les\Microsoft OneDrive\OneDrive.exe    N/A      |
|    0   N/A  N/A     22276    C+G   ...1.0_x64__8wekyb3d8bbwe\Video.UI.exe    N/A      |
|    0   N/A  N/A     22992    C+G   ...2txyewy\StartMenuExperienceHost.exe    N/A      |
|    0   N/A  N/A     23604    C+G   ...oogle\Chrome\Application\chrome.exe    N/A      |
|    0   N/A  N/A     24772    C+G   C:\Program Files\MarkText\MarkText.exe    N/A      |
|    0   N/A  N/A     29172    C+G   ...crosoft\Edge\Application\msedge.exe    N/A      |
|    0   N/A  N/A     31740    C+G   ....Search_cw5n1h2txyewy\SearchApp.exe    N/A      |
|    0   N/A  N/A     33220    C+G   ...Programs\Microsoft VS Code\Code.exe    N/A      |
+---------------------------------------------------------------------------------------+
```

https://jenny-jo55.tistory.com/60


```
conda create -n env_name python tensorflow numpy scipy=0.15.0​
conda activate env_name​
conda install notebook matplotlib pandas seaborn -y

```
#### 6.  Framework 
설치하려는  Framework(TF or Pytorch) 가 cuda 버전 어떤 것과 맞는 지 확인한다.

아나콘다 가상환경을 만들어준 후에 그 안에서 설치한다.
pip로 tensorflow 깔면 cuda, cdnn을 일일이 버전 찾아서 깔아줘야 하는 수고가 필요하나... 킹갓 conda로 깔면 그런거 필요 없이 알아서 깔아준다.(참고)
TF :  공홈 > 설치> 소스에서 빌드> 각자에게 맞는 OS > CUDA 버전에 맞는 TF 버전과 파이썬 버전 체크 
Pytorch : 공홈 > Get Started > Start Locally >  친절하게 각자 사양에 맞춰서 이미 표시된 셋팅으로 나온 명령어 복붙)

