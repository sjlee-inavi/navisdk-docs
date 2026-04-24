# iNavi SDK Android 개발 가이드

# 개정이력

## [ 0.0.1 ] 2020-01-

## 인증 업데이트 추가

## [ 0.0.2 ] 2020-01-

## SDK 적용방법 추가

## [ 0.0.3 ] 2020-02-

## setDrivingStatusListener I/F

## nearGoalDist Param. 추가

## [ 0.0.4 ] 2020-03-

## 주행중 특정지점에서 비정상 종료되는 이슈 수정

## [ 0.0.5 ] 2020-03-

## Proguard 옵션추가

## [ 0.0.6 ] 2020-04-

## SDK 난독화 예외처리 추가 ( 통신관련 )

## App 난독화 가이드 추가

## [ 0.0.7 ] 2020-04-

## 길 찾기 I/F 파라미터 변경 ( runRoute, runSingleRoute )

## RouteExtraInfo 추가

## RoutePtItem 에 angle필드 추가

## [ 0.0.8 ] 2020-04-


## 과속 백그라운드 알림 추가

## [ 0.0.9 ] 2020-05-

## 차량 속도 Callback 추가 ( setCarSpeedListener )

## [ 0.0.10 ] 2020-05-

## 디버그 로그 제거

## 주행화면 TBT UI 개선 ( 차기/차차기 높이 및 간격 조정 )

## [ 0.0.11 ] 2020-06-

## 내부안정성 이슈 개선

## NaviLocation 에 속도 필드 추가

## [ 0.0.12 ] 2020-07-

## 주행화면 GUI 개선 ( 회전정보, 카메라정보, 현위치 버튼 등 )

## 길 찾기 실패 코드 추가 ( 코드표 : 5002, 5003, 5004 )

## [ 0.0.13 ] 2020-11-

## 기본 자차 아이콘 및 폰트 변경

## 주행화면 TBT UI 개선 ( 형태 및 컬러 변경 )

## 주행화면 TBT 출발/도착 아이콘 변경 I/F 추가 ( setTurnViewTaxiIcon )

## 지도 컴포넌트 Show/Hide I/F 수정 ( forceHideMapComponent )

## 도로명 주소 I/F 추가 ( getFullAddr )

## 현재 도로명 I/F 추가 ( getCurrentRoadName )

## 경유지 정보 I/F 추가 ( getRoutePtViaInfo )

## 주행정보 요금 필드 추가 ( getRemainRouteInfo )

## RouteRemainInfo에 remainFee 필드 추가

## NaviEvent Callback 추가 ( setNaviEventListener )

## 현위치 이동, 전체경로 보기

## [ 0.0.14 ] 2020-11-


## 주행 속도 레이아웃 오류 개선

## [ 0.0.15 ] 2020-11-

## Audio Stream Type 변경 I/F 추가 ( setAudioStreamType )

## [ 0.0.16 ] 2020-12-

## 지도 Style 변경 I/F 추가 ( setMapStyle )

## 도착예정시간 초기화 및 갱신 타이밍 개선

## [ 0.0.17 ] 2020-12-

## 총 주행정보 I/F 추가 ( getTotalRemainRouteInfo )

## getRemainRouteInfo의 Distance 갱신 로직 개선

## forceHideMapComponent 지도 컴포넌트 타입 추가

## MAPCOMPONENT.ROUTE_TRAFFIC_STATUS_BAR

## [ 0.0.18 ] 2021-02-

## Layout 초기화 I/F 추가 ( initLayout )

## 기존 initLayout I/F 에, 지도/주행의 부모 뷰 추가

## [ 0.0.19 ] 2021-02-

## SurfaceView Activity Casting 오류 개선

## [ 0.0.20 ] 2021-03-

## SDK 저장소 변경 [ 필수 적용 항목 ]

## Bintray 에서 Artifactory 로 변경

## NaviLocation 자료형 변형 [ 필수 적용 항목 ]

## angle 필드 자료형 Double 로 변경

## 화면회전 세팅 I/F 수정 ( setOrientation )

## ORIENTATION_UNDEFINED 추가


## [ 0.0.21 ] 2021-03-

## 내부적으로 사용하던 TimeZone 제거

## [ 0.0.22 ] 2021-04-

## minSdkVersion 19에서 21 로 변경 [ 필수 적용 항목 ]

## 경유지 기능 추가

## 기존 길찾기 I/F 에 경유지 Param 추가

## runRoute, runSingleRoute

## 남은 경유지 정보 I/F 추가

## getRoutePtRemainViaInfo

## getRemainViaRouteInfo

## 경유지 변경 재탐색 I/F 추가

## runReRouteChangeVia

## 에뮬레이터 지원

## 에뮬레이터 모드 I/F 추가 (setEmulatorMode)

## [ 0.0.23 ] 2021-08-

## 안내종료거리 튜닝

## 길찾기 I/F에 탐색옵션 Param 추가

## runRoute

## 안전운행정보 변경 기능 추가

## 안내설정 I/F 추가 (setGuidanceSettings, getGuidanceSettings)

## GUIDANCESETTING 추가

## [ 0.0.24 ] 2021-11-

## 안내종료거리 2차 튜닝

## 내부 모듈 안정성 개선

## 주행 경로선 색상 변경 기능 추가

## 경로선 색상 변경 I/F 추가 ( setMapRouteColor )

## MAPROUTECOLOR 추가


## [ 0.0.25 ] 2021-12-

## 내부 모듈 안정성 개선

## 주행중 전체 경로보기 기능 추가

## 전체 경로보기 I/F 추가 ( drivingRouteZoomMap )

## [0.0.26] 2022-03-

## 목적지 도착시 요금 반환 기능 추가

## 목적지 도착시 요금 반환 I/F 추가

## onArrivalFee ( OnDrivingStatusListener )

## setDrivingStatusListener 설명 추가

## onArrivalFee 사양 설명 추가

## [0.0.27] 2022-11-

## 경유지 사양 확대 (최대 100개까지 설정 가능)

## forceHideMapComponent 지도 컴포넌트 타입 추가

## MAPCOMPONENT.BOTTOM_NORMAL_SIDE_BUTTON

## MAPCOMPONENT.BOTTOM_DRIVING_SIDE_BUTTON

## MAPCOMPONENT.BOTTOM_ARRIVAL_LEFT_BUTTON

## 화물차 설정 및 전용 탐색 옵션 추가

## 차량 높이/중량/U-turn 도로폭/좁은길 도로폭/통행제한구간 회피 설정 옵션 추가

## setCarHeight , getCarHeight

## setCarWeight , getCarWeight

## setAvoidUturn , getAvoidUturn

## setAvoidNarrowRoad , getAvoidNarrowRoad

## setAvoidRestriction , getAvoidRestriction

## 화물차 전용 탐색 옵션 추가

## ROUTEOPTIONTYPE 수정

## [0.0.28] 2023-01-

## 지도 여백(Padding) 설정 I/F 추가

## routeZoomMapWithPadding

## setMapPadding


## clearMapPadding

## 차종 설정 I/F 추가

## setCarType, getCarType

## enum class CARTYPE 추가

## [0.0.29] 2023-01-

## 경유지 도착 알림 I/F 추가

## **OnDrivingStatusListener 수정 (**onArrivalVia 추가) [필수 적용 항목]

## TBT(TurnView) Custom Background Color 설정 I/F 추가

## setTurnViewBackgroundColor , getTurnViewBackgroundColor (차기 TurnView)

## setNextTurnViewBackgroundColor, getNextTurnViewBackgroundColor (차차기)

## setArrivalViewBackgroundColor , getArrivalViewBackgroundColor (목적지 도착 view)

## resetTurnViewsBackgroundColor (기본값으로 초기화)

## 확대도 표출 기능 및 표출 여부 I/F 추가

## setVisibleExtendView , getVisibleExtendView

## [0.5.0] 2023-03-

## 내부 모듈 안정성 개선

## [0.5.1] 2023-05-

## 경유지 도착 알림 I/F 사양 변경

## 탐색열 에서 진행방향으로 현 위치에서 가장 가까운 좌표 인덱스 반환 I/F 추가

## getNearestVertexIndex

## [0.5.2] 2023-05-

## 내부 모듈 안정성 개선

## [0.6.0] 2023-08-

## 내부 엔진 수정

## AndroidX 적용


## playground-service-location 버전 16.0.0 → 21.0.1 로 수정 (fusedLocationProvider 관련 내용

## 적용)

## [0.6.1] 2023-09-

## 경로탐색 실패 처리 사양 변경

## 경유지가 포함된 경우 출발지-목적지 간 거리 체크 하지 않도록 변경

## [ 0.6.2] 2023-10-

## SDK 저장소 URL 변경 (필수 적용)

## 화물차 전용옵션 로직 개선

## [ 0.6.3] 2024-04-

## 안정성 개선

## [ 0.6.4] 2024-04-

## 구글 정책 위반 관련 이슈 개선

## [ 0.7.0 ] 2024-04-

## kotlin version 업그레이드 (1.5.21)

## 가이드 문서 업데이트 (프로젝트 설정 관련 내용 추가)

## 라이브러리 종속성 항목 추가 (recyclerview)

## jvmtarget 관련 내용 추가

## [ 0.7.1 ] 2024-09-

## 내부 엔진 수정

## 상수원보호구역 회피탐색 기능 추가

## 최적탐색 기능 추가

## [ 0.7.2 ] 2024-10-

## 안내 음성 수정


## 후면카메라 단속 안내 추가

## 안내 UI 폰트 변경

## [ 0.7.3 ] 2025-03-

## 내부 엔진 수정

## iMPS 내제화에 따른 인증 서버 전환

## [ 0.7.4 ] 2025-07-

## 다음턴 , 다다음턴 (TBT View) 백그라운드 안내 기능 추가 (다른 앱 위에 그리기)

## 사용자가 설정 → 디스플레이 크기 옵션을 임의로 수정한 경우 안내 화면이 의도와 다르게 오히

## 려 축소 되던 문제 수정

## [ 0.8.0 ] 2025-10-

## Android 15 대응 (support 16kb page size)

## 위수지역 회피탐색 기능 추가

## [ 0.8.1 ] 2025-11-

## 아파트 동/호/명칭 충돌 기능 On/Off 기능 추가

## setAptPoiCollisionIgnored

## 지도 엔진 최신화

## [ 0.9.0 ] 2026-03-

## 일부 단말에서 안내 음성 마지막이 잘리는 현상 수정

## 지도 Style 변경 I/F 제거

## setMapStyle, MAPSTYLE

## Android Studio 최소지원 AGP 정책에 따라 AGP 7.4.2 적용

## AGP 4.1.0 미만의 경우 호환성 문제 발생 여지가 있으므로 AGP 7.x 계열로 맞추는것을 권장

## 합니다.

## 지도 엔진 최신화


# 개요

## 본 문서는 Android 기반 플랫폼에서 구동되는 "아이나비 내비게이션 SDK"(이하 SDK) 연동에 대

## 한 기술 문서 이다.

# Appkey 발급

# 개발 환경

## 개발 도구 : AndroidStudio 2025.2.2 Patch 1 이상

## 개발 언어 : Android, Kotlin

## SDK 지원 범위

## targetSdkVersion : 28 ( Android 9, P OS )

## minSdkVersion : 21 ( Android 5.0, LOLLIPOP OS )

# SDK 세팅 방법

## 1. SDK 저장소 추가

## a. Root Project build.gradle 파일

## 2. SDK 의존성 추가

## a. App build.gradle 파일

## SDK를 사용하기 위해서는 우선 Appkey 발급이 필요합니다. (규격서 제공 제휴 사업 담당자

## 통해 별도 요청 필요)

```
1 // Root Project build.gradle
2 allprojects {
3 repositories {
4 maven { url '<https://repo.inavi.com/artifactory/navigation/>' }
5 }
6 }
7
```
```
1 // App build.gradle
2 dependencies {
3 //SDK 의존성
4 implementation 'com.inavisys.navisdk:inavi-navigation-sdk:0.7.3'
5
6 //SDK가 사용하는 Library 의존성 추가
7 implementation 'com.google.code.gson:gson:2.8.5'
8
9 // SDK v0.6.0 이하 버전은 16.0.0 사용
10 // implementation 'com.google.android.gms:play-services-location:16.0.0'
11
12 // SDK v0.6.0 부터 반영
13 implementation 'com.google.android.gms:play-services-location:21.0.1'
14
15 // APP 내에서 ConstraintLayout 사용 시 2.0 이상 사용 하여야 함 (SDK-0.0.28 이후 버전 부터)
16 implementation 'androidx.constraintlayout:constraintlayout:2.1.4'
17
18 // 1.0.0 이상버전 사용 가능
```

## b. gradle.properties 파일

## 3. SDK 환경 세팅

## a. App build.gradle 파일

## ndk abiFilters 추가

## 컴파일 옵션 추가

## b. AndroidManifest.xml

## http 허용

## Apache.http.legacy 허용

## AppKey 등록

```
19 implementation ("androidx.recyclerview:recyclerview:1.3.2")
20 }
21
```
```
1 android.useAndroidX=true // SDK v0.6.0 부터 필수
```
```
1 android {
2 defaultConfig {
3 ndk {
4 abiFilters "arm64-v8a", "armeabi-v7a"
5 }
6 }
7 }
8
```
```
1 android {
2 ...
3
4 compileOptions {
5 sourceCompatibility JavaVersion.VERSION_1_
6 targetCompatibility JavaVersion.VERSION_1_
7 }
8
9 ...
10
11 kotlinOptions {
12 jvmTarget = "1.8"
13 }
14 }
15
```
```
1 <manifest>
2 <application
3 android:usesCleartextTraffic="true">
4 </application>
5 </manifest>
6
```
```
1 <manifest>
2 <application
3 <uses-library android:name="org.apache.http.legacy" android:required="false"/>
4 </application>
5 </manifest>
6
```
```
1 <manifest>
```

## 4. SDK 난독화 옵션 세팅

## a. proguard-rules.pro

## 5. SDK Layout 세팅

## a. 지도를 표출할 Layout(xml) 파일

## 지도 View : "com.inaviair.sdkEngine.MapAdapter" 추가

## 주행화면 View : "com.inaviair.sdkEngine.MapLayer" 추가

# SDK 권한 목록

## 1. SDK 를 사용하기 위한 필수 권한 목록

## 2. SDK 내부에 선언되어 있는 Permission 목록

```
2 <application
3 <meta-data android:name="com.inaviair.sdk.appkey" android:value="AppKey"/>
4 </application>
5 </manifest>
6
```
```
1 -keep class com.inaviair.sdk.** { *; }
```
```
1 <androidx.constraintlayout.widget.ConstraintLayout
2 android:layout_width="match_parent"
3 android:layout_height="match_parent">
4
5 <androidx.constraintlayout.widget.ConstraintLayout
6 android:layout_width="match_parent"
7 android:layout_height="match_parent">
8
9 <!-- 지도 View -->
10 <com.inaviair.sdkEngine.MapAdapter
11 android:id="@+id/mapAdapter"
12 android:layout_width="match_parent"
13 android:layout_height="match_parent"
14 android:visibility="visible"
15 />
16
17 <!-- 주행화면 View -->
18 <com.inaviair.sdkEngine.MapLayer
19 android:id="@+id/mapLayer"
20 android:layout_width="match_parent"
21 android:layout_height="match_parent"
22 android:visibility="visible"
23 />
24
25 </androidx.constraintlayout.widget.ConstraintLayout>
26 </androidx.constraintlayout.widget.ConstraintLayout>
```
## App 에서 필수로 권한을 획득 해야 함

```
1 Manifest.permission.ACCESS_FINE_LOCATION
2 Manifest.permission.ACCESS_COARSE_LOCATION
3 Manifest.permission.READ_EXTERNAL_STORAGE
4 Manifest.permission.WRITE_EXTERNAL_STORAGE
```
### 1 //통신


# SDK Interface

## 1. SDK 생명주기

## SDK 생명주기는 Application 생명주기와 동일하게 사용하는것을 권장

## SDK 의 내비게이션 지도 및 주행화면은, 앱실행시 최초실행되는 Activity 에서 구현

## loadNaviLibrary, initLayout, initalizeNavi, destroyNavi 는 앱실행당 1회만 호출

## 2. "INaviController" class 를 통하여 SDK 의 모든 기능 사용

## INaviController 는 Singleton 객체

## 비동기 처리는 SDK 에서 Callback 제공

## 3. 좌표계

## SDK 는 위경도 좌표를 사용

## DD(십진수 도) 방식 사용

## ex> 서울역 위도 : 37.553173, 경도 : 126.

```
2 <uses-permission android:name="android.permission.INTERNET"/>
3 <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
4 <uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
5 <uses-permission android:name="android.permission.CHANGE_WIFI_STATE"/>
6
7 //위치
8 <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
9 <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
10 <uses-permission android:name="android.permission.ACCESS_LOCATION_EXTRA_COMMANDS"/>
11
12 //저장소
13 <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
14 <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
15
```

# 시나리오별 예시

## 1. 초기화

## Activity 예시

## Fragment 예시

### 1 // SDK 초기화 예시

```
2 // 필수적으로 loadNaviLibrary, initLayout, initalizeNavi 가 호출 되어야 함
3 // 호출 순서 중요
4
5 class MainActivity : AppCompatActivity() {
6 companion object {
7 init {
8 // application 초기화 시에 호출 : 필수 호출
9 INaviController.loadNaviLibrary()
10 }
11 }
12
13 override fun onCreate(savedInstanceState: Bundle?) {
14 setContentView(R.layout.xxx)
15
16 //OnCreate 에서 호출 : 필수 호출
17 INaviController.initLayout(this, R.id.mapAdapter, R.id.mapLayer)
18
19 //음성 Stream 변경
20 INaviController.setAudioStreamType(AudioManager.STREAM_MUSIC)
21
22 val mdn = "UniqueID" // ex) UUID 등 고유식별자
23
24 //SDK 엔진 초기화 : 필수 호출
25 INaviController.initalizeNavi(this, getRootPath(), mdn,
26 object : OnNaviInitListener {
27 override fun onSuccess() {
28 // SDK 초기화 성공
29 }
30
31 override fun onFail(errCode: Int, errMsg: String) {
32 // SDK 초기화 실패
33 }
34 })
35 }
36
37 private fun getRootPath(): String {
38 var strStorageDir: String = ""
39 val fRootPath = ContextCompat.getExternalFilesDirs(this, null)
40 if (fRootPath.isNotEmpty() && fRootPath[0] != null)
41 strStorageDir = fRootPath[0].absolutePath
42
43 return strStorageDir
44 }
45 }
46
```
### 1 // SDK 초기화 예시

```
2 // 필수적으로 loadNaviLibrary, initLayout, initalizeNavi 가 호출 되어야 함
3 // 호출 순서 중요
4
5 class MainActivity : AppCompatActivity() {
6 companion object {
7 init {
```

## 2. 지도 아이콘 표출 및 제거

```
8 // application 초기화 시에 호출 : 필수 호출
9 INaviController.loadNaviLibrary()
10 }
11 }
12
13 override fun onCreate(savedInstanceState: Bundle?) {
14 setContentView(R.layout.xxx)
15
16 val mapFragment = MapFragment(this)
17 }
18 }
19
20 class MapFragment(private val acty: Activity) : Fragment() {
21 override fun onCreateView(inflater: LayoutInflater, container: ViewGroup?,
22 savedInstanceState: Bundle?): View? {
23
24 val rootView = inflater.inflate(R.layout.fragment_xxx, container, false)
25
26 //OnCreateView 에서 호출 : 필수 호출
27 INaviController.initLayout(acty, rootView, R.id.mapAdapter, R.id.mapLayer)
28
29 //음성 Stream 변경
30 INaviController.setAudioStreamType(AudioManager.STREAM_MUSIC)
31
32 val phoneNumber = "UniqueID"
33 //SDK 엔진 초기화 : 필수 호출
34 INaviController.initalizeNavi(this, getRootPath(), phoneNumber,
35 object : OnNaviInitListener {
36 override fun onSuccess() {
37 // SDK 초기화 성공
38 }
39
40 override fun onFail(errCode: Int, errMsg: String) {
41 // SDK 초기화 실패
42 }
43 })
44 }
45
46 private fun getRootPath(): String {
47 var strStorageDir: String = ""
48 val fRootPath = ContextCompat.getExternalFilesDirs(this, null)
49 if (fRootPath.isNotEmpty() && fRootPath[0] != null)
50 strStorageDir = fRootPath[0].absolutePath
51
52 return strStorageDir
53 }
54 }
55
```
### 1 // 변수 선언

```
2 var overlayMap: MapOverlay? = null
3 var iconEx: MapIcon?= null
4
5 // 지도 overlay 생성
6 overlayMap = INaviController.createMapOverlay()
7
8 // 필요하면 overlay에 mapIcon 클릭 이벤트 등록 가능
9 overlayMap?.setMapIconListener { icon ->
10 }
11
12 // 지도 아이콘 생성
13 val mapIcon = INaviController.createMapIcon( ... )
14
15 // 지도 아이콘을 overlay에 추가
```

## 3. 검색

## 4. 길 찾기, 안내시작

```
16 // 정상적으로 overlay에 추가되면 mapIcon이 반환 된다.
17 iconEx = INaviController.addMapIcon(overlayMap, mapIcon)
18
19 // ...
20 // ...
21 // ...
22
23 // 지도 아이콘 제거
24 INaviController.removeMapIcon(overlayMap, iconEx)
25 iconEx = null
26
27 // 지도 overlay 제거
28 INaviController.removeMapOverlay(overlayMap)
29 overlayMap = null
30
```
### 1 // 검색 쿼리

```
2 var query = "검색어"
3 var lat = 37.
4 var lon = 127.
5
6 // 검색 시작 및 결과 Callback 처리
7 INaviController.runSearch( query, lat, lon, object : OnSearchListener {
8 override fun onSuccess(result : SearchResult ) {
9 // 검색 성공 처리
10 }
11 override fun onFail(errCode: Int, errMsg: String ) {
12 // 검색 실패 처리
13 }
14 })
15
```
### 1 // 출발지, 목적지

```
2 var startPoint: RoutePtItem
3 var goalPoint: RoutePtItem
4
5 //경유지
6 var viaList = mutableListOf<RoutePtItem>()
7
8 viaList.add(
9 RoutePtItem( “이름”,37.00000, 127.00000, 0.0, 0.0, 0)
10 )
11
12 // 부가정보
13 var extraInfo: RouteExtraInfo
14
15 // 안내시작에 사용할 경로
16 var routeID: String = “”
17
18 // 길찾기에 사용할 탐색 옵션
19 val optionType = mutableListOf<ROUTEOPTIONTYPE>()
20 optionType.add(ROUTEOPTIONTYPE.HIGHWAYPRIOTY)
21 optionType.add(ROUTEOPTIONTYPE.MOTOCYCLE)
22
23 // 길 찾기 시작 및 결과 Callback 처리
24 INaviController.runRoute( startPoint, goalPoint, viaList, optionType, extraInfo,
25 object : OnRouteMultiListener {
26 override fun onSuccess(result : ArrayList<String>, same: Boolean ) {
27 // 길 찾기 성공 처리
28
29 // 안내시작에 사용할 경로 ID 저장
```

## 5. 주행중 경유지 변경 재 탐색

## 6. 안전운행정보 안내 변경

```
30 routeID = result[0]
31 // 지도 화면 경로에 맞게 스케일 조절
32 // 모든 경로에 맞춰 스케일 되며, param 에 맞는 경로는 select 상태가 됨
33 INaviController.routeZoomMap(result, routeID)
34 }
35
36 override fun onFail(errCode: Int, errMsg: String ) {
37 // 길 찾기 실패 처리
38 }
39 })
40
41 // ...
42 // ...
43 // ...
44
45 // 주행 안내 시작
46 INaviController.runGuidance(routeID)
47
48 // 모의 주행 시작
49 INaviController.startSimulation(routeID)
50
```
### 1 // 주행중 지나가지 않은 경유지 정보 확인 ( 남은시간, 남은거리 )

```
2 var remainViaInfo: List<RouteViaRemainInfo>? = INaviController.getRemainViaRouteInfo()
3
4 // 주행중 지나가지 않은 경유지 정보 확인 ( 좌표 )
5 var rVia: List<RoutePtItem>? = INaviController.getRoutePtRemainViaInfo()
6
7 // 새로운 경유지 정보 생성
8 var viaList = mutableListOf<RoutePtItem>()
9
10 viaList.add(
11 // 기존 경유지 정보를 추가
12 RoutePtItem( rVia[0].name, rVia[0].rpLat, rVia[0].rpLon, 0.0, 0.0, 0)
13 )
14
15 viaList.add(
16 // 새로운 지점을 추가
17 RoutePtItem( “이름”,37.00000, 127.00000, 0.0, 0.0, 0)
18 )
19
20 // 경유지 변경 재 탐색
21 INaviController.runReRouteChangeVia(viaList, object: OnReRouteResultListener {
22 override fun onSuccess() {
23 // 재탐색 성공
24 // 새로운 경로로 자동 안내시작 됨
25 }
26
27 override fun onFail(errCode: Int, msg: String) {
28 // 재탐색 실패
29 }
30 })
31
```
### 1 // 현재 설정 값을 가져옴

```
2 var settings = INaviController.getGuidanceSettings().toMutableList()
3
4 // 과속방지턱 안내가 없다면, 추가
5 val exist = settings.find { it == GUIDANCESETTING.SPEED_BUMP }
6 if( exist == null ) {
7 settings.add(GUIDANCESETTING.SPEED_BUMP)
```

## 7. 화물차 특화 옵션 적용

### 8 }

### 9

### 10 // 교통정보 수집카메라 안내가 존재하면, 삭제

```
11 settings.find { it == GUIDANCESETTING.FIX_TRAFFIC }?.let { item ->
12 settings.remove(item)
13 }
14
15 // SDK에 현재 설정 적용
16 INaviController.setGuidanceSettings(settings)
17
```
### 1 // 설정 값은 재실행 시에도 유지되며, 앱 삭제 시 초기화

### 2

### 3 // 회피옵션을 설정하였더라도 해당경로가 유일한 경로일 경우에는 제한구역을 포함하는 경로로 안내될 수 있음

### 4 // 각각의 설정값은 별개의 사양으로 동작

```
5 // e.g)
6 // 1. 높이값만 설정 시 -> 좁은길, 유턴도로, 중량제한 적용 X
7 // 2. 좁은길, 유턴도로만 회피 설정 시 -> 높이, 중량제한 적용 X
8 // 3. 높이제한 설정하였으나 높이제한구역을 포함하는 경로가 '유일한' 경로일 때 -> 해당구역 포함하여 안내
9
10 var nHeight : Int = INaviController.getCarHeight() // (default : 0)
11 var nWeight : Int = INaviController.getCarWeight() // (default : 0)
12 var nAvoidNarrow : Int = INaviController.getAvoidNarrowRoad() // (default : 0)
13 var nAvoidUturn : Int = INaviController.getAvoidUturn() // (default : 0)
14 var bIsAvoidRestriction : Boolean = INaviController.getAvoidRestriction() // (default : false)
15
16 /** 도로통과 높이 제한 기능 설정 (cm) **/
17 // 0 ~ 1000cm [10m]
18 val nValue = value.toIntOrNull()
19 if(nValue != null){
20 // 제한구역을 통과하는 경로가 유일한 경로일 경우에는 해당 경로로 안내 될 수 있음.
21 INaviController.setCarHeight(nValue)
22 }
23
24 /** 도로통과 중량 제한 기능 설정 (kg) **/
25 // 0 ~ 60000kg [60t]
26 val nValue = value.toIntOrNull()
27 if(nValue != null){
28 // 제한구역을 통과하는 경로가 유일한 경로일 경우에는 해당 경로로 안내 될 수 있음.
29 INaviController.setCarWeight(nValue)
30 }
31
32 /** 왕복 n차선 이하 유턴 회피 **/
33 val nValue = value.toIntOrNull()
34 if(nValue != null){
35 INaviController.setAvoidUturn(nValue)
36 }
37
38 /** 왕복 n차선 이하 도로 회피 **/
39 val nValue = value.toIntOrNull()
40 if(nValue != null){
41 INaviController.setAvoidNarrowRoad(nValue)
42 }
43
44 /** 화물차 통행제한구간 회피 **/
45 val bVal = value.toBoolean()
46 INaviController.setAvoidRestriction(bVal)
47
48 /** 위수지역 회피 **/
49 val bVal = value.toBoolean()
50 INaviController.setAvoidEvasion(bVal)
51
52
```

## 8. 차종 설정

## 9. 지도 여백 (Padding) 적용

## 10. TurnView(차기,차차기, 목적지 도착 view) 배경색 변경

### 1 // 설정 값은 재실행 시에도 유지되며, 앱 삭제 시 초기화

### 2 /**

```
3 * type (value[int]) : title / description
4 * TYPE_1 (0) = 1종(소형차) / 일반승용, 승합16인 이하, 화물2.5톤 미만
5 * TYPE_2 (1) = 2종(중형차) / 승합32인 이하, 화물5.5톤 이하
6 * TYPE_3 (2) = 3종(대형차) / 승합33인 이상, 화물10톤 미만
7 * TYPE_4 (3) = 4종(대형화물차) / 화물20톤 미만
8 * TYPE_5 (4) = 5종(특수화물차) / 화물20톤 이상
9 * TYPE_6 (5) = 경차 / 1종 : 통행료 할인 적용
10 * TYPE_7 (6) = 이륜차 / ""
11 *
12 * */
13
14 // 차종 값 불러오기 ( default : TYPE_1 )
15 val curType = INaviController.getCarType()
16 // 차종 제목
17 val carTypeTitle = CARTYPE.getTitle(curType) // "1종(소형차)"
18 // 차종 설명
19 val carTypeDescription = CARTYPE.getDescription(curType) // "일반승용, 승합16인 이하, 화물2.5톤 미만"
20
21 // 차종 설정
22 INaviController.setCarType(CARTYPE.TYPE_1)
23
24 // int to CARTYPE 변환하여 차종 설정 예시
25 // 위 setCarType(CARTYPE.TYPE_1)과 같은 결과가 적용된다.
26 INaviController.setCarType(CARTYPE.from(0))
```
### 1 // 사용자가 설정한 패딩 값은 안내 사양에 따라 초기화 될 수 있다.

```
2 // e.g) 주행 시작시 설정값 초기화
3
4 // RectF 생성 파라메터는 left,top,right,bottom 순서
5 // 1. 경로선택 화면 지도에 하단 60dp 만큼의 패딩을 추가로 적용 예시
6 INaviController.routeZoomMapWithPadding(rIdList, selectedRid, android.graphics.RectF(0f,0f,0f,60f))
7
8 // 2. 기본지도에 패딩 적용 예시(경로안내/모의주행이 아닐 때)
9 INaviController.setMapPadding(android.graphics.RectF(0f,0f,0f,60f))
10
11 //지도에 적용한 패딩값 초기화
12 INaviController.clearMapPadding()
```
### 1 // 설정 값은 재실행 시에도 유지되며, 앱 삭제 시 초기화

### 2

```
3 // 현재 적용된 차기 turnview bg 얻어오기
4 val strCurTurnBg = INaviController.getTurnViewBackgroundColor()
5
6 /* 사용 가능한 색상명
7 red, blue, green, black, white, gray, cyan, magenta, yellow,
8 lightgray, darkgray, grey, lightgrey, darkgrey, aqua,
9 fuchsia, lime, maroon, navy, olive, purple, silver,teal.
10 */
11
12 // 차기 turnview에 색상명으로 배경값 적용
13 INaviController.setTurnViewBackgroundColor("black")
14
15 // 차차기 turnview에 16진수 String으로 배경값 적용 "#AARRGGBB"
16 INaviController.setNextTurnViewBackgroundColor("#f21e55f7")
17
18 // 목적지 도착 view에 16진수 String으로 배경값 적용 "#RRGGBB"
```

## 11. 확대도 표출

## 12. 현위치에서 진행방향으로 탐색열에서 가장 가까운 좌표 얻기

```
19 INaviController.setArrivalViewBackgroundColor("#1e55f7")
20
21 // 적용한 Custom background color 초기화
22 INaviController.resetTurnViewsBackgroundColor()
```
### 1 // 설정 값은 재실행 시에도 유지되며, 앱 삭제 시 초기화

### 2

```
3 // 현재 적용된 확대도 표출 여부 가져오기 (default : false)
4 val bIsShowExtendView = INaviController.getVisibleExtendView()
5
6 // 확대도 표출하도록 적용
7 INaviController.setVisibleExtendView(true)
```
```
확대도 표출 사양(가로모드)
```
```
확대도 표출 사양(세로모드)
```
### 1 // 엔진초기화 또는 경로가 설정되지 않았을 경우 -1 반환

```
2 // 현재 선택한 경로의 RouteID 필요
```

## 13. 백그라운드에서 TBT 표출하기

### 3

```
4 // 경로 Line 좌표열 얻기
5 var routeLinePoints = INaviController.getRouteLinePoints(strRouteId)
6
7 // 현위치에서 진행방향으로 경로 Line 좌표열 내에서 가장 가까운 index 얻기
8 var nIdx = INaviController.getNearestVertexIndex()
9
```
```
1 // ** AndroidMainfest 에 아래 권한 명시 필요 **
2 <uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW" />
```
```
1 // MainActivity 또는 상태주기를 관리하는 곳에서 백그라운드 <-> 포그라운드 전환 시 SDK에 세팅
2 override fun onResume() {
3 super.onResume()
4 // ** 중요 **
5 // 앱이 Foreground 로 전환 될 경우 Background TBT 를 그리지 않기 위해 APP STATUS 업데이트
6 INaviController.setApplicatonStatus(APPSTATUS.FOREGROUND)
7 }
8
9 override fun onStop() {
10 super.onStop()
11 // ** 중요 **
12 // 앱이 Background 로 전환 될 경우 Background TBT 를 그리기 위해 APP STATUS 업데이트
13 INaviController.setApplicatonStatus(APPSTATUS.BACKGROUND)
14 }
15
16 // initializeNavi 이후에 호출
17 private fun initBackgroundTBT(){
18 // 1. '다른 앱 위에 그리기' 권한 요청
19 if(!Settings.canDrawOverlays(applicationContext)){
20 val intent = Intent(
21 Settings.ACTION_MANAGE_OVERLAY_PERMISSION, "package:$packageName".toUri()
22 )
23 startActivityForResult(intent, REQUEST_CODE_TBT_PERMISSION)
24 }
25
26 // 2. Background TBT Draw 여부 SDK 에 설정
27 // 해당 기능이 설정 되어있어도 '다른 앱 위에 그리기' 권한이 설정되지 않은경우 그리지 않음.
28 // 해당 기능은 모의주행이 아닌 '안내시작' 상태일때만 동작합니다 (runGuidance)
29 INaviController.setDrawBackgroundTBT(true)
30
31 // 3. Background TBT 를 클릭 하면 돌아올 액티비티 설정 ( 설정하지 않으면 클릭 이벤트 무시 )
32 INaviController.setBringToFrontListener(object : OnBringToFrontListener {
33 override fun getBringToFrontPendingIntent(context: Context?): PendingIntent? {
34 val intent = Intent(context, MainActivity::class.java)
35 intent.setFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)
36
37 var flags = PendingIntent.FLAG_UPDATE_CURRENT
38 if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.S) {
39 flags = flags or PendingIntent.FLAG_IMMUTABLE
40 }
41
42 return PendingIntent.getActivity(context, 0, intent, flags)
43 }
44 })
45 }
46
```

# INaviController Reference

## 1. 초기화

## a. loadNaviLibrary

## b. initLayout

## c. initLayout

```
Background TBT 표출 예시
```
```
1 fun loadNaviLibrary()
2
3 Description : SDK에서 사용하는 native lib 로딩
4 * Application 초기화 단계에서 호출 필요
5 * initalizeNavi 호출전에 호출 필요
6
7 Param : void
8 Return : void
```
```
1 fun initLayout(acty: Activity, mapViewID: Int, guideViewID: Int): Boolean
2
3 Description : 지도/주행 뷰 초기화
4 * Root Activity onCreate 에서 호출 가능
5 * initalizeNavi 호출전에 호출 필요
6
7 Param
8 - acty = 지도/주행 뷰를 포함하는 Activity
9 - mapViewID = xml에 추가한 지도 리소스 ID
10 - guideViewID = xml에 추가한 주행화면 리소스 ID
11 Return : Boolean
```
```
1 fun initLayout(acty: Activity, parentView: View, mapViewID: Int, guideViewID: Int): Boolean
2
3 Description : 지도/주행 뷰 초기화
4 * Root Activity onCreate / Fragment onCreateView 에서 호출 가능
```

## d. setMapStyle ( deprecated, v0.9.0 )

## e. setAudioStreamType

## f. setEmulatorMode

## g. initalizeNavi

```
5 * initalizeNavi 호출전에 호출 필요
6
7 Param
8 - acty = View(Fragment)를 포함하는 Activity
9 - parentView = 지도/주행 뷰의, 부모 뷰(Parent View)
10 - mapViewID = xml에 추가한 지도 리소스 ID
11 - guideViewID = xml에 추가한 주행화면 리소스 ID
12 Return : Boolean
```
```
1 @deprecated
2 fun setMapStyle(style: MAPSTYLE)
3
4 Description : 지도 Style 변경
5 * initalizeNavi 호출전에 호출 필요
6 * 미 호출시 Default 지도 사용
7
8 Param
9 - style = 지도 style 타입 (MAPSTYLE)
10 Return : void
```
```
1 fun setAudioStreamType(streamType: Int)
2
3 Description : 내비게이션 음성 Stream Type 변경
4 * initalizeNavi 호출전에 호출 필요
5 * 미 호출시 STREAM_MUSIC 사용
6
7 Param
8 - streamType = 스트림 타입(AudioManager.STREAM_MUSIC, AudioManager.STREAM_NOTIFICATION)
9 Return = void
```
```
1 fun setEmulatorMode(emulator: Boolean)
2
3 Description : 타겟 단말 타입 설정
4 * initalizeNavi 호출전에 호출 필요
5 * 미 호출시 "단말기 타입" 사용
6
7 Param
8 - emulator = 타겟 단말 타입(true : 에뮬레이터 / false : 실제 단말기 )
9 Return : void
```
```
1 fun initalizeNavi(context: Context, rootPath: String, uniqueID: String,
2 listener: OnNaviInitListener)
3
4 Description : SDK 엔진 초기화
5 * 초기화 단계의 I/F(loadNaviLibrary, initLayout 등) 를 제외한 모든 I/F는 initalizeNavi 이후에 호출 가능
6 * 결과가 성공인 경우에만 SDK가 정상 동작 함
7
8 Param
9 - context : Application Context
10 - rootPath : Application 폴더 경로
11 - uniqueID : 유일 식별자 ( 필수값, 20자 이하 Alphanumeric )
12 - listener : interface OnNaviInitListener {
13 fun onSuccess()
14 fun onFail(errCode: Int, errMsg: String)
15 } = 결과 성공/실패 여부 Callback
```

## 2. 지도 컨트롤

## a. setMapClickListener

## b. setCarCurrentPosition

## c. setCarPosition

## d. setMapPosition

## e. zoomIn

## f. zoomOut

```
16 Return : void
```
```
1 fun setMapClickListener(listener: OnMapClickListener)
2
3 Description : 지도 롱 클릭 Listener 등록
4
5 Param
6 - listener : interface OnMapClickListener {
7 fun onMapLongClick(lat: Double, lon: Double)
8 } = 지도 롱 클릭 위치 좌표[WGS84] 반환 Callback
9 Return : void
```
```
1 fun setCarCurrentPosition()
2
3 Description : 지도와 자차를 GPS 위치로 이동
4
5 Param : void
6 Return : void
```
```
1 fun setCarPosition(lat: Double, lon: Double, angle: Double)
2
3 Description : 지도와 자차를 특정 위치로 이동
4
5 Param
6 - lat : 위도 (이동 시킬 좌표의 y값 [WGS84])
7 - lon : 경도 (이동 시킬 좌표의 x값 [WGS84])
8 - angle : 각도
9 Return : void
```
```
1 fun setMapPosition(lat: Double, lon: Double, angle: Double)
2
3 Description : 지도를 특정 위치로 이동
4
5 Param
6 - lat : 위도 (이동 시킬 좌표의 y값 [WGS84])
7 - lon : 경도 (이동 시킬 좌표의 x값 [WGS84])
8 - angle : 각도
9 Return : void
```
```
1 fun zoomIn()
2
3 Description : 현재 레벨에서 한 단계 확대
4
5 Param : void
6 Return : void
```
```
1 fun zoomOut()
2
```

## g. setMapViewMode

## h. getMapViewMode

## i. visibleTrafficLine

## j. createMapOverlay

## k. createMapIcon

```
3 Description : 현재 레벨에서 한 단계 축소
4
5 Param : void
6 Return : void
```
```
1 fun setMapViewMode(mode: MAPVIEWMODE)
2
3 Description : 지도 뷰 모드 변경
4
5 Param
6 - mode = 지도 뷰 모드
7 Return : void
```
```
1 fun getMapViewMode(): MAPVIEWMODE
2
3 Description : 현재 지도 뷰 모드 반환
4
5 Param : void
6 Return
7 - MAPVIEWMODE = 지도 뷰 모드
```
```
1 fun visibleTrafficLine(show: Boolean)
2
3 Description : 지도에 교통정보 라인 표출
4
5 Param
6 - show = 교통정보 라인 표출 여부 ( true : 표출 / false : 미 표출 )
7 Return : void
```
```
1 fun createMapOverlay(): MapOverlay?
2
3 Description : 지도 아이콘(MapIcon)을 관리하는 Overlay 생성 및 반환
4
5 Param : void
6 Return
7 - MapOverlay
```
```
1 fun createMapIcon(lat: Double, lon: Double, normalResID: Int, selectedResID: Int,
2 gravity: ICONGRAVITY, minLevel: Int, maxLevel: Int, clickable: Boolean): MapIcon?
3
4 Description : 지도 아이콘(MapIcon) 생성 및 반환
5
6 Param
7 - lat = 위도 (아이콘을 표출할 좌표 y값 [WGS84])
8 - lon = 경도 (아이콘을 표출할 좌표 x값 [WGS84])
9 - normalResID = 아이콘에 표출할 기본 리소스 ID
10 - selectedResID = 아이콘이 선택된 상태일때 표출할 리소스 ID
11 - gravity = 아이콘 표출 위치
12 - minLevel = 아이콘이 표출될 최소 지도 레벨
13 - maxLevel = 아이콘이 표출될 최대 지도 레벨
14 - clickable = 클릭 이벤트 동작 여부
15 Return : MapIcon
```

## l. createMapIcon

## m. addMapIcon

## n. removeMapIcon

## o. removeMapIconAll

## p. routeZoomMap ( deprecated, 20/01/16 )

## q. routeZoomMap

```
1 fun createMapIcon(lat: Double, lon: Double, normalResID: Int, gravity: ICONGRAVITY): MapIcon?
2
3 Description : 지도 아이콘(MapIcon) 생성 및 반환
4
5 Param
6 - lat : 위도 (아이콘을 표출할 좌표 y값 [WGS84])
7 - lon : 경도 (아이콘을 표출할 좌표 x값 [WGS84])
8 - normalResID : 아이콘에 표출할 기본 리소스 ID
9 - gravity : 아이콘 표출 위치
10 Return : MapIcon
```
```
1 fun addMapIcon(overlay: MapOverlay, mapIcon: MapIcon): MapIcon?
2
3 Description : MapOverlay 에 지도 아이콘(MapIcon) 추가
4
5 Param
6 - overlay = 지도 아이콘(MapIcon) 이 추가될 MapOverlay
7 - mapIcon = MapOverlay 에 추가할 지도 아이콘(MapIcon)
8 Return
9 - MapIcon = MapOverlay에 정상적으로 추가된 지도 아이콘(MapIcon)
```
```
1 fun removeMapIcon(overlay: MapOverlay, mapIcon: MapIcon)
2
3 Description : MapOverlay 에서 지도 아이콘(MapIcon) 제거
4
5 Param
6 - overlay = 지도 아이콘(MapIcon) 이 포함된 MapOverlay
7 - mapIcon = MapOverlay에서 제거할 지도 아이콘(MapIcon)
8 Return : void
```
```
1 fun removeMapIconALL(overlay: MapOverlay)
2
3 Description : MapOverlay 에 포함된 모든 지도 아이콘(MapIcon) 제거
4
5 Param
6 - overlay = 지도 아이콘(MapIcon) 이 포함된 MapOverlay
7 Return : void
```
```
1 @deprecated
2 fun routeZoomMap(rid: String)
3
4 Description : 탐색 경로 비율에 맞게 지도 스케일 조절
5 * OnRouteMultiListener/OnRouteSingleListener 성공시에만 호출 가능
6
7 Param
8 - rid : 활성화 시킬 경로 ID (runRoute/runSingleRoute 에서 획득)
9 Return : void
```
```
1 fun routeZoomMap(ridList: ArrayList<String>?, selectedRID: String)
2
```

## r. routeZoomMapWithPadding

## s. setMapPadding

## t. clearMapPadding

## u. drivingRouteZoomMap

## v. setMapLevel

```
3 Description : 탐색 경로 비율에 맞게 지도 스케일 조절
4 * OnRouteMultiListener/OnRouteSingleListener 성공시에만 호출 가능
5
6 Param
7 - ridList = 탐색결과 경로 ID Array
8 - selectedRID = 활성화 시킬 경로 ID (runRoute/runSingleRoute 에서 획득)
9 Return : void
```
```
1 fun routeZoomMapWithPadding(ridList: ArrayList<String>?, selectedRID: String,
2 fPaddingRect: android.graphics.RectF)
3
4 Description : 탐색 경로 비율에 Padding값을 추가로 적용한 지도 스케일 조절
5 * OnRouteMultiListener/OnRouteSingleListener 성공시에만 호출 가능
6 * fRectPadding의 left,top,right,bottom 값은 DP 단위
7
8 Param
9 - ridList = 탐색결과 경로 ID Array
10 - selectedRID = 활성화 시킬 경로 ID (runRoute/runSingleRoute 에서 획득)
11 - fPaddingRect = 추가로 적용 시킬 지도의 상하좌우 여백값
12 Return : void
```
```
1 fun setMapPadding(fPaddingRect : android.graphics.RectF)
2
3 Description : 지도에 Padding 값 적용
4 * fRectPadding의 left,top,right,bottom 값은 DP 단위
5 * 경로안내/모의주행 시 해당 여백값은 초기화되며 안내 사양에 따른 여백값이 적용
6
7 Param
8 - fPaddingRect = 적용 시킬 지도의 상하좌우 여백값
9 Return : void
```
```
1 fun clearMapPadding()
2
3 Description : 지도에 적용한 Padding값 초기화
4
5 Param : void
6 Return : void
```
```
1 fun drivingRouteZoomMap()
2
3 Description : 주행 경로 비율에 맞게 지도 스케일 조절
4 * 안내시작 이후에만 호출 가능
5 * 약 7초후 자동 현위치 복귀 ( 사용자 인터랙션 발생시 7초 Reset )
6 * 전체경로보기중 현위치I/F 호출시 바로 현위치 복귀
7
8 Param : void
9 Return : void
```
```
1 fun setMapLevel(level: Int): Boolean
2
3 Description : 지도 레벨 변경
4
5 Param
```

## w. setMapFontSizeType

## x. getMapFontSizeType

## y. setMapDayNightMode

## z. getMapDayNightMode

## aa. setMapEnableRotate

## ab. setMapMoveChangedListener

```
6 - level = 변경할 지도 레벨 ( 1 ~ 13 )
7 Return : void
```
```
1 fun setMapFontSizeType(type: MAPFONTSIZETYPE)
2
3 Description : 지도 주기 폰트 사이즈 타입 변경
4
5 Param
6 - type : MAPFONTSIZETYPE = 폰트 사이즈 타입
7 Return : void
```
```
1 fun getMapFontSizeType(): MAPFONTSIZETYPE
2
3 Description : 지도 주기 폰트 사이즈 타입 반환
4
5 Return : MAPFONTSIZETYPE = 폰트 사이즈 타입
```
```
1 fun setMapDayNigthMode(mode: MAPDAYNIGHTMODE)
2
3 Description : 지도 주/야 타입 변경
4
5 Param
6 - mode : MAPDAYNIGHTMODE = 지도 주/야 타입
7 Return : void
```
```
1 fun getMapDayNightMode(): MAPDAYNIGHTMODE
2
3 Description : 지도 주/야 타입 반환
4
5 Param : void
6 Return : MAPDAYNIGHTMODE = 지도 주/야 타입
```
```
1 fun setMapEnableRotate(enable: Boolean)
2
3 Description : 지도 회전 가능 여부 설정
4
5 Param
6 - Boolean : 지도 회전 가능 여부 ( true : 회전 가능 / false : 회전 불가 )
7 Return : void
```
```
1 fun setMapMoveChangedListener(listener: OnMapMoveChangedListener)
2
3 Description : 지도 제스처를 통한 지도 이동 이벤트 전달
4
5 Param
6 - listener : interface OnMapMoveChangedListener {
7 fun onStart()
8 fun onStop()
9 } = 지도 이동 시작/종료 Callback
10 Return : void
```

## ac. forceHideMapComponent ( deprecated, 20/10/14 )

## ad. forceHideMapComponent

## ae. setTurnViewTaxiIcon

## af. setMapRouteColor

## ag. setAptPoiCollisionIgnored

## 3. 검색

## a. runSearch

```
1 @deprecated
2 fun forceHideMapComponent()
3
4 Description : 주행 지도 컴포넌트 강제 Hide
5
6 Param : void
7 Return : void
```
```
1 fun forceHideMapComponent(componentID: MAPCOMPONENT, hide: Boolean)
2
3 Description : 주행 지도 컴포넌트 강제 Hide
4
5 Param
6 - componentID = 지도 컴포넌트 타입
7 - hide = 컴포넌트 표출 여부 ( true : 미 표출 / false : 표출 )
8 Return : void
```
```
1 fun setTurnViewTaxiIcon(showTaxiIcon: Boolean)
2
3 Description : 주행화면 TBT 아이콘 변경 ( 출발/도착 -> 탑승/하차 )
4
5 Param
6 - showTaxiIcon = 아이콘 타입 여부 ( true : 탑승/하차 아이콘 / false : 출발/도착 아이콘 )
7 Return : void
```
```
1 fun setMapRouteColor(color: MAPROUTECOLOR)
2
3 Description : 주행화면 경로선 색상 변경
4
5 Param
6 - color = 경로선 색상 타입
7 Return : void
```
```
1 fun setAptPoiCollisionIgnored(bEnable: Boolean)
2
3 Description : 아파트 동/호/명칭 충돌 처리대상 제외 적용 (Default : False)
4
5 Param
6 - bEnable = 충돌 처리 여부 (true : 충돌처리 제외[충돌시 모두 표출] , false : 충돌처리 )
7 Return : void
```
```
1 fun runSearch(query: String, lat: Double, lon: Double, listener: OnSearchListener)
2
3 Description : 통합검색 결과 반환
4
5 Param
6 - query : 검색어
7 - lat : 위도 (검색에 사용되는 기준 좌표 y)
```

## b. runRecommendWord

## c. getJibunAddr

## d. getFullAddr

## e. getCurrentRoadName

## 4. 길찾기

## a. runRoute

```
8 - lon : 경도 (검색에 사용되는 기준 좌표 x)
9 - listener : interface OnSearchListener {
10 fun onSuccess(result: SearchResult)
11 fun onFail(errCode: Int, errMsg: String)
12 } = 검색 성공 여부 및 결과 반환
13 Return : void
```
```
1 fun runRecommendWord(query: String, listener: OnRecommendWordListener)
2
3 Description : 추천어 검색
4
5 Param
6 - query : 검색어
7 - listener : OnRecommendWordListener {
8 fun onSuccess(result : ArrayList<RecommendWord>)
9 fun onFail(errCode: Int, errMsg: String)
10 } = 추천어 성공 여부 및 결과 반환
11 Return : void
```
```
1 fun getJibunAddr(lat: Double, lon: Double): String
2
3 Description : 축약형 지번주소 반환
4
5 Param
6 - Double : 위도
7 - Double : 경도
8 Return
9 - String : 축약형 지번 주소
```
```
1 fun getFullAddr(lat: Double, lon: Double, roadAddrType: Boolean): String
2
3 Description : 전체 주소 반환
4 * 도로명 주소 요청의 경우, 도로명 주소가 없으면 지번주소 반환
5
6 Param
7 - lat : 위도 (주소를 얻어올 위치의 좌표 y [WGS84])
8 - lon : 경도 (주소를 얻어올 위치의 좌표 x [WGS84])
9 - roadAddrType : 주소 타입 ( true : 도로명 주소 / false : 지번 주소 )
10 Return
11 - String : 전체 주소
```
```
1 fun getCurrentRoadName(): String
2
3 Description : 현재 위치 도로명 반환
4 * 경로가 존재하고, 현재위치(자차)가 경로위에 존재하는 경우에만 도로명 반환
5
6 Param : void
7 Return
8 - String : 도로명
```
```
1 fun runRoute(start: RoutePtItem, goal: RoutePtItem, viaList: List<RoutePtItem>?,
```

## b. runSingleRoute

## c. runReRouteChangeVia

## d. makeRouteSumInfo

## e. getRoutePtInfo

```
2 optionType: List<ROUTEOPTIONTYPE>?, extraInfo: RouteExtraInfo?,
3 listener: OnRouteMultiListener)
4
5 Description: 길 찾기 ( 멀티 경로 )
6
7 Param
8 - start = 출발지 정보
9 - goal = 목적지 정보
10 - viaList = 경유지 리스트 ( 최대 100개 )
11 - optionType = 탐색 옵션 정보 ( Default 옵션 사용시 null 입력 )
12 - extraInfo = 부가정보 ( 필요없을시 null 입력 )
13 - listener = 탐색 결과( 경로 ID ) 리스트 반환
14 Return : void
```
```
1 fun runSingleRoute(start: RoutePtItem, goal: RoutePtItem, viaList: List<RoutePtItem>?,
2 option: ROUTEOPTIONTYPE, extraInfo: RouteExtraInfo?,
3 listener: OnRouteSingleListener)
4
5 Description : 길 찾기 ( 단일 경로 )
6
7 Param
8 - start = 출발지 정보
9 - goal = 목적지 정보
10 - viaList = 경유지 리스트 ( 최대 100개 )
11 - optionType = 탐색 옵션 정보 ( Default 옵션 사용시 null 입력 )
12 - extraInfo = 부가정보 ( 필요없을시 null 입력 )
13 - listener : interface OnRouteSingleListener {
14 fun onSuccess(result: String)
15 fun onFail(errCode: Int, msg: String)
16 } = 단일 탐색 결과( 경로 ID ) 반환
17 Return : void
```
```
1 fun runReRouteChangeVia(viaList: List<RoutePtItem>?, listener: OnReRouteResultListener)
2
3 Description : 주행중, 경유지 변경하여 재탐색
4 * 기존 안내하던 경로가 존재 해야 함
5 * 기존 안내하던 경유지는 삭제 되고, 새로운 경유지로 안내
6
7 Param
8 - viaList : 경유지 리스트 ( 최대 100개 )
9 - listener : interface OnReRouteResultListener {
10 fun onSuccess(result: String)
11 fun onFail(errCode: Int, msg: String)
12 } = 재탐색 결과 성공여부 반환
13 Return : void
```
```
1 fun makeRouteSumInfo(routeID: String): RouteSumInfo
2
3 Description: 경로의 간단한 요약 정보 반환
4
5 Param
6 - String : 경로 ID
7 Return
8 - RouteSumInfo : 경로 요약 정보
```
```
1 fun getRoutePtInfo(routeID: String, ptType: ROUTEPTTYPE): RoutePtItem
```

## f. getRoutePtViaInfo

## g. getRoutePtRemainViaInfo

## h. getRouteLinePoints

## i. cancelRoute

## j. onOptimalRoute

### 2

```
3 Description : 경로의 출발지 / 목적지 정보 반환
4
5 Param
6 - routeID = 경로 ID
7 - ptType = 지점 타입
8 Return
9 - RoutePtItem : 지점 정보
```
```
1 fun getRoutePtViaInfo(routeID: String, viaIndex: Int): RoutePtItem
2
3 Description : 경로내 특정 경유지 정보 반환
4
5 Param
6 - routeID : 경로 ID
7 - viaIndex : 얻고자 하는 경유지의 순서
8 Return
9 - RoutePtItem : 경유지 정보
```
```
1 fun getRoutePtRemainViaInfo(): List<RoutePtItem>?
2
3 Description : 주행중인 경로의 지나가지 않은 경유지 정보 반환
4
5 Param : void
6 Return
7 - List<RoutePtItem> : 지나가지 않은 경유지 정보
```
```
1 fun getRouteLinePoints(routeID: String): JSONArray
2
3 Description : 경로 Line 좌표열 반환
4
5 Param
6 - routeID : 경로 ID
7 Return
8 - JSONArray : 경로 Line 좌표열
```
```
1 fun cancelRoute()
2
3 Description : 경로 취소
4
5 Param : void
6 Return : void
```
```
1 fun onOptimalRoute(start: RoutePtItem, goal: RoutePtItem, viaList: List<RoutePtItem>?,
2 optionType: List<ROUTEOPTIONTYPE>?, extraInfo: RouteExtraInfo?,
3 listener: OnRouteMultiListener)
4
5 Description: 길 찾기 ( 멀티 경로 최적지점탐색 ) 설정 한 목적지의 최적지점을 탐색하여
6 최적 입구점이 있는 경우 해당 위치로 변경하여 경로탐색
7
8 Param
9 - start = 출발지 정보
10 - goal = 목적지 정보
```

## 5. 주행

## a. runGuidance

## b. isSimulation

## c. startSimulation

## d. finishSimulation

## e. getRemainRouteInfo

```
11 - viaList = 경유지 리스트 ( 최대 100개 )
12 - optionType = 탐색 옵션 정보 ( Default 옵션 사용시 null 입력 )
13 - extraInfo = 부가정보 ( 필요없을시 null 입력 )
14 - listener = 탐색 결과( 경로 ID ) 리스트 반환
15 Return : void
```
```
1 fun runGuidance(routeID: String): Int
2
3 Description : 주행 시작
4 * 선택된 “경로 ID” 를 제외한 나머지 경로는 삭제 됨
5
6 Param
7 - routeID = 경로 ID
8 Return
9 - Int : 성공 여부 ( 0 : 성공 / 그 외 실패 )
```
```
1 fun isSimulation(): Boolean
2
3 Description : 모의 주행 여부 반환
4
5 Param : void
6 Return
7 - Boolean : 모의 주행 여부 ( true : 모의주행 중 / false : 모의주행 아님 )
```
```
1 fun startSimulation(routeID: String): Int
2
3 Description : 모의 주행 시작
4
5 Param
6 - routeID = 경로 ID
7 Return
8 - Int : 성공 여부 ( 0 : 성공 / 그 외 실패 )
```
```
1 fun finishSimulation(): Int
2
3 Description : 모의 주행 종료
4
5 Param : void
6 Return
7 - Int : 성공 여부 ( 0 : 성공 / 그 외 실패 )
```
```
1 fun getRemainRouteInfo(): RouteRemainInfo
2
3 Description : 주행중 남은거리/시간/요금 정보 반환
4 * 안내시작/모의주행 시작 이후 호출 필요
5
6 Param : void
7 Return
8 - RouteRemainInfo : 주행 남은거리/시간/요금
```

## f. getRemainViaRouteInfo

## g. getTotalRemainRouteInfo

## h. setGuidanceSettings

## i. getGuidanceSettings

## 6. 기타

## a. destroyNavi

## b. getNaviVersionName ( deprecated, 20/01/20 )

```
1 fun getRemainViaRouteInfo(): List<RouteViaRemainInfo>?
2
3 Description : 주행중 지나가지 않은 경유지의 남은거리/시간 정보 반환
4 * 안내시작 시작 이후 호출 필요
5
6 Param : void
7 Return
8 - RouteViaRemainInfo : 경유지의 남은거리/시간
```
```
1 fun getTotalRemainRouteInfo(routeID: String): RouteRemainInfo
2
3 Description : 경로의 총 거리/시간/요금 정보 반환
4 * 안내시작/모의주행 시작 전 호출 필요
5
6 Param
7 - routeID = 경로 ID
8 Return
9 - RouteRemainInfo : 총 남은거리/시간/요금
```
```
1 fun setGuidanceSettings(settings: List<GUIDANCESETTING>?)
2
3 Description : "안전운행정보 안내" 설정 변경
4
5 Param
6 - settings: List에 존재하는 값만 설정 On, 나머지 Off
7 * null 입력시 아이나비 Default 옵션 적용
8
9 Return : void
```
```
1 fun getGuidanceSettings(): List<GUIDANCESETTING>
2
3 Description : 현재 "안전운행정보 안내" 반환
4
5 Param : void
6 Return
7 - List<GUIDANCESETTING> : 현재 On 되어있는 설정 리스트
```
```
1 fun destroyNavi()
2
3 Description : SDK 메모리 해제 및 종료
4 * App 종료 시 호출 필요
5
6 Param : void
7 Return : void
```
```
1 fun getNaviVersionName(): String
2
3 Description : SDK 버전네임 반환
```

## c. getNaviVersionCode ( deprecated, 20/01/20 )

## d. getNaviSDKVersion

## e. setApplicationStatus

## f. setOrientation

## g. setNaviVolume

## h. getNaviVolume

### 4

```
5 Param : void
6 Return
7 - String : SDK 버전네임 ( ex “01.00.00” )
```
```
1 fun getNaviVersionCode(): Int
2
3 Description : SDK 버전코드 반환
4
5 Param : void
6 Return
7 - Int : SDK 버전코드
```
```
1 fun getNaviSDKVersion(): String
2
3 Description : SDK 버전 반환
4
5 Param : void
6 Return
7 - String : SDK 버전
```
```
1 fun setApplicationStatus(status: APPSTATUS)
2
3 Description : Application 상태 세팅 (Foreground, Background )
4
5 Param
6 - status = App 상태
7 Return : void
```
```
1 fun setOrientation(orientation: Int)
2
3 Description : 화면 가로/세로 상태 세팅
4
5 Param
6 - Int : 회전 상태 ( Default : Configuration.ORIENTATION_UNDEFINED )
7 -> 0 : Configuration.ORIENTATION_UNDEFINED ( 단말의 회전 상태 사용 )
8 -> 1 : Configuration.ORIENTATION_PORTRAIT ( 세로 상태 고정 )
9 -> 2 : Configuration.ORIENTATION_LANDSCAPE ( 가로 상태 고정 )
10 Return : void
```
```
1 fun setNaviVolume(vol: Float)
2
3 Description : 내비게이션 볼륨 세팅
4 * 단말기의 미디어 볼륨과는 별개로 내비게이션에서만 사용하는 음성
5
6 Param
7 - vol : 내비게이션 볼륨 ( 0.0 ~ 1.0 )
8 Return : void
```
```
1 fun getNaviVolume(): Float
```

## i. getCurrentPos

## j. setNaviEventListener

## k. setRouteChangedListener

## l. setDrivingStatusListener

## m. setCarSpeedListener

### 2

```
3 Description : 내비게이션 볼륨 반환
4 * 단말기의 미디어 볼륨과는 별개로 내비게이션에서만 사용하는 음성
5
6 Param : void
7 Return
8 - Float : 내비게이션 볼륨 ( 0.0 ~ 1.0 )
```
```
1 fun getCurrenPos(): NaviLocation
2
3 Description : 현재 위치 반환
4
5 Param : void
6 Return
7 - NaviLocation
```
```
1 fun setNaviEventListener(listener: OnNaviEventListener)
2
3 Description : 내비게이션 버튼 이벤트 Callback
4
5 Param
6 - listener : interface OnNaviEventListener {
7 fun onEvent(e: NaviEvent)
8 } = 버튼 이벤트 전달
9 Return : void
```
```
1 fun setRouteChangedListener(listener: OnRouteChangedListener)
2
3 Description : 주행 재탐색 성공 이벤트 Callback
4
5 Param
6 - listener : interface OnRouteChangedListener {
7 fun onChanged(routeID: String)
8 } = 새로운 경로 RouteID 전달
9 Return : void
```
```
1 fun setDrivingStatusListener(listener: OnDrivingStatusListener, nearGoalDist: Int)
2
3 Description : 주행 시작/도착 이벤트 및 목적지 도착시 요금 정보 Callback
4 * 목적지 도착시 요금은 도착이벤트 발생시에만 호출 됨
5 * 목적지 도착시 요금은 실 주행에서만 계산됨 (모의주행시 무조건 0원)
6 * 경유지 도착 알림 인덱스는 0부터 시작되며, 안내 시작 시 전달된 경유지 리스트의 순서와 동일하다.
7 * 만약 0번째 경유지 -> 2번째 -> 1번째 순서로 주행한다면 arrivalVia 이벤트도 0 -> 2 -> 1 순으로 전달
8 * 한번 지나간 경유지에 대해서 다시 onArrivalVia 이벤트가 호출되지는 않음
9
10 Param
11 - listener : interface OnDrivingStatusListener {
12 fun onStatus(status: DRIVINGSTATUS)
13 fun onArrivalFee(fee: Int)
14 fun onArrivalVia(nIndex: Int)
15 } = 주행 시작/종료 이벤트 전달 및 도착 후 통행요금, 경유지 도착 정보 전달
16 - nearGoalDist : NEARGOAL STATUS 체크 거리 ( 단위 : m, Default : 100m )
17 Return : void
```

## n. setCarType

## o. getCarType

## p. setTurnViewBackgroundColor

## q. getTurnViewBackgroundColor

## r. setNextTurnViewBackgroundColor

```
1 fun setCarSpeedListener(listener: OnCarSpeedListener)
2
3 Description : 차량 속도 Callback
4
5 Param
6 - listener : interface OnCarSpeedListener {
7 fun onSpeed(speed: Int)
8 } = 차량 속도 전달
9 Return : void
```
```
1 fun setCarType(nCarType : CARTYPE) {
2
3 Description : 차종 설정 (요금 및 경로 안내 시 반영)
4 * 차종 설명은 CARTYPE 참조
5
6 Param
7 - nCarType = 차종
8 Return : void
```
```
1 fun getCarType() : CARTYPE {
2
3 Description : 현재 설정된 차종 반환
4
5 Param : void
6 Return : CARTYPE
```
```
1 fun setTurnViewBackgroundColor(strColor : String) : Boolean
2
3 Description : 차기 turnview 배경색 변경
4
5 /* 사용 가능한 색상명
6 red, blue, green, black, white, gray, cyan, magenta, yellow,
7 lightgray, darkgray, grey, lightgrey, darkgrey, aqua,
8 fuchsia, lime, maroon, navy, olive, purple, silver, teal.
9 */
10
11 Param : strColor = 16진수 컬러값 또는 색상명 (#RRGGBB, #AARRGGBB, "red", "black" ..)
12 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
13 Return : 배경색 적용 여부
```
```
1 fun getTurnViewBackgroundColor() : String
2
3 Description : 현재 적용된 차기 turnview string 얻어오기
4
5 Param : void
6 Return : 배경색 문자열 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
```
```
1 fun setNextTurnViewBackgroundColor(strColor : String) : Boolean
2
3 Description : 차차기 turnview 배경색 변경
4
5 Param : strColor = 16진수 컬러값 또는 색상명 (#RRGGBB, #AARRGGBB, "red", "black" ..)
6 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
```

## s. getNextTurnViewBackgroundColor

## t. setArrivalViewBackgroundColor

## u. getArrivalViewBackgroundColor

## v. resetTurnViewsBackgroundColor

## w. setVisibleExtendView

## x. getVisibleExtendView

## y. setDrawBackgroundTBT

```
7 Return : 배경색 적용 여부
```
```
1 fun getNextTurnViewBackgroundColor() : String
2
3 Description : 현재 적용된 차차기 turnview string 얻어오기
4
5 Param : void
6 Return : 배경색 문자열 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
```
```
1 fun setArrivalViewBackgroundColor(strColor : String) : Boolean
2
3 Description : 목적지 도착 view 배경색 변경
4
5 Param : strColor = 16진수 컬러값 또는 색상명 (#RRGGBB, #AARRGGBB, "red", "black" ..)
6 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
7 Return : 배경색 적용 여부
```
```
1 fun getArrivalViewBackgroundColor() : String
2
3 Description : 목적지 도착 view 배경색 string 얻어오기
4
5 Param : void
6 Return : 배경색 문자열 e.g) "#f21e55f7", "#1e55f7", "red" , "black"
```
```
1 fun resetTurnViewsBackgroundColor()
2
3 Description : 차기, 차차기, 목적지 도착 view 배경색을 아래 기본값으로 초기화
4 TURN("#f21e55f7") // 차기
5 NEXT_TURN("#f2122672") // 차차기
6 ARRIVAL("#f21e55f7") // 목적지 도착
7
8 Param : void
9 Return : void
```
```
1 fun setVisibleExtendView(bIsShow : Boolean)
2 * 확대도는 모의주행/안내시작 후 표출
3 Description : 확대도 표출 여부 설정
4 Param : bIsShow = 표출 여부 (true = 표출, false = 표출 안함[Default])
5 Return : void
```
```
1 fun getVisibleExtendView() : Boolean
2
3 Description : 적용된 확대도 표출 여부
4 Param : void
5 Return : 표출 여부
```
```
1 fun setDrawBackgroundTBT(bisDrawBackgroundTBT : Boolean)
2 * 백그라운드 TBT View는 '안내시작' 상태일때 만 표출
```

## z. getDrawBackgroundTBT

## aa. forceHideBackgroundTBT

## ab. setBringToFrontListener

## ac. setLowResolution

## 7. 화물차 옵션

## a. setCarHeight

## b. getCarHeight

## c. setCarWeight

```
3 Description : 백그라운드 TBT View 표출 설정 여부
4 Param : bIsUseLowResolution = 설정여부 (true = 저해상도 모드 강제 적용, false = 적용 안함 [Default])
5 Return : void
```
```
1 fun getDrawBackgroundTBT() : Boolean
2
3 Description : 백그라운드 TBT View 표출 설정 여부
4 Param : void
5 Return : 설정여부 (true = 표출, false = 미표출 [Default])
```
```
1 fun forceHideBackgroundTBT()
2
3 Description : 백그라운드 TBT 강제 숨김처리
4 Param : void
5 Return : void
```
```
1 fun setBringToFrontListener(listener: OnBringToFrontListener)
2
3 Description : 백그라운드 TBT 클릭 이벤트 리스너 설정
4 Param : bIsUseLowResolution = 설정여부 (true = 저해상도 모드 강제 적용, false = 적용 안함 [Default])
5 Return : void
```
```
1 fun setLowResolution(bIsUseLowResolution : Boolean)
2
3 Description : 저해상도 단말 강제 설정 여부
4 Param : bIsUseLowResolution = 설정여부 (true = 저해상도 모드 강제 적용, false = 적용 안함 [Default])
5 Return : void
```
```
1 fun setCarHeight(nHeight: Int) : Boolean
2
3 Description : 차량 높이 설정 (cm), 설정 시 높이제한구역 회피안내
4
5 Param
6 - nHeight = 차량 높이 설정 (cm) // 0 ~ 1000 [10m]
7 Return : 설정값 적용 성공 여부 (true/false)
```
```
1 fun getCarHeight() : Int
2
3 Description : 현재 설정된 차량 높이값 반환 (default : 0)
4
5 Param : void
6 Return : 차량 높이(cm)
```
```
1 fun setCarWeight(nWeight: Int) : Boolean
2
3 Description : 차량 중량 설정 (kg) , 설정 시 중량제한구역 회피안내
```

## d. getCarWeight

## e. setAvoidUturn

## f. getAvoidUturn

## g. setAvoidNarrowRoad

## h. getAvoidNarrowRoad

## i. setAvoidRestriction

### 4

```
5 Param
6 - nWeight = 차량 중량 설정 (kg) // 0 ~ 60000 [60t]
7 Return : 설정값 적용 성공 여부 (true/false)
```
```
1 fun getCarWeight() : Int
2
3 Description : 현재 설정된 차량 중량값 반환 (default : 0)
4
5 Param : void
6 Return : 차량 중량(kg)
```
```
1 fun setAvoidUturn(nAvoidUturn : Int) : Boolean
2
3 Description : 왕복 n차선 이하 유턴 회피 설정
4
5 Param
6 - nAvoidUturn = 차선
7 Return : 설정값 적용 성공 여부 (true/false)
```
```
1 fun getAvoidUturn() : Int
2
3 Description : 현재 설정된 유턴회피 차선 반환 (default : 0)
4
5 Param : void
6 Return : 차선 정보
7
```
```
1 fun setAvoidNarrowRoad(nAvoidNarrowRoad : Int) : Boolean
2
3 Description : 왕복 n차선 이하 도로 회피여부 설정
4
5 Param
6 - nAvoidNarrowRoad = 차선
7 Return : 설정값 적용 성공 여부 (true/false)
```
```
1 fun getAvoidNarrowRoad() : Int
2
3 Description : 현재 설정된 n차선 이하 도로 회피여부 (default : 0)
4
5 Param : void
6 Return : 차선 정보
```
```
1 fun setAvoidRestriction(bIsAvoidRestriction : Boolean)
2
3 Description : 화물차 통행제한구간 회피여부 설정
4
5 Param
6 - bIsAvoidRestriction = 회피여부 (true = 구간 회피 , false : 구간 회피 안함)
7 Return : void
```

## j. getAvoidRestriction

## k. getNearestVertexIndex

## l. getZoneLimit

## m. setZoneLimit

## n. getAvoidEvasion

## o. setAvoidEvasion

# SDK Interface Reference

## 1. OnNaviInitListener

```
1 fun getAvoidRestriction() : Boolean
2
3 Description : 현재 설정된 화물차 통행제한구간 회피여부 (default : false)
4
5 Param : void
6 Return : 설정된 통행제한구간회피 여부
```
```
1 fun getNearestVertexIndex() : Int
2
3 Description : 현위치에서 진행방향으로 탐색 좌표리스트 내 가장 가까운 좌표 인덱스 반환
4
5 Param : void
6 Return : 가장 가까운 좌표 인덱스
```
```
1 fun getZoneLimit() : Boolean
2
3 Description : 현재 설정된 상수원보호구역 탐색 회피여부 (default : false)
4
5 Param : void
6 Return : 설정된 상수원보호구역 안내 회피 여부
```
```
1 fun setZoneLimit(bIsAvoidZoneLimit : Boolean)
2
3 Description : 상수원보호구역 회피 여부 설정
4
5 Param
6 - bIsAvoidZoneLimit = 회피여부 (true = 구간 회피 , false : 구간 회피 안함)
7 Return : void
```
```
1 fun getAvoidEvasion() : Boolean
2
3 Description : 현재 설정된 위수지역 회피여부 (default : false)
4
5 Param : void
6 Return : 설정된 위수지역 안내 회피 여부
```
```
1 fun setAvoidEvasion(bIsSetEvasion : Boolean)
2
3 Description : 위수지역 회피 여부 설정
4
5 Param
6 - bIsAvoidEvasion = 회피여부 (true = 구간 회피 , false : 구간 회피 안함)
7 Return : void
```

## 2. OnNaviEventListener

## 3. OnMapClickListener

## 4. OnMapMoveChangedListener

## 5. OnSearchListener

## 6. OnRecommendWordListener

## 7. OnRouteMultiListener

## 8. OnRouteSingleListener

```
1 interface OnNaviInitListener {
2 fun onSuccess()
3 fun onFail(errCode: Int, errMsg: String)
4 }
5
```
```
1 interface OnNaviEventListener {
2 fun onEvent(e: NaviEvent)
3 }
4
```
```
1 interface OnMapClickListener {
2 fun onMapLongClick(lat: Double, lon: Double)
3 }
4
```
```
1 interface OnMapMoveChangedListener {
2 fun onStart()
3 fun onStop()
4 }
5
```
```
1 interface OnSearchListener {
2 fun onSuccess(result: SearchResult)
3 fun onFail(errCode: Int, errMsg: String)
4 }
5
```
```
1 interface OnRecommendWordListener {
2 fun onSuccess(result : ArrayList<RecommendWord>)
3 fun onFail(errCode: Int, errMsg: String)
4 }
5
```
```
1 interface OnRouteMultiListener {
2 fun onSuccess(result: ArrayList<String>, same: Boolean)
3 fun onFail(errCode: Int, msg: String)
4 }
5
```
```
1 interface OnRouteSingleListener {
2 fun onSuccess(result: String)
3 fun onFail(errCode: Int, msg: String)
4 }
5
```

## 9. OnReRouteResultListener

## 10. OnRouteChangedListener

## 11. OnDrivingStatusListener

## 12. OnCarSpeedListener

## 13. OnBringToFrontListener

# SDK Structure Reference

## 1. NaviLocation

## 2. SearchResult

## 3. SearchItem

```
1 interface OnReRouteResultListener {
2 fun onSuccess(result: String)
3 fun onFail(errCode: Int, msg: String)
4 }
5
```
```
1 interface OnRouteChangedListener {
2 fun onChanged(routeID: String)
3 }
4
```
```
1 interface OnDrivingStatusListener {
2 fun onStatus(status: DRIVINGSTATUS)
3 fun onArrivalFee(fee: Int)
4 fun onArrivalVia(nIndex: Int) // v0.0.29 부터 추가
5 }
6
```
```
1 interface OnCarSpeedListener {
2 fun onSpeed(speed: Int)
3 }
4
```
```
1 interface OnBringToFrontListener {
2 fun getBringToFrontPendingIntent(context: Context?): PendingIntent?
3 }
4
```
```
1 class NaviLocation {
2 var lat: Double // 위도
3 var lon: Double // 경도
4 var angle: Double // 정북 기준 각도(0.0 ~ 360.0): v0.0.20 부터 Double 사용, v0.0.19 까지는 Int 사용
5 var speed: Double // 속도
6 }
7
```
```
1 class SearchResult {
2 var query: String // 검색어
3 var items: ArrayList<SearchItem>? // 검색 결과 리스트
4 }
5
```

## 4. RecommendWord

## 5. RoutePtItem

## 6. RouteSumInfo

## 7. NaviEvent

## 8. RouteRemainInfo

## 9. RouteViaRemainInfo

```
1 class SearchItem {
2 var dpLat: Double // 지도 위치보기 시에 사용하는 위도 좌표
3 var dpLon: Double // 지도 위치보기 시에 사용하는 경도 좌표
4 var rpLat: Double // 길 찾기 시에 사용하는 위도 좌표
5 var rpLon: Double // 길 찾기 시에 사용하는 경도 좌표
6 var mainTitle: String // 검색 결과 항목 타이틀
7 var addrJibun: String // 검색 결과 지번 주소
8 var addrRoad: String // 검색 결과 도로명 주소
9 var distane: Int // 검색에 사용했던 기준좌표와의 거리
10 }
11
```
```
1 class RecommendWord {
2 var recommendWord: String // 추천어
3 var frequency: Int // 추천어 조회 빈도 수
4 }
5
```
```
1 class RoutePtItem {
2 var name: String // 지점 명칭
3 var rpLat: Double // 길 찾기 시에 사용하는 위도 좌표
4 var rpLon: Double // 길 찾기 시에 사용하는 경도 좌표
5 var dpLat: Double // 지도 위치보기 시에 사용하는 위도 좌표
6 var dpLon: Double // 지도 위치보기 시에 사용하는 경도 좌표
7 var angle: Int // 길 찾기 시에 사용하는 각도 ( 0 ~ 359 )
8 }
9
```
```
1 class RouteSumInfo {
2 var optionName: String // 길찾기 시에 사용된 옵션 명칭
3 var dist: String // 경로 총 거리
4 var time: String // 목적지 도착 예정 시간
5 var fee: String // 총 톨게이트 요금 정보
6 }
7
```
```
1 class NaviEvent {
2 var eventType: [NAVIEVENTTYPE] // 이벤트 타입
3 }
4
```
```
1 class RouteRemainInfo {
2 var remainTime:Int // 목적지 까지 남은 시간 ( '초' 단위 )
3 var remainDist:Int // 목적지 까지 나은 거리 ( 'm' 단위 )
4 var remainFee:Int // 목적지 까지 남은 요금 ( '원' 단위 ), 요금 계산 실패시 -1
5 }
6
```
```
1 class RouteViaRemainInfo {
2 var remainTime: Int // 경유지 까지 남은 시간 ( '초' 단위 )
```

## 10. RouteExtraInfo

# SDK Define Reference

## 1. MAPVIEWMODE

## 2. ICONGRAVITY

## 3. MAPFONTSIZETYPE

## 4. MAPDAYNIGHTMODE

## 5. ROUTEPTTYPE

## 6. APPSTATUS

```
3 var remainDist: Int // 경유지 까지 남은 거리 ( 'm' 단위 )
4 }
5
```
```
1 class RouteExtraInfo {
2 var baseURL: String //부가정보 외부연동 URL
3 }
4
```
```
1 enum class MAPVIEWMODE {
2 VIEWMODE_3D, // 3D 뷰
3 VIEWMODE_2D, // 2D 회전 뷰
4 VIEWMODE_2D_FIX // 2D 고정 뷰 ( 지도가 정북 고정 )
5 }
6
```
```
1 enum class ICONGRAVITY {
2 CENTER, // 이미지 정중앙이 MapIcon 좌표 위치
3 CENTER_TOP, // 이미지의 정중앙 하단이 MapIcon 좌표 위치 ( 좌표를 중심으로 이미지를 상단으로 이동 )
4 LEFT_TOP, // 이미지의 우측하단 좌표가 MapIcon 좌표 위치 ( 좌표를 중심으로 이미지를 좌측 상단으로 이동 )
5 RIGHT_TOP, // 이미지의 좌측하단 좌표가 MapIcon 좌표 위치 ( 좌표를 중심으로 이미지를 우측 상단으로 이동 )
6 LEFT_BOTTOM, // 이미지의 우측상단 좌표가 MapIcon 좌표 위치 ( 좌표를 중심으로 이미지를 좌측 하단으로 이동 )
7 RIGHT_BOTTOM // 이미지의 좌측상단 좌표가 MapIcon 좌표 위치 ( 좌표를 중심으로 이미지를 우측 하단으로 이동 )
8 }
9
```
```
1 enum class MAPFONTSIZETYPE {
2 NORMAL, // 기본 사이즈
3 LARGE // 확대 사이즈
4 }
5
```
```
1 enum class MAPDAYNIGHTMODE {
2 AUTO, // 시간대별 주/야 자동 변경
3 ALWAYSDAY, // 항상 주간 지도
4 ALWAYSNIGHT // 항상 야간 지도
5 }
6
```
```
1 enum class ROUTEPTTYPE {
2 START, // 출발지
3 GOAL // 목적지
4 }
5
```

## 7. NAVIEVENTTYPE

## 8. DRIVINGSTATUS

## 9. ROUTEOPTIONTYPE

## 10. MAPCOMPONENT

```
1 enum class APPSTATUS {
2 BACKGROUND, // App 이 Background 상태
3 SCREEN_OFF_BACKGROUND, // 스크린 화면이 꺼진 상태
4 FOREGROUND // App 이 Foreground 상태
5 }
6
```
```
1 enum class NAVIEVENTTYPE {
2 NONE, // 없음
3 MAINMENU, // 하단바 좌측, 메인메뉴 버튼
4 MULTIMENU, // 하단바 우측, 멀티메뉴 버튼
5 EXITAPPLICATION, // 목적지 도착 하단바, 앱 종료 버튼
6 VOLUMEMAPBUTTON, // 지도이동시 볼륨 버튼
7 CURRRENTPOSITION, // 지도이동시 현위치로 버튼
8 ALLROUTEVIEW // 전체경로보기
9 }
10
```
```
1 enum class DRIVINGSTATUS {
2 START, // 주행 시작
3 NEARGOAL, // 목적지 근처 ( 목적지 근처 대략 100m 부근 )
4 ARRIVAL // 주행 완료
5 }
6
```
```
1 enum class ROUTEOPTIONTYPE {
2 TIMEPRIOTY, // 빠른길
3 RECOMMEND, // 추천길
4 FREEROAD, // 무료길
5 BEGINNER, // 편한길
6 MOTOCYCLE, // 이륜차
7 HIGHWAYPRIOTY, // 고속도로우선
8 DISTANCEPRIOTY, // 최단거리
9 * 0.0.27 화물차 전용 옵션 추가
10 TRUCK, // 실시간만차
11 TRUCK_FREEROAD, // 실시간만차(무료)
12 TRUCK2, // 실시간공차
13 TRUCK2_FREEROAD, // 실시간공차(무료)
14 TRUCK_NATIONALWAY, // 국도만차
15 TRUCK2_NATIONALWAY, // 국도공차
16 }
17
```
```
1 enum class MAPCOMPONENT {
2 ALL_COMPONENT, // 모든 지도 컴포넌트 (아래 모든 항목을 한번에 처리할때 사용)
3 ANGLE_BTN, // 나침반 버튼 (지도 이동시)
4 CUR_ON_BTN, // 현위치로 버튼 (지도 이동시)
5 ZOOM_IN_OUT_BTN, // 확대/축소 버튼 (지도 이동시)
6 BOTTOM_NORMAL_VIEW, // 지도 하단 뷰 (경로 없는 경우)
7 BOTTOM_DRIVING_VIEW, // 지도 하단 뷰 (경로 존재 하는 경우)
8 TOP_ARRIVAL_VIEW, // 목적지 도착 상단 뷰
9 BOTTOM_ARRIVAL_VIEW, // 목적지 도착 하단 뷰
10 ROUTE_TRAFFIC_STATUS_BAR, // 주행중 우측 교통정보 바
11 BOTTOM_NORMAL_SIDE_BUTTON, // 지도 하단 뷰 버튼 (경로 없는 경우)
12 BOTTOM_DRIVING_SIDE_BUTTON, // 지도 하단 뷰 버튼 (경로 존재 하는 경우)
```

## 11. MAPSTYLE ( deprecated, v0.9.0 )

## 12. GUIDANCESETTING

## 13. MAPROUTECOLOR

## 14. CARTYPE

### 13 BOTTOM_ARRIVAL_LEFT_BUTTON // 목적지 도착 하단바 좌측 버튼

### 14 }

### 15

```
1 enum class MAPSTYLE {
2 DEFAULT, // 아이나비 지도
3 MAPBOX // Mapbox Style 지도
4 }
5
```
```
1 enum class GUIDANCESETTING {
2 MOVE_OVERSPEED, // 이동식 과속 단속 카메라 주의안내
3 MOVE_BOX_OVERSPEED, // 박스형 과속 단속 카메라 주의안내
4 INTERRUPT, // 끼어들기 단속 주의안내
5 OVERLOAD, // 과적단속 주의안내
6 FIX_TRAFFIC, // 교통정보수집 카메라 안내
7 CURVE, // 급커브 구간 주의안내
8 ACCIDENT, // 사고다발 구간 주의안내
9 SPEED_BUMP, // 과속방지턱 주의안내
10 SCHOOL_ZONE, // 스쿨존/실버존 주의안내
11 WILDANIMAL, // 야생동물 출현 주의안내
12 TRAIN_TRACK, // 철도건널목 주의안내
13 ROAD_DROP, // 낙석구간 주의안내
14 GREEN_AREA // 녹색교통지역 진입 안내
15 }
16
```
```
1 enum class MAPROUTECOLOR {
2 TRAFFIC, // 실시간 교통정보
3 RED, // 빨간색
4 ORANGE, // 주황색
5 YELLOW, // 노란색
6 GREEN, // 초록색
7 BLUE, // 파란색 ( Default )
8 INDIGO // 군청색
9 }
10
```
```
1 enum class CARTYPE(val value : Int){
2 TYPE_1(0), // "1종(소형차)" -> "일반승용, 승합16인 이하, 화물2.5톤 미만",
3 TYPE_2(1), // "2종(중형차)" -> "승합32인 이하, 화물5.5톤 이하",
4 TYPE_3(2), // "3종(대형차)" -> "승합33인 이상, 화물10톤 미만",
5 TYPE_4(3), // "4종(대형화물차)" -> "화물20톤 미만"
6 TYPE_5(4), // "5종(특수화물차)" -> "화물20톤 이상"
7 TYPE_6(5), // "경차(1종 : 통행료 할인 적용)",
8 TYPE_7(6); // "이륜차",
9
10 companion object {
11 fun from(findValue: Int): CARTYPE = values().first { it.value == findValue }
12 fun getTitle(value : CARTYPE): String = when(value){
13 TYPE_1 -> {"1종(소형차)"}
14 TYPE_2 -> {"2종(중형차)"}
15 TYPE_3 -> {"3종(대형차)"}
16 TYPE_4 -> {"4종(대형화물차)"}
17 TYPE_5 -> {"5종(특수화물차)"}
18 TYPE_6 -> {"경차"}
```

# 코드 표

### 19 TYPE_7 -> {"이륜차"}

### 20 }

```
21 fun getDescription(value : CARTYPE): String = when(value){
22 TYPE_1 -> {"일반승용, 승합16인 이하, 화물2.5톤 미만"}
23 TYPE_2 -> {"승합32인 이하, 화물5.5톤 이하"}
24 TYPE_3 -> {"승합33인 이상, 화물10톤 미만"}
25 TYPE_4 -> {"화물20톤 미만"}
26 TYPE_5 -> {"화물20톤 이상"}
27 TYPE_6 -> {"1종 : 통행료 할인 적용"}
28 TYPE_7 -> {""}
29 }
30 }
31 }
32
```
## 0 성공

## 1 길찾기 실패

## 3 목적지가 물리적 섬 도로

## 4 유효하지 않은 출발지

## 5 유효하지 않은 목적지

## 9 요청 파라미터 오류

## 11 메모리 할당 실패

## 15 파일 오픈 실패

## 17 메모리 할당 실패

## 19 파일 읽기 실패

## 20 파일 쓰기 실패

## 21 유효하지 않은 지도 데이터

## 22 요청 파라미터 오류

## 23 Projection 실패

## 25 DB 오류

## 32 길찾기 가능 거리 초과

## 35 두 지점이 너무 가까운 경우

## 코드 값 설명


## 36 목적지 오류

## 39 논리적 길찾기 오류

## 43 차량이 진입할 수 없는 도로

## 48 소켓 연결 실패

## 49 결과 생성 실패

## 96 잘못된 경로 ID

## 97 Checksum 오류

## 120 최적경로 ( 재 탐색은 성공했으나, 더 좋은 경로가 없는 경

## 우 )

## 121 목적지 부근으로 재 탐색이 필요 없는 경우

## 300 미 지원 서비스

## 800 서버 파일 저장 에러

## 900 인증 실패

## 901 인증 정보가 변경되어 앱 재시작 필요

## 902 입력 파라미터 오류

## 903 조회결과 없음

## 904 존재하지 않는 파일 요청

## 905 DB 연동 에러

## 907 경로 ID 오류

## 931 유효하지 않은 좌표

## 933 유효하지 않은 검색어

## 1000 인증 데이터 오류

## 1001 인증 데이터 오류

## 1002 잘못된 요청 형식으로 인증

## 1003 인증 데이터가 존재하지 않음


## 1004 유효하지 않은 Unique Key ( 필수값인 Unique Key 값이

## Null 이거나 Empty 인 경우 )

## 1005 유효하지 않은 Unique Key ( 필수값인 Unique Key 값이

## 20자 초과 인 경우 )

## 2000 처리되지 않은 예외 발생

## 2001 유효하지 않은 출발지

## 2003 유효하지 않은 목적지

## 2006 서버 응답 오류

## 2007 버퍼 NULL

## 2008 데이터 파싱 실패

## 2010 패킷 생성 실패

## 2011 패킷 생성 실패

## 2012 다운로드 실패

## 2013 유효하지 않은 파라미터

## 3000 알 수 없는 인증 오류

## 3001 초기 지도 다운로드 실패

## 3002 초기 지도 다운로드 실패

## 3003 지도 URL 오류

## 3004 안전운행 URL 오류

## 3005 안전운행 URL 오류

## 3006 안전운행 다운로드 실패

## 3007 인증 실패

## 3008 인증 업데이트 실패

## 3050 지도 엔진 초기화 실패

## 3051 SMR 엔진 초기화 실패


## 3052 맵매칭 엔진 초기화 실패 ( 위치권한 미 획득시 에도 발생

## 할수 있음 )

## 3053 안내 엔진 초기화 실패

## 3054 기타 엔진 초기화 실패

## 4000 검색결과 없음

## 4001 유효하지 않은 검색어

## 5000 출발지 오류

## 5001 목적지 오류

## 5002 출발지가 유효 범위를 벗어난 경우

## 5003 목적지가 유효 범위를 벗어난 경우

## 5004 출발지와 목적지가 가까워 길찾기가 불가능

## 5005 안내중인 경로가 유효하지 않은 경우

## 6000 검색어 오류


