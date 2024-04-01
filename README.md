# 인지편향 평가 사이트
MBTI 와 유사한 인지편향 평가 사이트  
디자인/퍼블리싱을 제외한 1인개발  
사이트 링크 : [DQ체크](https://www.dqcheck.net/)  

## 아키텍처
![아키텍처](https://github.com/khj923265/dqcheck--description/assets/68458092/bbe225e1-00b1-4ee3-8e59-1a1b89576762)
* S3 웹 호스팅을 이용한 CSR 방식을 사용
* EC2 서버와 통신해 질문지, 결과 API 구현 & 결제 데이터 저장

## 기능 구현
* 질문지, 결과 API 개발
* 아임포트, 페이팔을 이용한 결제 구현
* 25개 언어 변환 기능 구현(i18n 라이브러리를 사용해 json 패키지를 나눠 개발)
* 바, 게이지 차트 시각화
* 결제 후 유효시간(7일) 시각화 & 결제 복구 구현

## 기술스택
* BackEnd : Springboot, Java17, JPA
* FrontEnd : React, TypeScript
* Infra : AWS (EC2, S3, CloudFront, Route53, RDS(MariaDB))
