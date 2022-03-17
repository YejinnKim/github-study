## 1. Git

### 1-1. Git 시작
    (1) git init  
    (2) git config --global user.name "이름"  
    (3) git config --global user.email "메일주소"  

### 1-2. 커밋
    git status  // 상태 확인(커밋 할 파일이 있는지)  
    
    (1) git add -A  // 스테이징 영역에 추가   
    (2) git commit -m "설명"  // 커밋, 설명 필수


## 2. GitHub

### 2-1. Local 파일 업로드
    (1) git remote add origin "github repository 주소"    
    (2) git push -u origin master
    
    git remote   // 원격 Ropository 이름 확인, origin  

### 2-2. Github 파일 다운로드
    git clone "github repository 주소"  // cd ./repository명 (폴더 안으로 들어가야 함)   
    

## 3. Branch로 작업하기
    Branch란 Git의 포인터 개념
    쉽게 말하면 작업 영역, Branch를 생성해두면 해당 작업 시점으로 자유롭게 이동 가능

### 3-1. Branch 생성
    git checkout -b 브랜치명  // 브랜치 생성 후 이동  
    
    git branch 브랜치명  // 브랜치 생성
    git checkout 브랜치명   // 브랜치 이동

### 3-2. Local Branch와 Github Branch 연결
    (1) git pull origin 브랜치명   // 원격 Repository 가져오기
    (2) 작업~~
    (3) git add -A   
    (4) git commit -m "설명"   
    (5) git push -u origin 브랜치명   // -u 옵션으로 local과 원격 연결, 이후 git push 만 입력해도 가능
    
    pull 대신 fetch도 가능
    pull : local과 바로 병합, fetch : log 확인 후 병합(merge)해야 함
    
    
## 4. VSCode에서 GUI로 Github 사용하기
    clone까지 완료 된 상황에서 Branch와 Pull/Push 사용법

### 4-1. Branch 생성 및 이동
<img width="200px" src="https://user-images.githubusercontent.com/50562634/158763631-f338f63d-c0d5-4160-ac0c-95e161008894.png"/> <img width="500px" src="https://user-images.githubusercontent.com/50562634/158763867-8993bb51-2063-4f35-afb3-cd08e8a39ed6.png"/>

    VSCode 좌측 하단 클릭하여 Branch 생성, 현재 Branch명 확인 가능
    
### 4-2. Pull
<img width="700px" src="https://user-images.githubusercontent.com/50562634/158764489-42cfba21-fec8-4ce0-b0e6-52c00b314cd3.png"/>

    이미지 상황) local branch yejin에 origin(원격 repository) main 가져오기
    
### 4-3. Push
<img width="700px" src="https://user-images.githubusercontent.com/50562634/158764979-e65b4d67-d5e7-4e89-bf64-99f5b8754a58.png"/>

    add, commit(커밋 메시지 작성 필수), push 순으로 클릭 시, 원격 repository에 저장
    github 페이지에서 확인 가능
