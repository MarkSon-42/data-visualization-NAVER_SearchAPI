# Data Visualization Project

## 프로젝트 소개

네이버 Datalab API를 활용하여 키워드 검색어 추이를 시각화하는 웹 애플리케이션
사용자가 입력한 키워드 그룹에 대한 검색 트렌드를 차트로 표현하여 데이터를 쉽게 이해할 수 있도록 
데이터 시각화를 제공하는 서비스

## 주요 기능

- 사용자 정의 키워드 그룹 입력
- 검색 기간 및 시간 단위 설정
- 네이버 Datalab API를 통한 검색어 트렌드 데이터 수집
- 수집된 데이터의 차트 시각화
- 실시간 차트 업데이트

## 기술 스택

### Frontend
- Vue.js 3
- Chart.js / vue-chartjs
- Axios

### Backend
- Node.js
- Express

### API
- 네이버 Datalab API

## 설치 및 실행 방법

1. 저장소 클론
   ```
   git clone https://github.com/MarkSon-42/data-visualization-NAVER_SearchAPI.git
   ```

2. 백엔드 설정
   ```
   cd server
   npm install
   ```
   `.env` 파일을 생성하고 네이버 API 키 설정:
   ```
   CLIENT_ID=your_naver_client_id
   CLIENT_SECRET=your_naver_client_secret
   ```

3. 프론트엔드 설정
   ```
   cd ../client
   npm install
   ```

4. 백엔드 실행
   ```
   cd ../server
   node index.js
   ```

5. 프론트엔드 실행
   ```
   cd ../client
   npm run dev
   ```

6. 브라우저에서 `http://localhost:5173` 접속

## 사용 방법

1. 시작일과 종료일 선택
2. 시간 단위 선택 (일간, 주간, 월간)
3. 키워드 그룹 이름 입력 후 '추가' 버튼 클릭
4. 키워드 입력 후 '추가' 버튼 클릭 (여러 개 추가 가능)
5. '그룹 확정' 버튼 클릭
6. 필요한 만큼 그룹과 키워드 추가
7. '제출' 버튼 클릭하여 차트 생성 및 업데이트

