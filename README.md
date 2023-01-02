### 2022 - AIFFEL Dataton Project 
## 🎬 [Netflix Data Analysis] Netflix 데이터셋과 Netflix의 연도별 행보를 활용하여 데이터 시각화, EDA 수행
#### Netflix의 연도별 실적, 투자 내용을 바탕으로 연관성 분석
![image](https://user-images.githubusercontent.com/108614874/208298254-4d423910-f700-48c3-bc76-2684c7cceaa6.png)

### 1. Intro
[넷플릭스 데이터셋](https://www.kaggle.com/datasets/shivamb/netflix-shows)과 [IMDB 별점 데이터셋](https://www.kaggle.com/datasets/ruchi798/tv-shows-on-netflix-prime-video-hulu-and-disney)을 이용
* 데이터를 시간 순서로 정렬하고, 넷플릭스의 행보를 따라가면서 그에 따른 영화/프로그램 장르의 변화, 영상 수 등을 분석하는 것이 목표입니다.
### 2. Project

* **Netflix Dataset**  
전 세계에서 가장 인기있는 스트리밍 플랫폼 Netflix의 영화와 TV 프로그램들의 정보를 담고 있는 데이터셋입니다!   
8000편 이상의 영화 또는 TV 프로그램의 정보를 담고 있습니다.   
이 데이터 세트는 출연진, 감독, 등급, 출시 연도, 기간 등과 같은 세부 정보와 함께 Netflix에서 사용할 수 있는 모든 영화 및 TV 프로그램 목록으로 구성됩니다.   
  - show_id  s1-s8807
  - type Movie, Tv Show
  - title
  - director
  - cast
  - country
  - date_added
  - release_year 출시연도
  - rating 관람등급
  - duration : 시간, Season
  - listed in
  - description
  - rating  

* **시각화 시 통일감을 주기 위해 [컬러믹서](https://htmlcolors.com/color-mixer) 사이트를 활용**
![image](https://user-images.githubusercontent.com/108614874/208299938-4110455b-e26a-496a-8310-262e35a4229e.png)

* **타입별(TV show / Movie)로 별점 평균내어 시각화에 활용**

![image](https://user-images.githubusercontent.com/108614874/208299995-e194f921-8ddd-45db-b3ea-597663aab74e.png)

* **장르 수 TOP15**

![image](https://user-images.githubusercontent.com/108614874/208300051-d973b685-4491-41b3-9549-b6e87d87002a.png)

* **연도별 추가된 컨텐츠 수**  

![image](https://user-images.githubusercontent.com/108614874/208300160-d40ef8d5-5c58-4ba1-bca9-136bcf934a8e.png)  
plotly 시각화 라이브러리를 사용, interactive visualization

* **국가별 넷플릭스 컨텐츠 추가 분포 확인**  

![image](https://user-images.githubusercontent.com/108614874/208300283-aad16cb8-4c56-45c1-90e6-7f7e22bbe1cf.png)  
plotly 시각화 라이브러리의 choropleth 사용, country와 지도의 위치가 매핑되어 직관적으로 확인가능

* **연도별, 월별 추가된 장르의 분포 확인**  

![image](https://user-images.githubusercontent.com/108614874/208300357-de5722c9-e2d7-4f05-9d46-83f534244b9a.png)  
altair 라이브러리 사용.

* **연도별 평점 분포 확인**

![image](https://user-images.githubusercontent.com/108614874/208300460-21da7dfa-0afd-4a16-89b0-a23584f4bf81.png)  
색상 면적이 밀도인 kdeplot을 사용, 파란색, 주황색, 초록색 면적이 큰 편인데, 각각 6점 7점 8점이므로 해당 평점의 작품 비중이 많은 것을 알 수 있습니다.  
그리고 2020년 총 밀도가 가장 많아진 것을 볼 수 있는데, 앞서 19년과 20년에 추가된 컨텐츠 수가 많았던 영향이라고 생각됩니다.

### 3. 팀원 소개
**Visual_flix** : Netflix를 Visualize 해보이겠다는 뜻의 팀명

모예송 🙆‍♀️  
팀장이지만 가장 팀원같은 모예송입니다.  
넷플릭스 데이터분석을 통해 지금까지 배웠던 것들을 복습해보고 새로운 지식도 알아가는 시간이 되었으면 좋겠습니다.  
Visual_Flix팀 쵝오👍🏻

이주미 👩‍💻  
넷플릭스구독 어언 5년차... 이주미입니다.  
가장 좋아하는 데이터셋을 맡게돼서 기대가 되네요.  
궁극의 시각화 가보자고!! ✨

심성보 🕵️‍♂️  
안녕하세요! 평소에 넷플릭스를 즐겨보던 한 사람입니다.  
넷플릭스 데이터를 이번 데이터톤 주제로 선정하여 분석하게 되어서 설렘 반 걱정 반입니다.  
재밌는 데이터 분석 결과를 보여드릴 수 있도록 최선을 다해보겠습니다!
