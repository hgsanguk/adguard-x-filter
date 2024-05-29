# AdGurard X Filter
X(구. 트위터) 웹 클라이언트의 불필요한 요소를 차단하여 서비스를 가볍게 이용할 수 있도록 하는 AdGuard 필터입니다. 특히 iOS, iPadOS 사용자가 광고를 차단하면서 네이티브 앱처럼 즐길 수 있는 PWA의 방해요소 필터링을 중점으로 합니다.

Android에선 [ReVanced](https://revanced.app/patches?pkg=com.twitter.android), PC에선 [Control Panel for Twitter](https://github.com/insin/control-panel-for-twitter)가 있으니, 타 플랫폼은 해당 애플리케이션 사용을 권장합니다.

## 종류
기본적으로 사용자가 X Premium을 결제할 의향이 없다는 가정 하에 제작되었습니다. 
* `filter.txt`: 기본 필터입니다. 무료 사용자에게 필요없는 X Premium 결제 유도만 제거합니다.
  * 메뉴(하단 바)의 Grok
  * 메뉴와 설정의 수익 창출
  * 메뉴와 설정의 X Premium
  * 내 프로필의 아티클과 하이라이트 탭
  * 내 프로필의 마음에 들어요 상단의 X Premium 안내
  * 인증된 사용자 프로필의 배지를 누르면 뜨는 X Premium 구독 버튼
  * 게시글 글자 제한 초과 시 X Premium 안내
  * 커뮤니티 우측 상단 커뮤니티 생성 버튼
* `filter-extra.txt`: 추가 필터입니다. 라이트한 사용자에게 필요없을 것으로 예상되는 요소를 제거합니다.
  * 메뉴의 채용
  * 메뉴의 광고(광고주의 광고 관리 페이지)
  * 내 게시글 우측 상단의 프로모션 버튼
  * 알림창의 인증됨 탭
  * 팔로잉/팔로워 목록의 인증된 팔로워, 구독(슈퍼 팔로잉) 탭
  * 설정의 크리에이터 구독
  * 프로필의 구독(슈퍼 팔로잉) 수
  * X Premium 사용자 프로필의 아티클과 하이라이트, 구독자용 탭
  * X Premium 사용자 프로필의 구독하기 버튼
  * 내 프로필의 Who to follow
  * 타임라인 추천 탭의 내가 팔로우하는 사람들의 메인 게시물, Who to follow, 추천 커뮤니티 등
  * 게시글 상세보기 최하단의 둘러보기(트윗 추천)

## 필터 링크
> [!NOTE]
> 기본 필터와 추가 필터는 각각 별개의 필터로, 추가 필터의 경우 기본 필터와 같이 사용해야 정상적으로 동작합니다.

**기본 필터**
```
https://raw.githubusercontent.com/hgsanguk/adguard-x-filter/main/filter.txt
```
**추가 필터**
```
https://raw.githubusercontent.com/hgsanguk/adguard-x-filter/main/filter-extra.txt
```

## 사용 방법
### iOS, iPadOS
1. App Store에서 [AdGuard](https://apps.apple.com/us/app/adguard-adblock-privacy/id1047223162)를 설치합니다.
2. 앱을 연 후 지시대로 Safari에서 AdGuard 확장 프로그램을 활성화합니다.
3. AdGuard에서 `보호 > Safari 보호 > 필터 > Custom`에서 스위치를 켜 활성화합니다.
4. 필터 추가를 누르면 나오는 입력 칸에 위에서 원하는 필터의 링크를 복사 후 붙여넣기 하고 다음을 누릅니다.
5. Safari로 [X](https://x.com)에 접속합니다.
6. Safari 주소창 하단, 중앙에 있는 옵션 버튼을 누르고 홈 화면에 추가를 누릅니다.
7. 원하는 이름을 지정하고 홈 화면에 X의 바로가기를 추가합니다.
8. 광고, Premium 결제 유도와 방해 요소가 없는 깔끔한 X를 즐기시기 바랍니다.
 
## 사용 시 주의 사항
### X PWA 자체의 문제점
PWA의 업데이트가 오랜 기간 없었으므로 아래의 문제는 X 측에서 해결할 가능성이 낮습니다. 이 점 참고하셔서, iOS 클라이언트를 보조로 사용하실 것을 권장합니다.
1. 스페이스 만들기가 불가능합니다. 참여는 가능합니다.
2. 사진의 저장이 불가능합니다.
3. 타래로 글을 이어나가게 되면 초안 저장이 불가능합니다. 단일 게시글만 초안 저장 가능합니다.
4. 초안을 불러온 뒤 게시글 수정을 하고 게시해도, 수정한 사안이 반영되지 않습니다.

### 필터의 문제점
1. 팔로잉/팔로워 목록의 '인증된 팔로워' 탭이 제거되더라도 팔로워를 누르면 기존대로 '인증된 팔로워' 페이지로 들어갑니다.

## 문의 및 오작동 제보
필터 관련 문의나 추가 차단 요소 제안은 필요시 스크린샷과 함께 issue를 열어주세요.
