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
 
*SVD, ANOVA 관련 윈도 10, 버전 2004상에서 numpy 관련 버그 패치입니다.*
- 참고이슈: https://github.com/numpy/numpy/issues/16744

## Brightics Python Process 중지 
전체 서비스를 Stop 하거나, Stop Python Process 버튼을 눌러서 비활성화 한다.

## 관련 패키지 다운로드 받기 
아래 5개 패키지 다운로드 한다.

- https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/numpy-1.18.5+mkl-cp36-cp36m-win_amd64.whl
- https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/scipy-1.5.2-cp36-cp36m-win_amd64.whl
- https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/numexpr-2.7.2-cp36-cp36m-win_amd64.whl
- https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/patsy-0.5.1-py2.py3-none-any.whl
- https://download.lfd.uci.edu/pythonlibs/w3jqiv8s/statsmodels-0.12.0-cp36-cp36m-win_amd64.whl

- https://pypi.lcsb.uni.lu/packages/dc/18/e69ef84530360c2d39db51acb4cc0012990f27fb1fa7542dac45ad30e7ab/numpy-1.18.5-cp36-cp36m-win_amd64.whl#sha256=b03b2c0badeb606d1232e5f78852c102c0a7989d3a534b3129e7856a52f3d161
- https://pypi.lcsb.uni.lu/packages/fc/f6/3d455f8b376a0faf1081dbba38bbd594c074292bdec08feaac589f53bc06/scipy-1.5.2-cp36-cp36m-win_amd64.whl#sha256=8e28e74b97fc8d6aa0454989db3b5d36fc27e69cef39a7ee5eaf8174ca1123cb
- https://pypi.lcsb.uni.lu/packages/6c/6b/44a9ddee4cdb260be71a2900b8a961897c13620bad6f4770b47dd7b32bf1/numexpr-2.7.1-cp36-none-win_amd64.whl#sha256=57d9ccd0820b7f5b1bed5100dd54a5ae52c39eb5b7e54317ae29e31ed9bd9edf
- https://pypi.lcsb.uni.lu/packages/ea/0c/5f61f1a3d4385d6bf83b83ea495068857ff8dfb89e74824c6e9eb63286d8/patsy-0.5.1-py2.py3-none-any.whl#sha256=5465be1c0e670c3a965355ec09e9a502bf2c4cbe4875e8528b0221190a8a5d40
- https://pypi.lcsb.uni.lu/packages/d8/f5/b2aaa505b2e8f43668c0a067dd9ebf83032648f451b1bad7f769c4a1c085/statsmodels-0.12.0rc0-cp36-none-win_amd64.whl#sha256=3b8f64699864e0fcb459e210a88ccabf7523fc8ac8a6f8a197db753e4bd11b69

## 패치 방법

### 1. 윈도 CMD 창 열기
- 윈도키+R  
- cmd 입력후 엔터 

### 2. python 폴더로 이동
- cd c:\본인의폴더\brightics-studio\lib\python

### 3. pip 설치
- python.exe get-pip.py

### 4. Scripts 폴더로 이동
- cd Scripts

### 5. 아래 명령어로 python 라이브러리를 설치한다.
*아래 파일 위치는 다운로드 받은 위치로 변경이 필요하다.*

*또는 c:\본인의폴더\brightics-studio\lib\python\Scripts 로 파일을 복사 또는 이동시킨다.*

- pip install numpy-1.18.5+mkl-cp36-cp36m-win_amd64.whl
- pip install scipy-1.5.2-cp36-cp36m-win_amd64.whl
- pip install numexpr-2.7.2-cp36-cp36m-win_amd64.whl
- pip install patsy-0.5.1-py2.py3-none-any.whl
- pip install statsmodels-0.12.0-cp36-cp36m-win_amd64.whl

이후 다시 Brightics Studio 를 실행해서 모델 실행을 하면 됩니다. 

위의 내용들이 잘 진행이 안되거나 문의사항 있는 경우 brightics.cs@samsung.com 계정으로 다시 메일 부탁 드립니다.
