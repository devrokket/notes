# **study-notes**
> 배움 노트

## AI를 즐겨라! 래블업 개발자 컨퍼런스 "lab | up > /conf/2" (2022.12.01)

> 발표 순서
  1. Beyond AI(신정규)
  - 현재 AI 소프트웨어와 하드웨어 쪽의 발전 현황.
  - Backend.AI에 대해 알 수 있었음.
  2. 로우레벨 리눅스는 처음이: 파이썬 개발자의 심연 탐방기 (조규진)
  - 백엔드 쪽은 접해본 적이 없어서 처음 듣는 내용이 많았음.
  - 리눅스 컨테이너 중 Docker를 사용함. (https://www.redhat.com/ko/topics/containers/what-is-docker) Red Hat 설명
  - strace처럼 처음 들어보는 디버거
  3. 비동기가 없는 것처럼 작동하는 리액트 컴포넌트 (이종은)
  - 동기 vs 비동기
  - 과거 프론트엔드는 멈춰 있는 스냅샷을 만드는 개념(동기)이었다면 현재는 동적인 프로그래밍(비동기) 비중이 늘어남.
  - React의 component가 비동기를 만들 때 How가 아닌 What에 집중할 수 있게 해줌.
  4. Google ML Developer Programs 소개 (권순선)
  - conference에 엄청난 노력.
  - 구글 ML(머신러닝) 관련 사업 : ML가이드(https://developers.google.com/machine-learning/guides/rules-of-ml) , Google ML Bootcamp (https://rsvp.withgoogle.com/events/google-machine-learning-bootcamp_84589b) ,
    부트캠프 참여 후기(https://developers.googleblog.com/2022/03/GoogleMachineLearningBootcamp.html)
  - TesorFlow KR (https://www.facebook.com/groups/TensorFlowKR/) 커뮤니티 소개
  - ML 공부해보고 싶다는 생각이 들었음.
  5. FastAPI 고군분투기-Forklift (권강민)
  - FastAPI (https://fastapi.tiangolo.com/ko/) 새로 출시된 파이썬 웹 프레임워크, 플라스크와 비교해서 편리함 설명. 공식문서가 잘 쓰여있음.
  6. NVDIA Omniverse for Generating Virtual Worlds
  - https://www.nvidia.com/en-us/omniverse/
  7. 머신러닝을 씁니다 (박해선)
  8. 오픈소스로 전생:PR 하나 날렸을 뿐인데 (강시온, 이상훈)
  - first-contributionhttps://github.com/firstcontributions/first-contributions
  9. 비동기 작업의 가시성 향상을 통한 프로덕션 이슈 디버그 하기 (김준기)
  - 비동기 작업의 가시성 향상을 통한 프로덕션 이슈 디버그하기, 김준기님(레블업 CTO)
  - asyncio 디버깅
  - aiomonitor라는 모니터에서 자동으로 디버깅이 돌아갈 수 있도록 함.
  - https://pypi.org/project/aiomonitor/
  - Open Source Software 컨트리뷰션 아카데 (https://www.oss.kr/contribution_academy)
<<<<<<< HEAD



## MySQL & JDBC

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.sql.Statement;
import java.util.Scanner;

public class JDBC_Example {

   static final String DB_URL = "jdbc:mysql://localhost/playlist_schema?useUnicode=true&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone= UTC";
   static final String USER = "root";
   static final String PASS = "dusdjrndl00!";
   static final String QUERY = "SELECT song_id, title, release_date, singer, genre FROM song";

   public static void main(String[] args) {
      // Open a connection

      try(Connection conn = DriverManager.getConnection(DB_URL, USER, PASS);
         Statement stmt = conn.createStatement();
         ResultSet rs = stmt.executeQuery(QUERY);
      ) {		      
         while(rs.next()){
            //Display values    	 
            System.out.print("song_id: " + rs.getInt("song_id"));
            System.out.print(", title: " + rs.getString("title"));
            System.out.print(", release_date: " + rs.getDate("release_date"));
            System.out.println(", singer: " + rs.getString("singer"));
            System.out.println(", genre: " + rs.getString("genre"));



         }

	Scanner sc = new Scanner(System.in);
	int option;

	System.out.println("<<옵션을 선택하시오>>");
 	System.out.println("1.Check your playlist");
 	System.out.println("2.Listen to songs by genre");
 	System.out.println("3.Terminate program...");
 	option = sc.nextInt();
 	System.out.println(option);



 	if(option == 1) {
 		System.out.println("You choose option 1");
 	}
 	else if(option == 2)
 		System.out.println("You choose option 2");
 		// genre 별 출
 	else if(option == 3)
 		System.out.println("You choose option 3");
 		// 프로그램 종
 	else
 		System.out.println("Enter again...");
 		//3번 입력 전까지 반복으로 돌려야 함.

      } catch (SQLException e) { //에러 발생 시 작
         e.printStackTrace();
      }
   }
}
=======
>>>>>>> 5adc03da56cedd0f4e8bacb2e0d91b2524017e4a
