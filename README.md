# 1. Git

### 1-1. Git 시작
    (1) git init  // 파일에 git 적용
    (2) git config --global user.name "이름"  
    (3) git config --global user.email "메일주소"  

### 1-2. 스테이징
    git add -A  // 스테이징 영역에 추가   
    
    git status  // 상태 확인
    
### 1-3. 커밋
    git commit -m "설명"  // 커밋, 커밋 메세지 작성 필수
    
    git log  // 로그 확인


# 2. GitHub

### 2-1. Git Push (로컬 파일 업로드)
    (1) git init
    (2) git remote add origin "github repository 주소"  // origin이라는 이름으로 remote(원격 repository) 연결
    (3) 스테이징, 커밋
    (4) git push -u origin master  // origin: remote명, master: 브랜치명
    
    git remote  // 연결된 remote 확인

### 2-2. Git Clone (원격 파일 다운로드)
    git clone "github repository 주소"
    
### 2-3. Git Pull, Fetch (원격 파일 다운로드, remote 연결되어 있을 때)
    git pull  // local과 병합
    git fetch  // log 확인 후 직접 병합(merge) 


# 3. Git Branch
    Branch란 Git의 포인터 개념
    쉽게 말하면 작업 영역, Branch를 생성해두면 해당 작업 시점으로 자유롭게 이동 가능

### 3-1. Branch 생성
    git checkout -b 브랜치명  // 브랜치 생성 후 이동  
    
    git branch 브랜치명  // 브랜치 생성
    git checkout 브랜치명   // 브랜치 이동

    
## 4. VSCode에서 GUI로 Github 사용하기
    remote 연결된 상태에서 Branch와 Pull/Push 사용법

### 4-1. Branch 생성 및 이동
<img width="200px" src="https://user-images.githubusercontent.com/50562634/158763631-f338f63d-c0d5-4160-ac0c-95e161008894.png"/> <img width="500px" src="https://user-images.githubusercontent.com/50562634/158763867-8993bb51-2063-4f35-afb3-cd08e8a39ed6.png"/>

    VSCode 좌측 하단 클릭하여 Branch 생성, 현재 Branch명 확인 가능
    
### 4-2. Pull
<img width="700px" src="https://user-images.githubusercontent.com/50562634/158764489-42cfba21-fec8-4ce0-b0e6-52c00b314cd3.png"/>

    이미지 상황) local branch yejin에 origin(원격 repository) main 가져오기
    
### 4-3. Push
<img width="700px" src="https://user-images.githubusercontent.com/50562634/158764979-e65b4d67-d5e7-4e89-bf64-99f5b8754a58.png"/>

    add, commit(커밋 메시지 작성 필수), push 순으로 클릭 시 원격 repository에 업로드(github에서 확인 가능)
