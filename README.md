## 2023년도 신용보증기금 DT 데이터분석 기본과정 - 데이터 시각화
* * * 
### 1. 실습 환경
1) 파이썬 버전 : 3.9.13 (Windows, 64bit)
2) 사용 IDE : Jupyter Notebook (7.0.6)
3) 사용 패키지 : </br>

    |순번|패키지명|버전|비고|
    |:---:|---|---|:---:|
    |1|pip|22.0.4|패키지 설치 및 버전관리|
    |2|pandas|2.1.4|구조화된 데이터 분석용|
    |3|numpy|1.26.2|데이터의 수리적 연산 등|
    |4|scipy|1.11.4|데이터 통계분석 등|
    |5|matplotlib|3.8.2|데이터 시각화 기본구조|
    |6|seaborn|0.13.0|데이터 고수준 시각화|
</br></br>
- - -
### 2. Git 다운로드 명령어

* Git은 협업 및 형상관리를 위한 프로그램으로, 여러 환경에서 한 프로젝트를 진행해야 할 경우 Github이라고 하는 클라우드에 작업 상황을 백업하고, 복원할 수 있음
   
* 이러한 버전은 branch라고 하는 단위로 관리되기 때문에, 프로젝트 수정이 필요한 경우 특정 branch에 접근해 롤백이 가능함

* 이번 연수에 필요한 데이터와 소스코드는 외부메일을 통해 배포드렸지만, 나중에 데이터를 다시 다운받고 싶은 경우나 Git에 관심이 생긴 분들은 아래 Git Bash 명령어를 통해
실습 환경을 복원할 수 있음
  
```python
    git init
    git add remote origin https://github.com/ta2444/KODIT_DT.git
    git branch -M main
    git pull origin main
```

</br></br>
- - -
### 3. Jupyter Notebook 완전 삭제 방법 (에러 발생시)

**1) cmd에 아래 명령어 입력**
  
```python
pip uninstall -y jupyter jupyter_core jupyter-client jupyter-console jupyterlab_pygments qtconsole notebook nbconvert nbformat nbclassic nbclient jupyterlab-widgets jupyter-events jupyter-server jupyter-server-terminals jupyter_server_fileid jupyter_server_ydoc jupyter-ydoc jupyterlab jupyterlab_server
```
    
* 👆 jupyter 관련 모든 패키지를 삭제하는 명령어 </br></br>
  
**2) 아래 경로의 모든 폴더 및 파일을 제거**

%USERPROFILE%\AppData\Roaming\jupyter

</br></br>
- - -
### 4. (참고) 주피터노트북 테마 설정 관련 (notebook 7.x.x. 이후 버전 사용 불가)

**1) 주피터 노트북 내 Terminal 실행 후 아래 패키지 수동 설치**

```python
pip install jupyterthemes
```

**2) 추천 테마 설정 : 아래 명령어 주피터 노트북 내 Terminal에 입력**
```python
jt -t onedork
```

**3) 다른 테마 및 옵션 키워드 참고**
```HTML
https://realblack0.github.io/2020/05/13/jupyter-notebook-themes.html
```

**4) 폰트 변경 방법 주피터노트북 config 파일 집합 생성**
</br>
    * cmd에 아래 명령어 입력
    </br>
```python
jupyter notebook --generate-config
```
</br>
    * cmd에 출력되는 생성 경로 확인
    </br></br>
    * 해당 폴더 아래, custom 폴더의 custom.css 파일 수정
        * font-family : 뒤의 모든 폰트를 변경
    </br></br>
    * 참고로, 코딩할 땐  D2coding Ligature 폰트가 가장 좋음

**5) 테마 원복 명령어**
</br>
```python
jt -r
```
