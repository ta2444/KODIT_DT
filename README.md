## 2023년도 신용보증기금 DT 데이터분석 기본과정 - 데이터 시각화

### 1. 실습 환경
1) 파이썬 버전 : 3.9.13 (Windows, 64bit)
2) 사용 IDE : Jupyter Notebook (7.0.6)
3) 사용 패키지 :
    __________
    * pip       (22.0.4)
    * pandas    (2.1.4)
    * numpy     (1.26.2)
    * matplolib (3.8.2)
    * seaborn   (0.13.0)

### 2. Jupyter Notebook 완전 삭제 방법

1) cmd에 아래 명령어 입력
  
pip uninstall -y jupyter jupyter_core jupyter-client jupyter-console jupyterlab_pygments qtconsole notebook nbconvert nbformat nbclassic nbclient jupyterlab-widgets jupyter-events jupyter-server jupyter-server-terminals jupyter_server_fileid jupyter_server_ydoc jupyter-ydoc jupyterlab jupyterlab_server  
    
* jupyter 관련 모든 패키지를 삭제하는 명령어

2) %USERPROFILE%\AppData\Roaming\jupyter  

* 경로의 모든 폴더 및 파일을 제거

### 3. (참고) 주피터노트북 테마 설정 관련

1) 주피터 노트북 내 Terminal 실행 후 아래 패키지 수동 설치
    * pip install jupyterthemes

2) 추천 테마 설정 : 아래 명령어 주피터 노트북 내 Terminal에 입력
    * jt -t onedork -fs 115 -nfs 125 -tfs 115 -dfs 115 -ofs 115 -cursc r -cellw 80% -lineh 115 -altmd -kl -T -N

3) 다른 테마 및 옵션 키워드 참고 https://realblack0.github.io/2020/05/13/jupyter-notebook-themes.html

4) 폰트 변경 방법 주피터노트북 config 파일 집합 생성 
    * cmd에 아래 명령어 입력
        * jupyter notebook --generate-config 
        * cmd에 출력되는 생성 경로 확인
    * 해당 폴더 아래, custom 폴더의 custom.css 파일 수정
        * font-family : 뒤의 모든 폰트를 변경
    * 참고로, 코딩할 땐  D2coding Ligature 폰트가 가장 좋음

5) 테마 원복 명령어
    * jt -r