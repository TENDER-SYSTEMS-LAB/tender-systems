# 애플 디자인 적용 비교

**User:** Anonymous  
**Created:** 9/4/2026 23:39:18  
**Updated:** 9/4/2026 23:40:27  
**Exported:** 9/5/2026 2:51:21  
**Link:** [https://chatgpt.com/g/g-p-6a9a975d22648191a192c2e4c5b4a3de/c/6a9ad810-48c0-83ee-b0ff-837a69583b9b](https://chatgpt.com/g/g-p-6a9a975d22648191a192c2e4c5b4a3de/c/6a9ad810-48c0-83ee-b0ff-837a69583b9b)  

## Prompt:
2026. 9. 4. 오후 11:39:06

https://github.com/dickwu/apple-design-skill 여기에 있는 애플 디자인 스킬을 사용해서 우리의 작품들에 적용하면 좀 별로일까?

## Response:
2026. 9. 4. 오후 11:39:17

링크의 스킬이 실제로 어떤 원칙을 강제하는지 먼저 확인한 뒤, **OTHER GOODS / LONGING의 작품적 성격과 충돌하는 지점**을 나눠서 보겠습니다. 핵심은 “Apple처럼 보이게 만들 것인가”가 아니라, **Apple의 설계 규율만 빌려올 수 있는가**입니다.

> **검토를 위해 디렉터리와 스킬 자료를 조회하고 Apple 디자인 적용을 검토**
>
> 
>
> 32s 동안 처리함

응. **그 스킬을 그대로 적용하는 건 오히려 별로일 가능성이 높고, 일부 원칙만 하위 레이어로 사용하는 건 상당히 좋다고 봐.**

확인해보니 이 스킬은 단순히 “Apple처럼 예쁘게 만들어라”는 스킬은 아니다. Apple HIG를 플랫폼 독립적인 원칙으로 바꿔서 접근성 → 플랫폼 관습 → 시각 디자인 → 인터랙션 → 문구 순으로 UI를 감사하고, 색상·타이포그래피·레이아웃·접근성은 항상 검토하도록 되어 있다.  그래서 **UI 품질 검수기**로서는 꽤 괜찮다.

문제는 우리 작품에서는 **좋은 일반 UI와 좋은 작품 UI가 반드시 같은 게 아니라는 점**이야.

### OTHER GOODS

OTHER GOODS는 기본적으로 커머스라는 익숙한 문법을 이용하는 작품이잖아. 그래서 여기에는 Apple식 원칙이 꽤 유용해.

상품 목록이 잘 읽히고, 장바구니가 이해되고, 결제 인터랙션이 자연스럽고, 가격/재고/상태가 명확하게 보이는 것은 오히려 중요해. 사용자가 인터페이스 때문에 막히는 게 아니라 **“이걸 정말 상품처럼 사고 있다는 상황” 때문에 이상함을 느껴야 하기 때문**이야.

즉,

> UI는 너무나 정상적인데  
> 판매되고 있는 것이 비정상적이다.

이 구조가 OTHER GOODS에서는 굉장히 강할 수 있어.

Apple HIG의 **명료성, 계층 구조, 정렬, 피드백, 접근성, 터치 영역, 반응형 레이아웃** 같은 부분은 그대로 차용해도 좋다고 봐.

반면 Apple의 **시각 스타일**까지 가져오면 위험해.

둥근 카드, 과도한 여백, 친절한 아이콘, Liquid Glass, 부드러운 애니메이션 같은 것이 전면에 나오면 OTHER GOODS가

> TENDER SYSTEMS의 이상한 상거래 시스템

이 아니라

> Apple Store 느낌의 예쁜 컨셉 쇼핑몰

처럼 보일 수 있어.

그건 피하고 싶어.

---

### LONGING

LONGING에서는 훨씬 더 조심해야 해.

우리가 지금 잡은 방향은 **Bloomberg Terminal / research center / market intelligence system**에 가깝고, 현재 지수·차트·애널리스트 리포트가 동시에 보이는 고밀도 정보 환경이 핵심이었지.

여기에 Apple HIG를 강하게 적용하면 상당 부분이 망가질 가능성이 있다.

예를 들어 이 스킬은 일반적으로 표준 플랫폼 내비게이션, 명확한 계층, 간결한 문구, 시스템 컴포넌트 사용 등을 권장한다. 

그런데 LONGING에서는 오히려

```text
LNG Composite        62.41   +1.82%
ROMANTIC EXPOSURE    71.08   ▲
UTILITY PRESSURE     44.12   ▼

ANALYST CONSENSUS
------------------------------
LONG    4
NEUTRAL 7
SHORT   12

LN-RISK / 30D        0.73
```

같은 **조금 과도할 정도의 정보 밀도와 전문 시스템의 언어**가 작품의 일부야.

Apple식으로 정리하다 보면

```text
Longing Index

62.4
↑ 1.8% today

View analysis
```

같아질 가능성이 있는데, 이 순간 LONGING은 작품의 상당 부분을 잃어버린다고 생각해.

전자는 **기관의 시스템** 같고, 후자는 **잘 만든 소비자용 금융 앱** 같거든.

그래서 LONGING에서는 Apple HIG를 거의 **보이지 않는 품질 검수 레이어**로만 쓰는 게 좋겠다.

---

## 그래서 나는 이런 구조를 추천해

Apple Design Skill을 디자인 생성의 최상위 규칙으로 두지 않고:

```text
TENDER SYSTEMS DESIGN PRINCIPLES
        ↓
PROJECT-SPECIFIC DESIGN LANGUAGE
        ↓
OTHER GOODS / LONGING UI RULES
        ↓
APPLE HIG
        ↓
ACCESSIBILITY / USABILITY CHECK
```

이 순서로 두는 거야.

Apple HIG가 위에 있으면

> “이 디자인은 비표준적입니다. 표준 UI로 바꾸겠습니다.”

가 되어버리고,

TENDER SYSTEMS 원칙이 위에 있으면

> “이 비표준성이 작품적으로 의도된 것인가?”
>
> YES → 유지
>
> NO → HIG를 이용해 개선

할 수 있어.

이 차이가 굉장히 중요하다고 생각해.

### 적용 여부를 나누면

| 영역 | Apple 원칙 적용 |
|---|---|
| 접근성 | 적극 적용 |
| 텍스트 가독성 | 적극 적용 |
| 클릭/터치 영역 | 적극 적용 |
| 오류 처리 | 적극 적용 |
| 로딩/상태 피드백 | 적극 적용 |
| 반응형 레이아웃 | 적극 적용 |
| 정보 계층 | 참고 |
| spacing consistency | 참고 |
| 플랫폼 표준 navigation | 선택적 |
| 표준 component 사용 | 선택적 |
| 정보 밀도 감소 | **적용하지 않음** |
| 전문 용어 제거 | **적용하지 않음** |
| 친절한 UX writing | **적용하지 않음** |
| Apple aesthetic | **적용하지 않음** |
| Liquid Glass | 거의 사용하지 않음 |

특히 스킬에는 아예 **Liquid Glass Review 모드**까지 들어 있다.  이건 TENDER SYSTEMS에서는 특별한 개념적 이유가 없는 한 굳이 가져오지 않는 편이 좋다고 본다.

---

## 그런데 오히려 이것을 이용해서 아주 좋은 걸 만들 수 있어

나는 이 Apple Design Skill을 직접 설치해서 모든 프로젝트에 적용하기보다는, **fork하거나 wrapping해서 `TENDER SYSTEMS Design Skill`을 만드는 방향**이 상당히 마음에 들어.

예를 들면 가장 중요한 원칙을 이렇게 시작하는 거지.

```text
TENDER SYSTEMS interfaces are not consumer software.

They may resemble commerce systems,
financial terminals,
research databases,
administrative tools,
or institutional infrastructure.

Usability should support the fiction,
not erase it.
```

그리고 아주 중요한 예외 규칙을 둔다.

```text
Do not automatically "fix" intentional friction.

Before modifying an unconventional interface,
determine whether the friction serves
a conceptual, narrative, or institutional function.
```

더 나아가:

```text
Clarity ≠ simplicity.

High information density is acceptable
when density itself communicates
institutional authority, measurement,
analysis, or bureaucracy.
```

그리고 Apple Design Skill을 마지막에 호출해서,

> 접근성 문제인가?  
> 진짜 사용성 문제인가?  
> 아니면 작품적으로 의도된 불편함인가?

를 구분하게 하는 거야.

이렇게 하면 꽤 강력할 것 같아.

그리고 사실 **OTHER GOODS와 LONGING을 같은 작가의 작품처럼 느끼게 만드는 공통 디자인 문법을 만드는 데도 이 방식이 상당히 유용하다.** Apple의 디자인을 가져오는 게 아니라, Apple이 HIG를 통해 여러 제품을 하나의 시스템처럼 관리하는 **‘디자인 규칙을 만드는 방식’ 자체를 가져오는 것**이지. 이게 TENDER SYSTEMS에는 훨씬 더 잘 어울린다고 생각해. 

원한다면 다음 단계로 **이 `apple-design-skill`의 SKILL.md를 기반으로 `TENDER SYSTEMS Design Skill`의 초안을 실제로 만들어보자.** OTHER GOODS와 LONGING뿐 아니라 앞으로 나오는 OG-002, LN-002 같은 시스템까지 공통으로 통제하는 디자인 헌법에 가깝게 만들 수 있을 것 같아.



---
Powered by [ChatGPT Exporter](https://www.chatgptexporter.com)