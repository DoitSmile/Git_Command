# Git_Command

# git 깔고 초기 한번만 설정
git config --global user.name "Your Name" : 전역 유저 이름설정
git config --global user.email you@example.com: 전역 이메일 설정


# 새로운 프로젝트 만들고 반복 
1. git init : 저장소 만들기
2. git add . (전체파일추가)/ git add <폴더/파일경로> (선택파일추가): 현재 상태 추가
3. git status : 현재 상태 확인 ( 새로 생긴 파일이 있으면 new파일 머시기 뜸)
4. git commit -a -m "입력할메세지": 현재 상태 저장 (-a add와 commit을 동시에)
5. git remote add origin URL주소 : url주소를 origin 변수에저장
6. git branch <새로 생성할 브런치이름> : 브런치 생성
7. git branch -M <변경할 브런치>: branch(저장할 저장소 지점) 변경
8. git branch : 현재 브런치 확인 
9. git push -u origin <브런치> : 저장소로 푸쉬
(오류가나면 -u는 강제푸쉬 or +브런치이름 ex) git push origin +main )

# 진행중인 프로젝트에 업데이트만 필요시 
git remote -v : 현재 원격 업로드 주소 확인
git status로 생성/수정된 파일을 알아냄 
git add로 생성/수정된 파일추가 
git commit -a -m "입력할메세지" 으로 저장 
git push origin <브런치> 을 반복적으로 사용하여 버전 관리를 해주면된다.

# 프로젝트 가져오기 
git pull : 원격저장소에 있는 프로젝트의 변경사항을 그대로 로컬저장소에 옮겨와 자동으로 병합
git clone :  원격저장소의 내용을 새로운 폴더에 그대로 복사



* error: origin 리모트가 이미 있습니다. 오류시
git remote rm origin
