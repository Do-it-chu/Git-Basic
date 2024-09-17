## BE
- S3를 통한 이미지 저장소 구현

<img width="708" alt="image" src="https://user-images.githubusercontent.com/103571758/186388733-475a1802-f3d6-420a-a5b3-6bda76425458.png"><img width="787" alt="image" src="https://user-images.githubusercontent.com/103571758/186388923-954abfb9-aa83-428c-b901-7b37f24568f7.png">
post형식으로 image를 업로드시 s3저장소에 이미지가 올라가는 것 까지 확인

[현재 문제점]
> 이미지 파일의 크기가 클 경우 또는 확장자에 따라 500 server error가 발생 됨 
<img width="852" alt="image" src="https://user-images.githubusercontent.com/103571758/186389879-2c3c3390-f0d0-4502-8a99-b9da79ec8ce6.png">

<img width="747" alt="image" src="https://user-images.githubusercontent.com/103571758/186387915-021e7548-8ec7-4d55-a653-d1eb1f724338.png">
해당 오류는 EC2 환경이 아닌 곳에서 AWS 리소스를 사용하게 됨으로써 endpoint를 찾지 못하는 에러 발생 

- EC2를 통한 MySQL 통합 DB 환경 구현
<img width="1159" alt="image" src="https://user-images.githubusercontent.com/103571758/186390372-5de5a9e5-0c07-4bb9-8003-5b63278f7674.png">
DB환경을 만들 ec2 인스턴스에 고정IP를 할당


<img width="557" alt="image" src="https://user-images.githubusercontent.com/103571758/186392062-3dbdabe4-e5fd-4c07-9715-0da2a97358bb.png">
root 계정으로 wil계정 생성 및 모든 권한 부여

<img width="553" alt="image" src="https://user-images.githubusercontent.com/103571758/186392765-069302c6-9693-4396-9e22-ea96a0f0c1f0.png">
wil 계정으로 MySQL 재접속 및 DB접근

<img width="582" alt="image" src="https://user-images.githubusercontent.com/103571758/186393109-115f8453-dab2-4dbf-a822-114369ee070a.png">
Backend DB 설정 

<img width="189" alt="image" src="https://user-images.githubusercontent.com/103571758/186393378-e7202052-e7b5-4b0d-a91c-a34bb8885825.png">
BE Model Entity 구현 부분에 대해 서버 실행시 쿼리 수행되며 EC2에 구현한 DB에 테이블 생성까지 확인
