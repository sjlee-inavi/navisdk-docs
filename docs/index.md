## 개정이력

___

\[ 0.0.1 \] 2020-01-17

-   인증 업데이트 추가
    

___

\[ 0.0.2 \] 2020-01-29

-   SDK 적용방법 추가
    

___

\[ 0.0.3 \] 2020-02-20

-   setDrivingStatusListener I/F
    
    -   nearGoalDist Param. 추가
        

___

\[ 0.0.4 \] 2020-03-23

-   주행중 특정지점에서 비정상 종료되는 이슈 수정
    

___

\[ 0.0.5 \] 2020-03-30

-   Proguard 옵션추가
    

___

\[ 0.0.6 \] 2020-04-01

-   SDK 난독화 예외처리 추가 ( 통신관련 )
    
-   App 난독화 가이드 추가
    

___

\[ 0.0.7 \] 2020-04-07

-   길 찾기 I/F 파라미터 변경 ( runRoute, runSingleRoute )
    
    -   RouteExtraInfo 추가
        
    -   RoutePtItem 에 angle필드 추가
        

___

\[ 0.0.8 \] 2020-04-23

-   과속 백그라운드 알림 추가
    

___

\[ 0.0.9 \] 2020-05-20

-   차량 속도 Callback 추가 ( setCarSpeedListener )
    

___

\[ 0.0.10 \] 2020-05-28

-   디버그 로그 제거
    
-   주행화면 TBT UI 개선 ( 차기/차차기 높이 및 간격 조정 )
    

___

\[ 0.0.11 \] 2020-06-08

-   내부안정성 이슈 개선
    
-   NaviLocation 에 속도 필드 추가
    

___

\[ 0.0.12 \] 2020-07-30

-   주행화면 GUI 개선 ( 회전정보, 카메라정보, 현위치 버튼 등 )
    
-   길 찾기 실패 코드 추가 ( 코드표 : 5002, 5003, 5004 )
    

___

\[ 0.0.13 \] 2020-11-02

-   기본 자차 아이콘 및 폰트 변경
    
-   주행화면 TBT UI 개선 ( 형태 및 컬러 변경 )
    
-   주행화면 TBT 출발/도착 아이콘 변경 I/F 추가 ( setTurnViewTaxiIcon )
    
-   지도 컴포넌트 Show/Hide I/F 수정 ( forceHideMapComponent )
    
-   도로명 주소 I/F 추가 ( getFullAddr )
    
-   현재 도로명 I/F 추가 ( getCurrentRoadName )
    
-   경유지 정보 I/F 추가 ( getRoutePtViaInfo )
    
-   주행정보 요금 필드 추가 ( getRemainRouteInfo )
    
    -   RouteRemainInfo에 remainFee 필드 추가
        
-   NaviEvent Callback 추가 ( setNaviEventListener )
    
    -   현위치 이동, 전체경로 보기
        

___

\[ 0.0.14 \] 2020-11-05

-   주행 속도 레이아웃 오류 개선
    

___

\[ 0.0.15 \] 2020-11-25

-   Audio Stream Type 변경 I/F 추가 ( setAudioStreamType )
    

___

\[ 0.0.16 \] 2020-12-04

-   지도 Style 변경 I/F 추가 ( setMapStyle )
    
-   도착예정시간 초기화 및 갱신 타이밍 개선
    

___

\[ 0.0.17 \] 2020-12-16

-   총 주행정보 I/F 추가 ( getTotalRemainRouteInfo )
    
-   getRemainRouteInfo의 Distance 갱신 로직 개선
    
-   forceHideMapComponent 지도 컴포넌트 타입 추가
    
    -   MAPCOMPONENT.ROUTE\_TRAFFIC\_STATUS\_BAR
        

___

\[ 0.0.18 \] 2021-02-05

-   Layout 초기화 I/F 추가 ( initLayout )
    
-   기존 initLayout I/F 에, 지도/주행의 부모 뷰 추가
    

___

\[ 0.0.19 \] 2021-02-09

-   SurfaceView Activity Casting 오류 개선
    

___

\[ 0.0.20 \] 2021-03-03

-   **SDK 저장소 변경 \[ 필수 적용 항목 \]**
    
    -   Bintray 에서 Artifactory 로 변경
        
-   **NaviLocation 자료형 변형 \[ 필수 적용 항목 \]**
    
    -   angle 필드 자료형 Double 로 변경
        
-   화면회전 세팅 I/F 수정 ( setOrientation )
    
    -   ORIENTATION\_UNDEFINED 추가
        

___

\[ 0.0.21 \] 2021-03-17

-   내부적으로 사용하던 TimeZone 제거
    

___

\[ 0.0.22 \] 2021-04-21

-   **minSdkVersion 19에서 21로 변경 \[ 필수 적용 항목 \]**
    
-   경유지 기능 추가
    
    -   기존 길찾기 I/F 에 경유지 Param 추가
        
        -   runRoute, runSingleRoute
            
    -   남은 경유지 정보 I/F 추가
        
        -   getRoutePtRemainViaInfo
            
        -   getRemainViaRouteInfo
            
    -   경유지 변경 재탐색 I/F 추가
        
        -   runReRouteChangeVia
            
-   에뮬레이터 지원
    
    -   에뮬레이터 모드 I/F 추가 (setEmulatorMode)
        

___

\[ 0.0.23 \] 2021-08-06

-   안내종료거리 튜닝
    
-   길찾기 I/F에 탐색옵션 Param 추가
    
    -   runRoute
        
-   안전운행정보 변경 기능 추가
    
    -   안내설정 I/F 추가 (setGuidanceSettings, getGuidanceSettings)
        
    -   GUIDANCESETTING 추가
        

___

\[ 0.0.24 \] 2021-11-29

-   안내종료거리 2차 튜닝
    
-   내부 모듈 안정성 개선
    
-   주행 경로선 색상 변경 기능 추가
    
    -   경로선 색상 변경 I/F 추가 ( setMapRouteColor )
        
    -   MAPROUTECOLOR 추가
        

___

\[ 0.0.25 \] 2021-12-22

-   내부 모듈 안정성 개선
    
-   주행중 전체 경로보기 기능 추가
    
    -   전체 경로보기 I/F 추가 ( drivingRouteZoomMap )
        

___

\[0.0.26\] 2022-03-31

-   목적지 도착시 요금 반환 기능 추가
    
    -   목적지 도착시 요금 반환 I/F 추가
        
        -   onArrivalFee ( OnDrivingStatusListener )
            
    -   setDrivingStatusListener 설명 추가
        
        -   onArrivalFee 사양 설명 추가
            

___

\[0.0.27\] 2022-11-11

-   경유지 사양 확대 (최대 100개까지 설정 가능)
    
-   forceHideMapComponent 지도 컴포넌트 타입 추가
    
    -   MAPCOMPONENT.BOTTOM\_NORMAL\_SIDE\_BUTTON
        
    -   MAPCOMPONENT.BOTTOM\_DRIVING\_SIDE\_BUTTON
        
    -   MAPCOMPONENT.BOTTOM\_ARRIVAL\_LEFT\_BUTTON
        
-   화물차 설정 및 전용 탐색 옵션 추가
    
    -   차량 높이/중량/U-turn 도로폭/좁은길 도로폭/통행제한구간 회피 설정 옵션 추가
        
        -   setCarHeight , getCarHeight
            
        -   setCarWeight , getCarWeight
            
        -   setAvoidUturn , getAvoidUturn
            
        -   setAvoidNarrowRoad , getAvoidNarrowRoad
            
        -   setAvoidRestriction , getAvoidRestriction
            
    -   화물차 전용 탐색 옵션 추가
        
        -   **ROUTEOPTIONTYPE 수정**
            

___

\[0.0.28\] 2023-01-10

-   지도 여백(Padding) 설정 I/F 추가
    
    -   routeZoomMapWithPadding
        
    -   setMapPadding
        
    -   clearMapPadding
        
-   차종 설정 I/F 추가
    
    -   setCarType, getCarType
        
-   enum class CARTYPE 추가
    

___

\[0.0.29\] 2023-01-20

-   경유지 도착 알림 I/F 추가
    
    -   \*\*OnDrivingStatusListener 수정 (\*\*onArrivalVia 추가) **\[필수 적용 항목\]**
        
-   TBT(TurnView) Custom Background Color 설정 I/F 추가
    
    -   setTurnViewBackgroundColor , getTurnViewBackgroundColor (차기 TurnView)
        
    -   setNextTurnViewBackgroundColor, getNextTurnViewBackgroundColor (차차기)
        
    -   setArrivalViewBackgroundColor , getArrivalViewBackgroundColor (목적지 도착 view)
        
    -   resetTurnViewsBackgroundColor (기본값으로 초기화)
        
-   확대도 표출 기능 및 표출 여부 I/F 추가
    
    -   setVisibleExtendView , getVisibleExtendView
        

___

\[0.5.0\] 2023-03-22

-   내부 모듈 안정성 개선
    

___

\[0.5.1\] 2023-05-04

-   경유지 도착 알림 I/F 사양 변경
    
-   탐색열 에서 진행방향으로 현 위치에서 가장 가까운 좌표 인덱스 반환 I/F 추가
    
    -   getNearestVertexIndex
        

___

\[0.5.2\] 2023-05-15

-   내부 모듈 안정성 개선
    

___

\[0.6.0\] 2023-08-31

-   내부 엔진 수정
    
-   AndroidX 적용
    
    -   playground-service-location 버전 16.0.0 → 21.0.1 로 수정 (fusedLocationProvider 관련 내용 적용)
        

___

\[0.6.1\] 2023-09-05

-   경로탐색 실패 처리 사양 변경
    
    -   경유지가 포함된 경우 출발지-목적지 간 거리 체크 하지 않도록 변경
        

___

\[ 0.6.2\] 2023-10-17

-   **SDK 저장소 URL 변경 (필수 적용)**
    
-   화물차 전용옵션 로직 개선
    

___

\[ 0.6.3\] 2024-04-03

-   안정성 개선
    

___

\[ 0.6.4\] 2024-04-17

-   구글 정책 위반 관련 이슈 개선
    

___

\[ 0.7.0 \] 2024-04-25

-   kotlin version 업그레이드 (1.5.21)
    
-   가이드 문서 업데이트 (프로젝트 설정 관련 내용 추가)
    
    -   라이브러리 종속성 항목 추가 (recyclerview)
        
    -   jvmtarget 관련 내용 추가
        

___

\[ 0.7.1 \] 2024-09-26

-   내부 엔진 수정
    
-   상수원보호구역 회피탐색 기능 추가
    
-   최적탐색 기능 추가
    

___

\[ 0.7.2 \] 2024-10-23

-   안내 음성 수정
    
-   후면카메라 단속 안내 추가
    
-   안내 UI 폰트 변경
    

___

\[ 0.7.3 \] 2025-03-12

-   내부 엔진 수정
    
-   iMPS 내제화에 따른 인증 서버 전환
    

___

\[ 0.7.4 \] 2025-07-09

-   다음턴 , 다다음턴 (TBT View) 백그라운드 안내 기능 추가 (다른 앱 위에 그리기)
    
-   사용자가 설정 → 디스플레이 크기 옵션을 임의로 수정한 경우 안내 화면이 의도와 다르게 오히려 축소 되던 문제 수정
    

___

\[ 0.8.0 \] 2025-10-29

-   Android 15 대응 (support 16kb page size)
    
-   위수지역 회피탐색 기능 추가
    

___

\[ 0.8.1 \] 2025-11-13

-   아파트 동/호/명칭 충돌 기능 On/Off 기능 추가
    
    -   setAptPoiCollisionIgnored
        
-   지도 엔진 최신화
    

___

\[ 0.9.0 \] 2026-03-13

-   일부 단말에서 안내 음성 마지막이 잘리는 현상 수정
    
-   지도 Style 변경 I/F 제거
    
    -   setMapStyle, MAPSTYLE
        
-   Android Studio 최소지원 AGP 정책에 따라 AGP 7.4.2 적용
    
    -   AGP 4.1.0 미만의 경우 호환성 문제 발생 여지가 있으므로 AGP 7.x 계열로 맞추는것을 권장합니다.
        
-   지도 엔진 최신화
    

___

## 개요

-   본 문서는 Android 기반 플랫폼에서 구동되는 "**아이나비 내비게이션 SDK**"(이하 SDK) 연동에 대한 기술 문서 이다.
    

## Appkey 발급

SDK를 사용하기 위해서는 우선 Appkey 발급이 필요합니다. (규격서 제공 제휴 사업 담당자 통해 별도 요청 필요)

## 개발 환경

-   개발 도구 : AndroidStudio 2025.2.2 Patch 1 이상
    
-   개발 언어 : Android, Kotlin
    
-   SDK 지원 범위
    
    -   targetSdkVersion : 28 ( Android 9, P OS )
        
    -   minSdkVersion : 21 ( Android 5.0, LOLLIPOP OS )
        

## SDK 세팅 방법

1.  SDK 저장소 추가
    
    1.  Root Project build.gradle 파일
        
    
    
    
2.  SDK 의존성 추가
    
    1.  App build.gradle 파일
        
    
    
    
    b. gradle.properties 파일
    
    
    
3.  SDK 환경 세팅
    
    1.  App build.gradle 파일
        
        -   ndk abiFilters 추가
            
        
        
        
        -   컴파일 옵션 추가
            
        
        
        
    2.  AndroidManifest.xml
        
        -   http 허용
            
        
        
        
        -   Apache.http.legacy 허용
            
        
        
        
        -   AppKey 등록
            
        
        
        
4.  SDK 난독화 옵션 세팅
    
    1.  proguard-rules.pro
        
    
    
    
5.  SDK Layout 세팅
    
    1.  지도를 표출할 Layout(xml) 파일
        
        -   지도 View : "com.inaviair.sdkEngine.MapAdapter" 추가
            
        -   주행화면 View : "com.inaviair.sdkEngine.MapLayer" 추가
            
    
    
    

## SDK 권한 목록

App 에서 필수로 권한을 획득 해야 함

1.  SDK 를 사용하기 위한 필수 권한 목록
    
    
    
2.  SDK 내부에 선언되어 있는 Permission 목록
    
    
    

## SDK Interface

1.  SDK 생명주기
    
    -   SDK 생명주기는 Application 생명주기와 동일하게 사용하는것을 권장
        
    -   SDK 의 내비게이션 지도 및 주행화면은, 앱실행시 최초실행되는 Activity 에서 구현
        
        -   loadNaviLibrary, initLayout, initalizeNavi, destroyNavi 는 앱실행당 1회만 호출
            
2.  "**INaviController**" class 를 통하여 SDK 의 모든 기능 사용
    
    -   INaviController 는 Singleton 객체
        
    -   비동기 처리는 SDK 에서 Callback 제공
        
3.  좌표계
    
    -   SDK 는 위경도 좌표를 사용
        
    -   DD(십진수 도) 방식 사용
        
        -   ex> 서울역 위도 : 37.553173, 경도 : 126.972471
            

## 시나리오별 예시

1.  초기화
    
    -   Activity 예시
        
    
    
    
    -   Fragment 예시
        
    
    
    
2.  지도 아이콘 표출 및 제거
    
    
    
3.  검색
    
    
    
4.  길 찾기, 안내시작
    
    
    
5.  주행중 경유지 변경 재 탐색
    
    
    
6.  안전운행정보 안내 변경
    
    
    
7.  화물차 특화 옵션 적용
    
    
    
8.  차종 설정
    
    
    
9.  지도 여백 (Padding) 적용
    
    
    
10.  TurnView(차기,차차기, 목적지 도착 view) 배경색 변경
    



11.  확대도 표출
    
    
    
    확대도 표출 사양(가로모드)
    
    확대도 표출 사양(세로모드)
    
12.  현위치에서 진행방향으로 탐색열에서 가장 가까운 좌표 얻기
    
    
    
13.  백그라운드에서 TBT 표출하기
    
    
    
    
    

Background TBT 표출 예시

## 

INaviController Reference

1.  초기화
    
    1.  loadNaviLibrary
        
        
        
    2.  initLayout
        
        
        
    3.  initLayout
        
        
        
    4.  setMapStyle ( deprecated, v0.9.0 )
        
        
        
    5.  setAudioStreamType
        
        
        
    6.  setEmulatorMode
        
        
        
    7.  initalizeNavi
        
        
        
2.  지도 컨트롤
    
    1.  setMapClickListener
        
        
        
    2.  setCarCurrentPosition
        
        
        
    3.  setCarPosition
        
        
        
    4.  setMapPosition
        
        
        
    5.  zoomIn
        
        
        
    6.  zoomOut
        
        
        
    7.  setMapViewMode
        
        
        
    8.  getMapViewMode
        
        
        
    9.  visibleTrafficLine
        
        
        
    10.  createMapOverlay
        
        
        
    11.  createMapIcon
        
        
        
    12.  createMapIcon
        
        
        
    13.  addMapIcon
        
        
        
    14.  removeMapIcon
        
        
        
    15.  removeMapIconAll
        
        
        
    16.  routeZoomMap ( deprecated, 20/01/16 )
        
        
        
    17.  routeZoomMap
        
        
        
    18.  routeZoomMapWithPadding
        
        
        
    19.  setMapPadding
        
        
        
    20.  clearMapPadding
        
        
        
    21.  drivingRouteZoomMap
        
        
        
    22.  setMapLevel
        
        
        
    23.  setMapFontSizeType
        
        
        
    24.  getMapFontSizeType
        
        
        
    25.  setMapDayNightMode
        
        
        
    26.  getMapDayNightMode
        
        
        
    27.  setMapEnableRotate
        
        
        
    28.  setMapMoveChangedListener
        
        
        
    29.  forceHideMapComponent ( deprecated, 20/10/14 )
        
        
        
    30.  forceHideMapComponent
        
        
        
    31.  setTurnViewTaxiIcon
        
        
        
    32.  setMapRouteColor
        
        
        
    33.  setAptPoiCollisionIgnored
        
        
        
3.  검색
    
    1.  runSearch
        
        
        
    2.  runRecommendWord
        
        
        
    3.  getJibunAddr
        
        
        
    4.  getFullAddr
        
        
        
    5.  getCurrentRoadName
        
        
        
4.  길찾기
    
    1.  runRoute
        
        
        
    2.  runSingleRoute
        
        
        
    3.  runReRouteChangeVia
        
        
        
    4.  makeRouteSumInfo
        
        
        
    5.  getRoutePtInfo
        
        
        
    6.  getRoutePtViaInfo
        
        
        
    7.  getRoutePtRemainViaInfo
        
        
        
    8.  getRouteLinePoints
        
        
        
    9.  cancelRoute
        
        
        
    10.  onOptimalRoute
        
        
        
5.  주행
    
    1.  runGuidance
        
        
        
    2.  isSimulation
        
        
        
    3.  startSimulation
        
        
        
    4.  finishSimulation
        
        
        
    5.  getRemainRouteInfo
        
        
        
    6.  getRemainViaRouteInfo
        
        
        
    7.  getTotalRemainRouteInfo
        
        
        
    8.  setGuidanceSettings
        
        
        
    9.  getGuidanceSettings
        
        
        
6.  기타
    
    1.  destroyNavi
        
        
        
    2.  getNaviVersionName ( deprecated, 20/01/20 )
        
        
        
    3.  getNaviVersionCode ( deprecated, 20/01/20 )
        
        
        
    4.  getNaviSDKVersion
        
        
        
    5.  setApplicationStatus
        
        
        
    6.  setOrientation
        
        
        
    7.  setNaviVolume
        
        
        
    8.  getNaviVolume
        
        
        
    9.  getCurrentPos
        
        
        
    10.  setNaviEventListener
        
        
        
    11.  setRouteChangedListener
        
        
        
    12.  setDrivingStatusListener
        
        
        
    13.  setCarSpeedListener
        
        
        
    14.  setCarType
        
        
        
    15.  getCarType
        
        
        
    16.  setTurnViewBackgroundColor
        
        
        
    17.  getTurnViewBackgroundColor
        
        
        
    18.  setNextTurnViewBackgroundColor
        
        
        
    19.  getNextTurnViewBackgroundColor
        
        
        
    20.  setArrivalViewBackgroundColor
        
        
        
    21.  getArrivalViewBackgroundColor
        
        
        
    22.  resetTurnViewsBackgroundColor
        
        
        
    23.  setVisibleExtendView
        
        
        
    24.  getVisibleExtendView
        
        
        
    25.  setDrawBackgroundTBT
        
        
        
    26.  getDrawBackgroundTBT
        
        
        
    27.  forceHideBackgroundTBT
        
        
        
    28.  setBringToFrontListener
        
        
        
    29.  setLowResolution
        
        
        
7.  화물차 옵션
    
    1.  setCarHeight
        
        
        
    2.  getCarHeight
        
        
        
    3.  setCarWeight
        
        
        
    4.  getCarWeight
        
        
        
    5.  setAvoidUturn
        
        
        
    6.  getAvoidUturn
        
        
        
    7.  setAvoidNarrowRoad
        
        
        
    8.  getAvoidNarrowRoad
        
        
        
    9.  setAvoidRestriction
        
        
        
    10.  getAvoidRestriction
        
        
        
    11.  getNearestVertexIndex
        
        
        
    12.  getZoneLimit
        
        
        
    13.  setZoneLimit
        
        
        
    14.  getAvoidEvasion
        
        
        
    15.  setAvoidEvasion
        
        
        

## SDK Interface Reference

1.  OnNaviInitListener
    
    
    
2.  OnNaviEventListener
    
    
    
3.  OnMapClickListener
    
    
    
4.  OnMapMoveChangedListener
    
    
    
5.  OnSearchListener
    
    
    
6.  OnRecommendWordListener
    
    
    
7.  OnRouteMultiListener
    
    
    
8.  OnRouteSingleListener
    
    
    
9.  OnReRouteResultListener
    
    
    
10.  OnRouteChangedListener
    
    
    
11.  OnDrivingStatusListener
    
    
    
12.  OnCarSpeedListener
    
    
    
13.  OnBringToFrontListener
    
    
    

## SDK Structure Reference

1.  NaviLocation
    
    
    
2.  SearchResult
    
    
    
3.  SearchItem
    
    
    
4.  RecommendWord
    
    
    
5.  RoutePtItem
    
    
    
6.  RouteSumInfo
    
    
    
7.  NaviEvent
    
    
    
8.  RouteRemainInfo
    
    
    
9.  RouteViaRemainInfo
    
    
    
10.  RouteExtraInfo
    
    
    

## SDK Define Reference

1.  MAPVIEWMODE
    
    
    
2.  ICONGRAVITY
    
    
    
3.  MAPFONTSIZETYPE
    
    
    
4.  MAPDAYNIGHTMODE
    
    
    
5.  ROUTEPTTYPE
    
    
    
6.  APPSTATUS
    
    
    
7.  NAVIEVENTTYPE
    
    
    
8.  DRIVINGSTATUS
    
    
    
9.  ROUTEOPTIONTYPE
    
    
    
10.  MAPCOMPONENT
    
    
    
11.  MAPSTYLE ( deprecated, v0.9.0 )
    
    
    
12.  GUIDANCESETTING
    
    
    
13.  MAPROUTECOLOR
    
    
    
14.  CARTYPE
    
    
    

## 코드 표

|**코드 값**|**설명**|
|---|---|
|0|성공|
|1|길찾기 실패|
|3|목적지가 물리적 섬 도로|
|4|유효하지 않은 출발지|
|5|유효하지 않은 목적지|
|9|요청 파라미터 오류|
|11|메모리 할당 실패|
|15|파일 오픈 실패|
|17|메모리 할당 실패|
|19|파일 읽기 실패|
|20|파일 쓰기 실패|
|21|유효하지 않은 지도 데이터|
|22|요청 파라미터 오류|
|23|Projection 실패|
|25|DB 오류|
|32|길찾기 가능 거리 초과|
|35|두 지점이 너무 가까운 경우|
|36|목적지 오류|
|39|논리적 길찾기 오류|
|43|차량이 진입할 수 없는 도로|
|48|소켓 연결 실패|
|49|결과 생성 실패|
|96|잘못된 경로 ID|
|97|Checksum 오류|
|120|최적경로 ( 재 탐색은 성공했으나, 더 좋은 경로가 없는 경우 )|
|121|목적지 부근으로 재 탐색이 필요 없는 경우|
|300|미 지원 서비스|
|800|서버 파일 저장 에러|
|900|인증 실패|
|901|인증 정보가 변경되어 앱 재시작 필요|
|902|입력 파라미터 오류|
|903|조회결과 없음|
|904|존재하지 않는 파일 요청|
|905|DB 연동 에러|
|907|경로 ID 오류|
|931|유효하지 않은 좌표|
|933|유효하지 않은 검색어|
|1000|인증 데이터 오류|
|1001|인증 데이터 오류|
|1002|잘못된 요청 형식으로 인증|
|1003|인증 데이터가 존재하지 않음|
|1004|유효하지 않은 Unique Key ( 필수값인 Unique Key 값이 Null 이거나 Empty 인 경우 )|
|1005|유효하지 않은 Unique Key ( 필수값인 Unique Key 값이 20자 초과 인 경우 )|
|2000|처리되지 않은 예외 발생|
|2001|유효하지 않은 출발지|
|2003|유효하지 않은 목적지|
|2006|서버 응답 오류|
|2007|버퍼 NULL|
|2008|데이터 파싱 실패|
|2010|패킷 생성 실패|
|2011|패킷 생성 실패|
|2012|다운로드 실패|
|2013|유효하지 않은 파라미터|
|3000|알 수 없는 인증 오류|
|3001|초기 지도 다운로드 실패|
|3002|초기 지도 다운로드 실패|
|3003|지도 URL 오류|
|3004|안전운행 URL 오류|
|3005|안전운행 URL 오류|
|3006|안전운행 다운로드 실패|
|3007|인증 실패|
|3008|인증 업데이트 실패|
|3050|지도 엔진 초기화 실패|
|3051|SMR 엔진 초기화 실패|
|3052|맵매칭 엔진 초기화 실패 ( 위치권한 미 획득시 에도 발생할수 있음 )|
|3053|안내 엔진 초기화 실패|
|3054|기타 엔진 초기화 실패|
|4000|검색결과 없음|
|4001|유효하지 않은 검색어|
|5000|출발지 오류|
|5001|목적지 오류|
|5002|출발지가 유효 범위를 벗어난 경우|
|5003|목적지가 유효 범위를 벗어난 경우|
|5004|출발지와 목적지가 가까워 길찾기가 불가능|
|5005|안내중인 경로가 유효하지 않은 경우|
|6000|검색어 오류|