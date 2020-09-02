# 주소

## [bit.ly/edu_Br](https://bit.ly/edu_Br)

# 파일 다운로드 방법

#### 1) 전체 파일 다운로드 
우측 상단의 초록색 버튼인 [code] 버튼을 누르면 됩니다.

#### 2) 특정 파일 다운로드
해당 파일을 클릭해서 들어간 후 흰색 [download] 버튼을 누르면 됩니다.

# Brightics 윈도우 2004버전 긴급 패치
[긴급패치]윈도 10, 버전 2004. Brightics Studio 에러발생시 해결 가이드

* 본 패치는 수업진행이 안되는 분들을 위한 패치이므로, 수업용도로만 사용 부탁드립니다. 
정식 패치는 테스트 완료 후, 공유될 예정입니다. 
 
SVD, ANOVA 관련 윈도 10, 버전 2004상에서 numpy 관련 버그 패치입니다.  
 
Brightics Python Process 중지 
전체 서비스를 Stop 하거나, Stop Python Process 버튼을 눌러서 비활성화 시킵니다. 
 
관련 패키지 다운로드 받기 
아래 5개 패키지를 다운로드 받습니다. 
 
https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/numpy-1.18.5+mkl-cp36-cp36m-win_amd64.whl
https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/scipy-1.5.2-cp36-cp36m-win_amd64.whl
https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/numexpr-2.7.2-cp36-cp36m-win_amd64.whl
https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/patsy-0.5.1-py2.py3-none-any.whl
https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/statsmodels-0.12.0-cp36-cp36m-win_amd64.whl
 
패치 방법
 
윈도키+R => cmd => 엔터 
 
탐색기 여시고 brightics-studio 설치된 곳 이동해서 하위 lib => python 으로 이동  한뒤, 경로를 ctrl + c 로 카피 합니다.
 
cmd창에서  
cd  오른쪽 마우스 버튼 클릭해서 붙여넣기 => 엔터 
python.exe get-pip.py   입력 하신후 엔터 
cd Scripts  입력 하신후 엔터
 
위에 받은 파일을 탐색기  brightics-studio\lib\python\Scripts 로 복사 또는 이동 시켜주세요.
 
pip install numpy-1.18.5+mkl-cp36-cp36m-win_amd64.whl </br>
pip install scipy-1.5.2-cp36-cp36m-win_amd64.whl </br>
pip install numexpr-2.7.2-cp36-cp36m-win_amd64.whl </br>
pip install patsy-0.5.1-py2.py3-none-any.whl </br>
pip install statsmodels-0.12.0-cp36-cp36m-win_amd64.whl </br>
 
이후 다시 Brightics Studio 를 실행해서 모델 실행을 하면 됩니다. 

위의 내용들이 잘 진행이 안되거나 문의사항 있는 경우 brightics.cs@samsung.com 계정으로 다시 메일 부탁 드립니다.
