# **study-notes**
> 배움 노트

## AI를 즐겨라! 래블업 개발자 컨퍼런스 "lab | up > /conf/2" (2022.12.01)

> 발표 순서
  1. Beyond AI(신정규)
    * 현재 AI 소프트웨어와 하드웨어 쪽의 발전 현황.
    * Backend.AI에 대해 알 수 있었음.
  2. 로우레벨 리눅스는 처음이: 파이썬 개발자의 심연 탐방기 (조규진)
    * 백엔드 쪽은 접해본 적이 없어서 처음 듣는 내용이 많았음.
    * 리눅스 컨테이너 중 Docker를 사용함. (https://www.redhat.com/ko/topics/containers/what-is-docker) Red Hat 설명
    * strace처럼 처음 들어보는 디버거
  3. 비동기가 없는 것처럼 작동하는 리액트 컴포넌트 (이종은)
    * 동기 vs 비동기
    * 과거 프론트엔드는 멈춰 있는 스냅샷을 만드는 개념(동기)이었다면 현재는 동적인 프로그래밍(비동기) 비중이 늘어남.
    * React의 component가 비동기를 만들 때 How가 아닌 What에 집중할 수 있게 해줌.
  4. Google ML Developer Programs 소개 (권순선)
    * conference에 엄청난 노력.
    * 구글 ML(머신러닝) 관련 사업 : ML가이드(https://developers.google.com/machine-learning/guides/rules-of-ml) , Google ML Bootcamp (https://rsvp.withgoogle.com/events/google-machine-learning-bootcamp_84589b) ,
    부트캠프 참여 후기(https://developers.googleblog.com/2022/03/GoogleMachineLearningBootcamp.html)
    * TesorFlow KR (https://www.facebook.com/groups/TensorFlowKR/) 커뮤니티 소개
    * ML 공부해보고 싶다는 생각이 들었음.
  5. FastAPI 고군분투기-Forklift (권강민)
    * 
  6. NVDIA Omniverse for Generating Virtual Worlds
  7. 머신러닝을 씁니다 (박해선)
  8. 오픈소스로 전생:PR 하나 날렸을 뿐인데 (강시온, 이상훈)
  9. 비동기 작업의 가시성 향상을 통한 프로덕션 이슈 디버그 하기 (김준기)


> 3. 비동기가 없는 것처럼 작동하는 리액트 컴포넌트 (이종은)
> > 동기 & 비동기

오픈소스, 인턴 강시온님
주제 찾기
1. 사용하는 프로그램 혹은 라이브러리에서 찾아보기
2. 스스로 불편한점 찾아보기
3. 큰 프로젝트에서 시작하지 말기

""""
Good first issue

Github 파헤치기
(issue, review, actions, security)
""""

## Github 업적 시스템
발표자 devrank라는 오픈소스 랭킹 서비스 만드는중
@Yaminyam

##

* <오픈소스 탐험기> 레블업 백엔드개발, 이상훈<

오픈소스 컨트리뷰션아카데미
Backend.AI 멘티, 영어 문서 번역, python type hint 작성 등 작은 프로젝트부터 진행
그 다음해에 멘토로 참여
Kurbernetes: 오픈소스 컨테이너

내년에 파이콘 스피커로 참가하고 싶어짐.

* 비동기 작업의 가시성 향상을 통한 프로덕션 이슈 디버그하기, 김준기님(레블업 CTO)
asyncio 디버
aiomonitor라는 모니터에서 자동으로 디버깅이 돌아갈 수 있도록 함.
https://pypi.org/project/aiomonitor/
