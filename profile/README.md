# AESLAB
홈페이지 : https://shseo6.wixsite.com/aesl  

## 내용 변경
- 변경해야 할 사항이 있을 시 발견한 사람이 수정하기

## 사용 규칙
- 개인적으로 작업하는 것은 fork후 자신의 이름을 딴 폴더를 만들고 작업 하는 것을 권장(git 충돌 방지를 위함)
- 공동 파일을 수정해야할 때도 fork후 내용 수정 후  PR을 요청하도록 함(git 충돌 방지를 위함)
- Commit 메세지 잘 만들기 그래야 다른 사람이 뭘 추가했는지 알 수 있다.
- 규칙을 만들 시 해당하는 규칙이 필요한 이유에 대해 간략하게나마 글로 남기기(이후에 규칙을 수정할 지에 대한 평가가 지속적으로 이루어질 수 있도록)
---
1. Fork 사용 안할 시 (나는 commit 실수 안할 자신 있다.)
   1. 바탕화면 혹은 AESLAB에 git 용 폴더 생성
   2. 폴더 우클릭하여 Git bash 클릭 
   3. 이제 AESLAB을 사용해 보자
      1. 처음 AESLAB 사용 경우git clone 하여 AESLAB 데이터 다운 **(중요)clone 할 경우 git init 하지말자!**
            ````bash
            $git clone https://github.com/21-Arbiter/AESLAB.git
            ````
      
      2. AESLAB clone이 다 완성 되고 그 다음 부터 사용할 경우는 commit 기록은 확인해보고 commit 된 경우가 있는 경우 
            ````bash
            $git remote add origin https://github.com/21-Arbiter/AESLAB.git
            $git pull origin master
            ````

     
   4. 작업 폴더 안에 AESLAB 생성됨 그 폴더 안으로 이동 
        ````bash
        $cd AESLAB
        ````
   5. 작업 진행 
   6. 작업이 완료 
        ````bash
        $git status #git 변경 사항 제대로 적용 됐는지 확인
        $git add .
        $git commit -m "커밋 메세지"
        $git push origin master 
        #참 쉽다
        ````
2. Fork 사용 경우 (주로 오픈 소스 Contribute 할때 사용한다. 내가 AESLAB master 조질꺼 같다 그럴때 사용)
   1. AESLAB Fork 부터 사용하여 내 계정에 원격 저장소 추가
   2. 이후 AESLAB 작업용 폴더 생성
   3. 생성된 폴더 우클릭
   4. 이후 그 폴더 클론하자 
        ````bash
        $git clone https://github.com/너의계정/AESLAB.git
        ````
   5. 작업 진행
   6. 작업 완료
        ````bash
        $git status #git 변경 사항 제대로 적용 됐는지 확인
        $git add .
        $git commit -m "커밋 메세지"
        $git push origin master 
        
        ````  
    1. 이러면 너의 Fork된 원격 저장소에만 저장될 것이다. 하지만 우리는 AESLAB의 Master에 저장해야한다 그러므로 Pull Request를 요청하자 (Compare & prequest 클릭)   
    ![image](https://user-images.githubusercontent.com/86957779/179984146-acb61ad9-cb5c-4821-af6e-f1be7112d03f.png)

    2. Pull Request 했다 요청해달라 하면 Master에 너가 한 내용 반영됨
    3. 참 쉽다.
   * 만약 MASTER의 업데이트 된 내용을 너의 Fork 된 원격 저장소에 업데이트 하고 싶을 경우
    ````bash
    $git remote add upstream https://github.com/21-Arbiter/AESLAB.git
    $git pull upstream master
    $git push origin master
    #이러면 너의 원격 저장소에도 저장 될 것이다.
    ````
---
## 유의사항 및 참고
- Readme 파일은 마크다운 언어로 일반 txt 파일과는 다르므로 문서 작성 시 해당 문법을 조금 공부할 필요가 있음

    [마크다운 문법정리 사이트](https://gist.github.com/ihoneymon/652be052a0727ad59601)
