# 구조
/(root)
    >> requirements.txt : 특정 환경에서 사용한 모듈들을 기술
                          환경이 구출될 때, 이 서비스 운영/개발시 사용, 필요한 모듈 설치를 위해 기술되는 파일 
                          - 반드시 버전 명시 >> 향후에 서버가 변경되도, 문제없이 구동될 수 있도록 동일한 환경 제공
    >> run.py : 서비스 메인
    >> wsgi.py : 엔트리 포인트, 아파치 서버가 바라보는 파일
    >> deploy.json : 페브릭이 배포 작업을 하는 데 필요한 상수값들을 저장한 파일 
                     - 환경 변수가 저장된 파일 



# fabric 설치 
- pip install fabric / conda install fabric >> X
    >> python2.7.xx 버전에 맞게 설치 된다
    >> python3.x 버전 사용 불가 

- pip install fabric3 / conda install fabric3 

# github 사용 
1. github.com >> create repository 
2. local pc에서 git 명령어 이용하여 적절한 위치에 저장소 다운 
    - 저장소에서 카피 
        - $ git clone https://github.com/ok0749/deploy.git
    - 이미 작성된 내용을 카피해서 만들어진 폴더 deploy안으로 붙여놓는다.
