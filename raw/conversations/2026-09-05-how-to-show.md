나는 **웹/앱 작품이라면 인터넷에 “작품 페이지를 공개한다”기보다, 하나의 서비스·기관·제품이 실제로 세상에 출시된 것처럼 공개하는 방식**이 가장 잘 맞는다고 생각해.

특히 OTHER GOODS나 LONGING 같은 경우에는 미술관식 소개 페이지보다 **관객이 설명 없이 실제 시스템에 접속해보는 것** 자체가 첫 감상이 되는 편이 훨씬 강할 것 같아.

### 내가 추천하는 공개 구조

```text
                     발견
        Instagram / YouTube / 링크 공유
                       ↓
              TENDER SYSTEMS
             institutional index
                       ↓
        ┌──────────────┴──────────────┐
        ↓                             ↓
   OTHER GOODS                    LONGING
   실제 쇼핑몰                     실제 터미널
   작품 = 웹서비스                 작품 = 웹앱
        ↓                             ↓
        └──────────────┬──────────────┘
                       ↓
              Archive / Research
             GitHub / Wiki / Docs
```

여기서 제일 중요한 것은 **TENDER SYSTEMS 사이트조차 일반적인 작가 포트폴리오처럼 만들지 않는 것**이야.

예를 들면 처음 방문했을 때:

```text
TENDER SYSTEMS

Systems for things that resist measurement.

ACTIVE SYSTEMS

OG-001 — OTHER GOODS
LN-001 — LONGING
```

정도만 보이고 각각 들어가면 바로 작품이 시작되는 거지.

---

## 1. 작품의 원본은 반드시 독립적인 웹사이트

이걸 가장 강하게 추천해.

`Instagram → 작품 소개 페이지 → 이미지 → 설명`

구조보다는

`Instagram → 링크 → 작품`

이어야 해.

예를 들어 OTHER GOODS 링크를 누르면 바로 상품 목록이 나오고,

LONGING 링크를 누르면 바로 가격, 차트, ticker, analyst report가 떠야 해.

**“이것은 인터랙티브 아트 프로젝트입니다”라는 설명을 먼저 읽게 하지 않는 것.**

관객이 처음 몇 초 동안 정말로,

> "뭐지? 진짜 쇼핑몰인가?"

혹은

> "이런 시장이 실제로 있는 건가?"

라고 생각할 수 있어야 해.

이 몇 초의 불확실성이 작품의 일부가 될 수 있어.

---

## 2. 그래서 App Store 앱은 기본적으로 권하지 않아

네 작업은 일단 **Web-first**가 더 좋아 보여.

App Store / Play Store로 가면 설치라는 장벽이 생기고, 관객은 처음부터 이것을 **“앱”이라는 제품 카테고리**로 인식하게 된다.

반면 웹은 링크 하나로 바로 들어갈 수 있다.

특히 작품이

* 데이터가 계속 변하고
* URL을 공유할 수 있고
* 웹 인터페이스 자체가 작품이고
* 다른 사람이 발견해서 바로 경험해야 한다면

웹이 훨씬 자연스럽다.

정말 카메라, GPS, Bluetooth, LiDAR, push notification처럼 **휴대폰의 native capability 자체가 작품의 중요한 재료**가 될 때 앱을 고려하면 돼.

---

# 3. 공개할 때도 '전시 오픈'보다 '서비스 런칭'처럼

이건 TENDER SYSTEMS에서 굉장히 중요한 미학이 될 수 있다고 생각해.

예를 들어 OTHER GOODS를 공개하면서

> My new interactive artwork OTHER GOODS is now online.

이라고 하지 않고,

그냥 TENDER SYSTEMS 계정에서

> **OG-001 — OTHER GOODS**
> Now available.

정도로 공개하는 거야.

LONGING도

> **LN-001 — LONGING**
> Market open.

같은 식으로.

작가의 감상을 대신 설명하지 않는다.

### 작품 내부에서도 마찬가지

OTHER GOODS:

```text
OTHER GOODS

A store for other kinds of goods.

SHOP
```

LONGING:

```text
LONGING

Research on changing values.

MARKETS OPEN
```

그리고 그냥 작동한다.

이 정도면 충분할 수도 있어.

---

# 4. 대신 작품 바깥에는 두 번째 레이어가 필요해

여기서 약간 역설적인데,

**작품을 설명하지 않는 것과 작품에 대한 기록을 남기지 않는 것은 전혀 다른 문제야.**

작품 안에서는 설명을 최소화하고,

작품 밖에서는 아주 철저하게 기록하는 것을 추천해.

그래서 두 층으로 분리하면 좋아.

### Public experience

```text
othergoods.[domain]
longing.[domain]
```

관객용.

설명 거의 없음.

### Archive / Documentation

```text
TENDER SYSTEMS
Archive
Research
System Notes
```

여기에는 나중에

* 작품명
* 연도
* 버전
* URL
* screenshots
* screen recording
* 작품 설명
* conceptual statement
* system architecture
* 데이터 출처
* AI 사용 방식
* 전시 이력
* 업데이트 로그

등을 남길 수 있어.

지금 구축하고 있는 GitHub Wiki가 이 역할에는 상당히 잘 맞아.

다만 **GitHub를 일반 관객의 첫 번째 입구로 만들지는 않는 것**을 추천해.

---

# 5. Instagram / YouTube는 '작품 게시 공간'이 아니라 발견 장치

이미 만든 계정들도 이 관점에서 운영하면 굉장히 명확해진다.

OTHER GOODS Instagram에 작품 설명을 장문으로 쓰기보다는 상품이 진짜 존재하는 것처럼 보여주는 거야.

예를 들어:

```text
OG-004

June 13,
4:03 PM

Sunlight through the window.
```

상품 사진.

가격.

그리고 URL.

LONGING이면 실제 금융 계정처럼:

```text
LN:HNWRT

12.83 ↓ 3.2%

Handwritten Letter
52W LOW
```

같은 게시물.

그리고 갑자기 analyst report가 하나 올라오고.

이렇게 하면 **SNS 자체도 작품 세계관의 surface**가 된다.

YouTube도 작품 설명 영상보다 처음에는

* OTHER GOODS 광고
* LONGING market update
* quarterly report
* analyst interview
* institutional announcement

처럼 운영하는 편이 훨씬 재미있어.

그걸 보고 링크를 타고 웹으로 들어오게 만드는 거지.

---

# 6. 그리고 외부 미술/디자인 세계에는 별도로 배포

자체 사이트만 만들면 작품은 존재하지만 **발견되기가 어렵다.**

그래서 작품을 완성한 다음 외부의 여러 생태계에 던져볼 가치가 있어.

### 디지털 아트 쪽

**New Art City**는 현재도 browser 기반 digital art 전시를 위한 artist-run 플랫폼을 운영하고 있고, 별도 설치나 로그인 없이 웹과 모바일에서 전시를 경험할 수 있다. 다만 3D 가상 갤러리 성격이 강해서, 나는 작품의 **본체를 여기에 옮기기보다는 특별전/그룹전 참가용**으로 생각하겠어. ([Newart City][1])

**Rhizome ArtBase**는 net art 보존의 중요한 아카이브지만 현재는 누구나 상시 제출하는 구조가 아니라 invitation과 periodic targeted open call 중심이다. 따라서 당장 배포 채널이라기보다는 **장기적으로 작품이 들어가면 의미 있는 아카이브**라고 보는 편이 정확하다. ([Artbase][2])

### 웹/인터랙션 디자인 쪽

오히려 나는 여기를 꽤 중요하게 볼 것 같아.

**FWA**는 지금도 FWA of the Day를 운영하면서 experimental/interactive digital experience를 선정하고 있다. ([FWA Wire][3])

**Awwwards** 역시 `Experimental`, `Web & Interactive`, `Mobile & Apps`, `Art & Illustration` 등의 분류로 웹사이트를 받고 있다. ([Awwwards][4])

여기서 재미있는 점이 있어.

TENDER SYSTEMS 작품은

> **미술계 + creative coding계 + web design계**

세 군데에 동시에 걸칠 가능성이 있어.

나는 일부러 하나를 선택하지 않는 게 좋다고 생각해.

---

# 7. 오프라인에 전시되더라도 '웹사이트를 보여주는 모니터'가 되면 아쉬워

나중에 전시 기회가 생긴다면,

```text
모니터
↓
웹사이트
↓
마우스
```

만 두는 건 피하고 싶어.

웹에 존재하던 **system이 현실 공간으로 침투한 것처럼** 보여주는 편이 훨씬 재미있어.

예를 들어 OTHER GOODS라면:

```text
       OTHER GOODS

   ┌─────────────────┐
   │   쇼핑몰 화면     │
   └─────────────────┘

         Receipt
         Catalog
      Shipping Label
       Product Card
```

관객이 주문하면 실제 receipt가 나온다든지.

LONGING이면 Bloomberg terminal처럼 실제 키보드와 여러 디스플레이를 배치하고

```text
LONGING MARKET TERMINAL
```

이 되어버리는 식.

즉,

**Web → Exhibition adaptation**

이지,

**Web을 전시장 모니터에 띄움**

이 아닌 거야.

---

# 8. 공개 시점도 작품의 일부로 만들 수 있어

이건 특히 추천하고 싶다.

모든 것을 완성해서 한꺼번에 공개할 필요가 없어.

TENDER SYSTEMS라는 기관이 실제로 **systems를 하나씩 가동시키는 것처럼** 하면 된다.

예를 들어:

```text
2026

TENDER SYSTEMS
established

        ↓

OG-001
OTHER GOODS
System Online

        ↓

상품 12개

        ↓

상품 30개

        ↓

LN-001
LONGING
Research Begins

        ↓

LONGING Market Open

        ↓

First Analyst Report

        ↓

Market event
```

이렇게 시간이 흐르면서 세계가 만들어진다.

그러면 **작품을 만드는 과정과 작품을 공개하는 과정이 분리되지 않는다.**

---

# 내가 지금이라면 이렇게 할 것 같아

**1단계**

TENDER SYSTEMS의 아주 작은 institutional website를 만든다.

```text
TENDER SYSTEMS

Systems for things that resist measurement.

ACTIVE SYSTEMS

OG-001 — OTHER GOODS
LN-001 — LONGING
```

그 이상 거의 없음.

**2단계**

OTHER GOODS를 완전히 독립적인 URL에서 실제 commerce처럼 공개한다.

설명하지 않는다.

**3단계**

TENDER SYSTEMS와 OTHER GOODS의 SNS에 상품을 하나씩 공개한다.

사이트 방문을 유도한다.

**4단계**

LONGING을 별도의 시스템으로 launch한다.

OTHER GOODS와 디자인은 달라도 **같은 기관에서 만들어졌다는 이상한 공통성**만 존재하게 한다.

**5단계**

어느 정도 작품이 축적되고 사람들이 경험하기 시작한 뒤에야 TENDER SYSTEMS Archive를 만든다.

그곳에서 작품의 배경과 research를 조금 더 볼 수 있게 한다.

**6단계**

그다음 FWA/Awwwards 같은 interactive web 분야와, New Art City·Rhizome·각종 new-media open call 같은 미술 분야를 **동시에 공략**한다.

---

그리고 이 구조가 지금까지 이야기했던 TENDER SYSTEMS의 정체성과도 꽤 잘 맞는다.

**작가 → 작품 → 관객**

보다

**TENDER SYSTEMS → System → Public**

이라는 관계를 만드는 거야.

그래서 관객 입장에서 처음 만나는 것은 **“누가 만든 예술작품”이 아니라 “인터넷 어딘가에 실제 존재하고 있는 이상한 시스템”**이다.

나는 이게 웹을 기반으로 작업한다는 것을 가장 적극적으로 활용하는 공개 방식이라고 생각해. 단순히 웹을 작품을 담는 매체로 사용하는 게 아니라, **웹에 존재한다는 사실 자체를 작품의 fiction과 현실 사이의 경계로 사용하는 것**이니까.

[1]: https://www.newart.city/join?utm_source=chatgpt.com "Join New Art City"
[2]: https://artbase.rhizome.org/wiki/FAQ?utm_source=chatgpt.com "FAQ - Rhizome Artbase"
[3]: https://www.thefwa.net/?utm_source=chatgpt.com "FWA Wire — winners' newswire"
[4]: https://www.awwwards.com/websites/art/?utm_source=chatgpt.com "Awwwards Nominees"
