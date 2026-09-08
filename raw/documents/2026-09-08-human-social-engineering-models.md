# 인간·사회 현상의 수학적 모델과 공학 논문: TENDER SYSTEMS 참고 조사

조사 기준일: 2026-09-08  
상태: 연구 참고 제안. 설계 결정·구현·실증 검증 아님.

## 조사 맥락

GitHub의 LONGING, OTHER GOODS, THE RESERVE의 `wiki/current-state.md`, LONGING의 `wiki/concepts/academic-model-survey.md` 및 기존 교차분야 목록, TENDER SYSTEMS의 `wiki/overview.md`를 읽고 선별했다. LONGING에는 이미 120항목의 교차분야 탐색 목록이 있다. 이 문서는 그 목록의 원출처 재확인과 추가 후보 선별을 결합한 20편의 주석 목록이며, 20편 모두 처음 발견된 논문이라는 뜻이 아니다.

현재 LONGING의 제작 기반은 가상의 과거와 축적된 시장·연구 기록이다. 실제 감정을 실시간 측정하는 서비스로 전제하지 않는다. OTHER GOODS의 모든 상품에 특별한 계산 장치를 의무화하지 않는다. THE RESERVE의 신용·보관·통화 체계는 확정된 것으로 취급하지 않는다.

## 읽을 때 구별할 것

- **이론적 설명 모델:** 명시된 가정 아래 어떤 결과가 나오는지 분석한다. 현실의 보편법칙과는 다르다.
- **데이터·실험 기반 모델:** 특정 관측과 과제에서 얼마나 설명하거나 예측하는지 평가한다. 다른 대상·시간 단위로의 전이는 별도 검증이 필요하다.
- **알고리즘·공학적 정리:** 규칙이 무엇을 보장하는지 명시한다. 그 보장이 인간적 바람직함 전체를 뜻하지 않는다.

각 항목의 ‘작품 연결’은 이번 조사의 해석·제안이며 원 논문의 주장이나 사용자 확정 사항이 아니다. DOI·공식 링크·원문 위치를 남겼지만, 20편 모두의 전체 증명·부록을 정독하거나 구현한 체계적 문헌고찰은 아니다. 구체적인 확인 범위는 항목별로 기록했다.

## 우선순위 안내

세계관의 긴장을 생각할 때는 Bénabou–Tirole, Inverse Reward Design, Algorithmic Monoculture를 먼저 읽을 만하다. 인간적 경험의 모델링 사례로는 Loewenstein, Rutledge, Rinaldi가 좋다. LONGING의 정보·가격·연구 기록 설계에는 Kalman, Brock–Hommes, Lamport, Brier가 서로 다른 층을 제공한다. 이들 모두를 하나의 가격식에 더하라는 권고는 아니다.

## 주석 서지 20편

### 01. Laura and Petrarch: An Intriguing Case of Cyclical Love Dynamics (1998)

**저자:** Rinaldi, Sergio  
**출판:** SIAM Journal on Applied Mathematics, 58(4), 1205–1221  
**분야:** 문학 소재 / 비선형 동역학

**모델이 다루는 것:** 페트라르카와 라우라의 감정, 시적 영감을 세 상태변수로 놓고 상호작용과 감쇠를 연립 미분방정식으로 표현한다.

**작품 연결 — 제안:** 감정을 점수 하나로 고정하기보다 관계·시간·창작의 피드백으로 구성하는 참고 사례. LONGING 가격식으로 직접 쓰는 모델은 아니다.

**가정·한계:** 시의 정서·연대 해석에 의존하는 탐색적 사례다. 실제 인물의 내면을 독립적으로 관측하거나 사랑의 보편법칙을 입증한 연구가 아니다.

**이번 확인 범위:** 공개 원문 모델 부분과 문헌적 자료의 한계 확인; 인쇄면 1208의 방정식 확인.

**원출처:** [SIAM Journal on Applied Mathematics / 원문](https://userpages.umbc.edu/~rostamia/math481/love-dynamics/love-dynamics-1998-b.pdf)  
**DOI:** `10.1137/S003613999630592X`  
**BibTeX 키:** `Rinaldi1998Laura`

### 02. A computational and neural model of momentary subjective well-being (2014)

**저자:** Rutledge, Robb B.; Skandali, Nikolina; Dayan, Peter; Dolan, Raymond J.  
**출판:** Proceedings of the National Academy of Sciences, 111(33), 12252–12257  
**분야:** 계산인지과학 / 실험

**모델이 다루는 것:** 확실한 보상, 기대값, 보상예측오차의 최근 이력을 감쇠 가중합하여 순간적 행복 보고를 설명한다. 확률적 보상 과제와 스마트폰 과제를 사용한다.

**작품 연결 — 제안:** 같은 결과라도 기대와 경험의 순서에 따라 다른 정서적 상태를 만드는 설계 참고. 기대·결과·기억을 분리하는 데 유용하다.

**가정·한계:** 삶 전체의 행복이나 낭만의 시장가격을 계산하는 공식이 아니다. 과제에서 얻은 시간 단위와 계수를 작품의 주간 데이터에 그대로 이식할 수 없다.

**이번 확인 범위:** 저자 공개 원문 PDF의 모델 식·실험 범위·추가 실험 부분 확인.

**원출처:** [Proceedings of the National Academy of Sciences / 원문](https://www.robbrutledge.com/s/RutledgeSkandaliDayanDolanPNAS2014.pdf)  
**DOI:** `10.1073/pnas.1407535111`  
**BibTeX 키:** `Rutledge2014WellBeing`

### 03. Anticipation and the Valuation of Delayed Consumption (1987)

**저자:** Loewenstein, George  
**출판:** The Economic Journal, 97(387), 666–684  
**분야:** 행동경제학 / 시간선호

**모델이 다루는 것:** 실제 소비뿐 아니라 그 이전의 기대와 두려움에도 효용을 부여하여 지연된 소비의 평가를 설명한다.

**작품 연결 — 제안:** 편지의 답장이나 필름 현상을 기다리는 경험에서 기다림의 비용과 기대의 가치를 분리하는 출발점이다.

**가정·한계:** 기다림이 항상 좋다는 주장이 아니다. 불확실한 관계의 기다림은 원래의 지연 소비 문제보다 추가적인 가정이 필요하다.

**이번 확인 범위:** 저자 공개 원문 및 인쇄면 670의 기대효용/소비효용 구분 확인.

**원출처:** [The Economic Journal / 원문](https://www.cmu.edu/dietrich/sds/docs/loewenstein/AnticipationDelayed.pdf)  
**DOI:** `10.2307/2232929`  
**BibTeX 키:** `Loewenstein1987Anticipation`

### 04. Incentives and Prosocial Behavior (2006)

**저자:** Bénabou, Roland; Tirole, Jean  
**출판:** American Economic Review, 96(5), 1652–1678  
**분야:** 경제학 / 신호·동기 모형

**모델이 다루는 것:** 내재적 동기, 외적 보상, 비용, 타인과 자신에게 보이는 이미지가 결합된 의사결정을 모델링한다. 보상이 동기의 해석을 바꾸면 참여를 약화시킬 수도 있다.

**작품 연결 — 제안:** OTHER GOODS에서 가격·결제를 도입한 뒤에도 행위의 의미가 같은지 검토하기 좋다. THE RESERVE의 약속과 평판에도 비교할 수 있다.

**가정·한계:** 돈이 언제나 선의를 파괴한다는 결론이 아니다. 효과는 정보와 평판의 조건에 의존한다.

**이번 확인 범위:** 공식 초록 및 저자 원문 https://rbenabou.scholar.princeton.edu/document/30 의 모델 부분 확인.

**원출처:** [American Economic Review / 원문](https://www.aeaweb.org/articles?id=10.1257/aer.96.5.1652)  
**DOI:** `10.1257/aer.96.5.1652`  
**BibTeX 키:** `BenabouTirole2006Prosocial`

### 05. Threshold Models of Collective Behavior (1978)

**저자:** Granovetter, Mark  
**출판:** American Journal of Sociology, 83(6), 1420–1443  
**분야:** 수리사회학 / 임계값 모형

**모델이 다루는 것:** 다른 사람들의 참여가 자신의 임계값을 넘을 때 행동하는 개인들의 결합으로 집단행동을 설명한다.

**작품 연결 — 제안:** 작은 변화가 관습의 급격한 쇠퇴나 재개로 이어지는 가상 역사의 후보 메커니즘이다.

**가정·한계:** 임계값이나 관찰 대상이 정해져야 한다. 모든 사회적 변화가 전염이나 임계값으로 설명되는 것은 아니다.

**이번 확인 범위:** 출판사 서지와 초록 중심 선별; 전체 증명과 시뮬레이션 재현은 하지 않음.

**원출처:** [American Journal of Sociology / 원문](https://www.journals.uchicago.edu/doi/10.1086/226707)  
**DOI:** `10.1086/226707`  
**BibTeX 키:** `Granovetter1978Thresholds`

### 06. Modelling the dynamics of language death (2003)

**저자:** Abrams, Daniel M.; Strogatz, Steven H.  
**출판:** Nature, 424, 900  
**분야:** 문화 변화 / 비선형 전환모형

**모델이 다루는 것:** 두 언어 집단 사이의 이동률을 사용 인구 비중과 언어의 지위에 연결한다.

**작품 연결 — 제안:** 관행의 쇠퇴가 외생적인 하락 직선이 아니라 선택과 전환의 누적으로 발생하게 하는 비교 사례다.

**가정·한계:** 기본형은 두 언어·배타적인 사용 집단을 단순화한다. 서로 병행할 수 있는 편지와 메시지, 여러 종목에 그대로 적용할 수 없다. 참여율과 가격도 별개다.

**이번 확인 범위:** 한 페이지 원문과 방정식 확인: https://pdodds.w3.uvm.edu/teaching/courses/2009-08UVM-300/docs/others/2003/abrams2003.pdf

**원출처:** [Nature / 원문](https://www.nature.com/articles/424900a)  
**DOI:** `10.1038/424900a`  
**BibTeX 키:** `AbramsStrogatz2003Language`

### 07. Accelerating dynamics of collective attention (2019)

**저자:** Lorenz-Spreen, Philipp; Mønsted, Bjarke Mørch; Hövel, Philipp; Lehmann, Sune  
**출판:** Nature Communications, 10, 1759  
**분야:** 계산사회과학 / 주의 경쟁

**모델이 다루는 것:** 여러 자료에서 집단적 관심의 시간적 변화를 조사하고 유한한 관심을 두고 주제들이 경쟁하는 모델을 제시한다.

**작품 연결 — 제안:** 더 많은 이야기와 더 짧아지는 관심의 체류시간을 분리하여 LONGING의 attention 층을 설계하는 데 적합하다.

**가정·한계:** 집단적 주제 관심의 변화와 개인의 집중력 저하, 낭만의 실천 빈도는 같은 변수가 아니다.

**이번 확인 범위:** 출판사 색인 및 공저자 소속기관 초록·서지 확인: https://orbit.dtu.dk/en/publications/accelerating-dynamics-of-collective-attention/ . 원문 전체 검토 아님.

**원출처:** [Nature Communications / 원문](https://www.nature.com/articles/s41467-019-09311-w)  
**DOI:** `10.1038/s41467-019-09311-w`  
**BibTeX 키:** `LorenzSpreen2019Attention`

### 08. A New Approach to Linear Filtering and Prediction Problems (1960)

**저자:** Kalman, R. E.  
**출판:** Journal of Basic Engineering, 82(1), 35–45  
**분야:** 제어공학 / 상태추정

**모델이 다루는 것:** 시스템의 상태와 잡음이 포함된 측정을 구분하고 측정이 들어올 때 상태 추정을 재귀적으로 갱신한다.

**작품 연결 — 제안:** LONGING에서 세계의 상태, 관측 자료, 기관의 추정치, 시장가격을 분리하는 기반 구조로 참고할 수 있다.

**가정·한계:** 선형성·잡음 등 가정 아래의 추정법이다. 의도적인 허위 보도를 자동으로 판별하지 않는다. 가격결정식이나 가치의 정의를 제공하지 않는다.

**이번 확인 범위:** 공식 초록과 원문 확인: https://eceweb1.rutgers.edu/~gajic/pdffiles/519KalmanFiltering/kalman1960.pdf . 필터 구현·수치 검증 없음.

**원출처:** [Journal of Basic Engineering / 원문](https://asmedigitalcollection.asme.org/fluidsengineering/article/82/1/35/397706/A-New-Approach-to-Linear-Filtering-and-Prediction)  
**DOI:** `10.1115/1.3662552`  
**BibTeX 키:** `Kalman1960Filtering`

### 09. The Beta Reputation System (2002)

**저자:** Jøsang, Audun; Ismail, Roslan  
**출판:** Proceedings of the 15th Bled Electronic Commerce Conference  
**분야:** 전자상거래 / 확률적 평판 시스템

**모델이 다루는 것:** 긍정·부정 피드백을 베타분포로 결합하고 평판 평가를 도출하는 시스템을 제안한다.

**작품 연결 — 제안:** THE RESERVE의 신뢰를 단일 점수가 아니라 증거의 양과 불확실성까지 포함하여 다루는 참고점이다.

**가정·한계:** 거래 피드백에서 추정하는 평판은 사람의 도덕적 가치나 모든 맥락의 신뢰가 아니다. 평가 조작과 맥락 이동은 추가 문제다.

**이번 확인 범위:** 공식 학회 아카이브 초록 및 저자 PDF 색인 확인. PDF 직접 열람은 제한됨. 저자순서는 원문 PDF 색인(Audun Jøsang, Roslan Ismail)을 따름; AIS 메타데이터 순서와 다름.

**원출처:** [Proceedings of the 15th Bled Electronic Commerce Conference / 원문](https://aisel.aisnet.org/bled2002/41/)  
**BibTeX 키:** `JosangIsmail2002Beta`

### 10. A Proof for the Queuing Formula: {L = λW} (1961)

**저자:** Little, John D. C.  
**출판:** Operations Research, 9(3), 383–387  
**분야:** 산업공학 / 대기행렬

**모델이 다루는 것:** 적절한 정상성·유한 평균 등의 조건에서 시스템의 평균 체류 수 L, 도착률 λ, 평균 체류시간 W 사이의 관계를 증명한다.

**작품 연결 — 제안:** 기관이 아직 처리하지 못한 약속이나 요청을 다룬다면, 유입·대기·처리량 사이의 일관성을 점검하는 참고점이다.

**가정·한계:** 매 순간의 수량에 적용하는 식이 아니다. 무한히 누적되는 상태에 유한한 정상상태 평균을 가정할 수 없다. 기다림의 정서적 의미는 설명하지 않는다.

**이번 확인 범위:** 출판사 초록에 기재된 정리와 조건, 서지 확인. 전체 증명 재검증은 하지 않음.

**원출처:** [Operations Research / 원문](https://pubsonline.informs.org/doi/10.1287/opre.9.3.383)  
**DOI:** `10.1287/opre.9.3.383`  
**BibTeX 키:** `Little1961Queue`

### 11. College Admissions and the Stability of Marriage (1962)

**저자:** Gale, David; Shapley, Lloyd S.  
**출판:** The American Mathematical Monthly, 69(1), 9–15  
**분야:** 수학 / 시장설계·알고리즘

**모델이 다루는 것:** 두 집단의 선호에 따라 현재 배정을 서로 바꾸고 싶어 하는 차단 쌍이 없는 안정적 매칭을 구성한다.

**작품 연결 — 제안:** 기관의 완벽한 규칙이 보장하는 성질과 인간이 기대하는 좋은 관계가 어떻게 다른지 생각하게 한다.

**가정·한계:** 안정성은 최대 행복이나 공정성 일반을 뜻하지 않는다. 실제 결혼의 심리나 모든 현실 제약을 설명하는 모델이 아니다.

**이번 확인 범위:** 원문 스캔의 안정성과 최적성 정의 부분 확인; RAND 원본도 발견.

**원출처:** [The American Mathematical Monthly / 원문](https://cramton.umd.edu/market-design-papers/gale-shapley-college-admissions.pdf)  
**DOI:** `10.1080/00029890.1962.11989827`  
**BibTeX 키:** `GaleShapley1962Matching`

### 12. Resource-rational analysis: Understanding human cognition as the optimal use of limited computational resources (2020)

**저자:** Lieder, Falk; Griffiths, Thomas L.  
**출판:** Behavioral and Brain Sciences, 43, e1  
**분야:** 계산인지과학 / 방법론

**모델이 다루는 것:** 제한된 계산 자원과 계산 비용을 고려해 인지 전략을 분석하는 resource-rational 접근을 제안한다.

**작품 연결 — 제안:** LONGING의 사유를 생각의 양보다 자기 판단을 형성하는 조건으로 다룰 때, 판단의 이익과 시간·인지 비용을 구별하는 참고점이다.

**가정·한계:** 인간이 실제로 항상 최적화한다는 확정된 법칙이 아니다. 비용을 줄이는 것이 사유의 가치를 높인다는 결론도 아니다.

**이번 확인 범위:** 출판사 초록과 서지 중심 검토. 개별 사례와 논평 전체 정독은 하지 않음.

**원출처:** [Behavioral and Brain Sciences / 원문](https://www.cambridge.org/core/journals/behavioral-and-brain-sciences/article/abs/resourcerational-analysis-understanding-human-cognition-as-the-optimal-use-of-limited-computational-resources/586866D9AD1D1EA7A1EECE217D392F4A)  
**DOI:** `10.1017/S0140525X1900061X`  
**BibTeX 키:** `LiederGriffiths2020Resource`

### 13. Inverse Reward Design (2017)

**저자:** Hadfield-Menell, Dylan; Milli, Smitha; Abbeel, Pieter; Russell, Stuart; Dragan, Anca  
**출판:** Advances in Neural Information Processing Systems, 30  
**분야:** 인공지능 / 보상함수·추론

**모델이 다루는 것:** 설계된 보상함수를 진짜 목적 그 자체가 아니라 설계 상황에서 의도된 목적에 관한 불완전한 관측으로 보고 추론한다.

**작품 연결 — 제안:** 기관이 채택한 지표와 인간적 가치의 차이를 형식적으로 다루는 참고점. 정교한 시스템이 부정확한 목표를 충실하게 최적화하는 문제에 연결된다.

**가정·한계:** 가치 정렬 문제를 일반적으로 해결한 논문은 아니다. 제한된 환경의 모델·실험이며 작품에 강화학습을 반드시 넣어야 한다는 뜻도 아니다.

**이번 확인 범위:** 공식 학회 초록·공개 원문, 도입의 보상함수 사례와 추론 문제 설정 확인.

**원출처:** [Advances in Neural Information Processing Systems / 원문](https://proceedings.neurips.cc/paper/2017/hash/32fdab6559cdfa4f167f8c31b9199643-Abstract.html)  
**BibTeX 키:** `HadfieldMenell2017IRD`

### 14. Algorithmic Monoculture and Social Welfare (2021)

**저자:** Kleinberg, Jon; Raghavan, Manish  
**출판:** Proceedings of the National Academy of Sciences, 118(22), e2018340118  
**분야:** 컴퓨터과학 / 알고리즘·사회후생

**모델이 다루는 것:** 개별 선택자에게 더 정확한 알고리즘도 여러 선택자가 함께 사용할 때 집단의 선택 결과를 악화시킬 수 있는 조건을 확률적 선택 모델로 분석한다.

**작품 연결 — 제안:** 악한 인물이나 고장 없이, 합리적인 개인 선택과 공통 평가 기준의 결합이 인간적 가능성을 좁히는 세계를 설계하는 데 유용하다.

**가정·한계:** 모든 알고리즘이 사회에 해롭다는 주장이 아니며 오늘날 LLM 이용자를 직접 실험한 연구도 아니다.

**이번 확인 범위:** 저자 아카이브 초록 및 PNAS 출판 서지 확인. 정리 증명과 수치 실험 전체 검토 아님.

**원출처:** [Proceedings of the National Academy of Sciences / 원문](https://arxiv.org/abs/2101.05853)  
**DOI:** `10.1073/pnas.2018340118`  
**BibTeX 키:** `KleinbergRaghavan2021Monoculture`

### 15. A Theory of Fairness, Competition, and Cooperation (1999)

**저자:** Fehr, Ernst; Schmidt, Klaus M.  
**출판:** The Quarterly Journal of Economics, 114(3), 817–868  
**분야:** 행동경제학 / 불평등 회피

**모델이 다루는 것:** 자신의 금전 보상뿐 아니라 타인보다 적게 또는 많이 받는 불평등을 효용에 포함한다.

**작품 연결 — 제안:** 같은 가격이나 보상도 비교 대상에 따라 다르게 받아들여지는 상황의 참고 모델이다.

**가정·한계:** 불평등 회피는 도덕·책임·죄책감 전부가 아니다. 논문도 의도와 결과를 구별하며 의도를 완전히 모델링하지 않는 한계를 인정한다.

**이번 확인 범위:** 공개 원문 인쇄면 822의 일반식과 2인식 확인.

**원출처:** [The Quarterly Journal of Economics / 원문](https://archiv.soms.ethz.ch/sociology_course/Lecture6/Fehr1999.pdf)  
**DOI:** `10.1162/003355399556151`  
**BibTeX 키:** `FehrSchmidt1999Fairness`

### 16. The Economics of Cultural Transmission and the Dynamics of Preferences (2001)

**저자:** Bisin, Alberto; Verdier, Thierry  
**출판:** Journal of Economic Theory, 97(2), 298–319  
**분야:** 경제학 / 세대 간 문화전승

**모델이 다루는 것:** 부모의 사회화 노력과 사회적 전승으로 선호의 인구 분포가 변화하는 모델을 다룬다. 조건에 따라 이질적인 문화 분포가 유지된다.

**작품 연결 — 제안:** 관행이 다음 세대로 이어지는 조건과 유지 비용을 가상의 역사에 넣는 후보이며 쇠퇴만 예정하는 서사를 견제할 수 있다.

**가정·한계:** 소수 문화가 반드시 살아남거나 부모가 전승을 완전히 통제한다는 뜻이 아니다. 작품에 맞는 상태·전승 단위를 새로 정의해야 한다.

**이번 확인 범위:** 저자 공개 원문의 초록·문제 설정 확인. 모든 안정성 조건과 증명을 재검증하지 않음.

**원출처:** [Journal of Economic Theory / 원문](https://bpb-us-e1.wpmucdn.com/wp.nyu.edu/dist/c/16384/files/2019/12/43.-bvjet.pdf?bid=16384)  
**DOI:** `10.1006/jeth.2000.2678`  
**BibTeX 키:** `BisinVerdier2001Culture`

### 17. The universal decay of collective memory and attention (2019)

**저자:** Candia, Cristian; Jara-Figueroa, C.; Rodriguez-Sickert, Carlos; Barabási, Albert-László; Hidalgo, César A.  
**출판:** Nature Human Behaviour, 3, 82–91  
**분야:** 계산사회과학 / 집단기억

**모델이 다루는 것:** 문화적 산출물에 대한 관심의 감소를 소통적 기억과 기록된 문화적 기억의 경로로 설명한다.

**작품 연결 — 제안:** 작품의 attention 층에서 사건이나 문화적 대상이 잊히는 시간 구조를 참고할 수 있다.

**가정·한계:** 논문 제목의 universal을 모든 기억에 대한 보편법칙으로 확대하면 안 된다. 개인의 기억과 관련 행위의 실천율은 직접 측정한 변수가 아니다.

**이번 확인 범위:** 출판사 초록·서지 확인. 학술지 연도는 2019이며 온라인 공개는 2018.

**원출처:** [Nature Human Behaviour / 원문](https://www.nature.com/articles/s41562-018-0474-5)  
**DOI:** `10.1038/s41562-018-0474-5`  
**BibTeX 키:** `Candia2019Memory`

### 18. Heterogeneous beliefs and routes to chaos in a simple asset pricing model (1998)

**저자:** Brock, William A.; Hommes, Cars H.  
**출판:** Journal of Economic Dynamics and Control, 22(8--9), 1235–1274  
**분야:** 계산경제학 / 이질적 기대

**모델이 다루는 것:** 이질적인 기대 규칙과 그 선택이 자산가격과 함께 변화하는 동학을 분석한다.

**작품 연결 — 제안:** LONGING에서 전망의 가중치와 시장가격이 서로 영향을 주는 계산적 구조를 고민할 때 직접적이다.

**가정·한계:** 원모형의 거래자 수익·전략 선택 구조를 작품의 애널리스트 전망과 동일시하지 않는다. 가상의 인간적 대상에 가격을 부여하는 정의는 별도로 필요하다.

**이번 확인 범위:** 원 논문 출판 서지 및 저자 Hommes의 2013년 저서 해당 장 요약으로 모델 구조 교차 확인. 1998년 논문 전체 증명 검토 아님.

**원출처:** [Journal of Economic Dynamics and Control / 원문](https://www.sciencedirect.com/science/article/abs/pii/S0165188998000116)  
**DOI:** `10.1016/S0165-1889(98)00011-6`  
**BibTeX 키:** `BrockHommes1998Beliefs`

### 19. Time, Clocks, and the Ordering of Events in a Distributed System (1978)

**저자:** Lamport, Leslie  
**출판:** Communications of the ACM, 21(7), 558–565  
**분야:** 분산시스템 / 사건 순서

**모델이 다루는 것:** 서로 다른 프로세스의 사건에 대해 메시지와 프로세스 내 순서를 바탕으로 happened-before 관계와 논리 시계를 구성한다.

**작품 연결 — 제안:** 가상의 과거에서 사건 발생, 정보 전달, 보고서 발간의 순서를 구별하고 당시 이용할 수 없던 미래 정보를 차단하는 사고 도구다.

**가정·한계:** 논리 시계의 숫자가 실제 물리적 시간이나 인과의 완전한 증거는 아니다. 반드시 분산 인프라를 구현해야 한다는 뜻도 아니다.

**이번 확인 범위:** 저자 공개 원문 인쇄면 559의 사건 순서 정의와 도식 확인.

**원출처:** [Communications of the ACM / 원문](https://lamport.azurewebsites.net/pubs/time-clocks.pdf)  
**DOI:** `10.1145/359545.359563`  
**BibTeX 키:** `Lamport1978Time`

### 20. Verification of Forecasts Expressed in Terms of Probability (1950)

**저자:** Brier, Glenn W.  
**출판:** Monthly Weather Review, 78(1), 1–3  
**분야:** 기상학 / 확률예측 검증

**모델이 다루는 것:** 사건에 부여한 확률과 실제 결과의 제곱오차를 사용하여 확률 예보를 평가하는 기준을 제시한다.

**작품 연결 — 제안:** LONGING의 애널리스트 기록을 단순 적중 여부보다 확률 판단의 질로 비교하려 할 때 출발점이 된다.

**가정·한계:** 목표주가 하나나 BUY/HOLD/SHORT 라벨만으로 바로 적용할 수 없다. 사건·평가기간·결과를 정의하고 동일한 기준에서 비교해야 한다.

**이번 확인 범위:** 출판사 서지·색인 중심 확인; 원문 직접 접근 제한. 현대의 이진 Brier score 표기는 원래 범주 합산식과 정규화가 다를 수 있음.

**원출처:** [Monthly Weather Review / 원문](https://journals.ametsoc.org/view/journals/mwre/78/1/1520-0493_1950_078_0001_vofeit_2_0_co_2.xml)  
**DOI:** `10.1175/1520-0493(1950)078<0001:VOFEIT>2.0.CO;2`  
**BibTeX 키:** `Brier1950Forecasts`

## 몇 가지 수식을 읽는 방법

### 순간적 행복: 논문의 모델식

Rutledge et al. (2014)의 표기를 정리하면 다음과 같다.

\[
H_t=w_0+w_1\sum_{j=1}^{t}\gamma^{t-j}CR_j
+w_2\sum_{j=1}^{t}\gamma^{t-j}EV_j
+w_3\sum_{j=1}^{t}\gamma^{t-j}RPE_j.
\]

CR은 확실한 선택의 보상, EV는 선택한 도박의 기대값, RPE는 도박 결과와 기대값의 차이, γ는 과거 사건의 영향이 줄어드는 가중치다. 이 식의 t는 실험 시행 순서이지 달력의 주가 아니다. 이 공식으로 ‘인생 전체의 행복’이나 ‘낭만의 금융가격’을 산출할 수 있다는 뜻이 아니다.

### 상태와 관측: 현대적인 단순화 표기

Kalman (1960)의 상태추정 접근을 설명하는 표준적인 선형 상태공간 표기는 다음과 같다. 원문 표기를 그대로 전사한 것은 아니다.

\[
x_{t+1}=Ax_t+w_t,\qquad y_t=Hx_t+v_t.
\]

x는 상태, y는 관측, w와 v는 각각 과정·관측 잡음이다. LONGING에 적용한다면 x의 정의, 잡음의 의미, H의 관측 관계가 먼저 정해져야 한다. 금융가격은 자동으로 y나 x가 되는 것이 아니다.

### 대기행렬: Little의 관계

\[
L=\lambda W.
\]

적절한 조건 아래 평균 체류 수 = 유입률 × 평균 체류시간이다. 예를 들어 안정적인 가상 시스템에서 매주 10건이 들어와 평균 4주 체류한다면 평균 40건이 시스템에 남는다. 이 숫자는 작품을 위한 산술 예시이지 논문의 실증 추정값이 아니다. 끝없이 적체되는 시스템에 유한한 정상상태를 가정하면 안 된다.

### 불평등 회피: 2인 모형

Fehr–Schmidt (1999), 식 (2):

\[
U_i=x_i-\alpha_i\max(x_j-x_i,0)-\beta_i\max(x_i-x_j,0).
\]

자신의 보상뿐 아니라 불리한 불평등과 유리한 불평등에 대한 반응을 구분한다. 원모형에서 βᵢ≤αᵢ, 0≤βᵢ<1을 가정한다. 그 반응을 ‘모든 도덕감정’으로 확장하는 것은 별개의 주장이다.

## 작품에 적용할 때 남길 연구 기록

각 모델마다 원래의 상태변수·단위·가정, 작품에서 바꾸는 부분, 합성 데이터 생성 규칙, 실제 관측과의 구분을 따로 적는 것이 좋다. 특히 사람들의 실천 빈도, 그에 대한 관심, 개인이 부여하는 가치, 연구기관의 추정, 시장의 가격은 서로 다른 양이다. 하나의 곡선을 재현했다고 그 곡선을 낳은 원인까지 밝혀진 것은 아니다.

현재 LONGING에서 제안할 수 있는 분리 구조는 ‘가상 세계의 상태 → 당시 이용 가능한 정보 → 기관의 추정 → 가격과 전망 → 사후 평가’다. 이는 문헌들을 읽기 위한 설계 제안이며, GitHub의 기존 설계를 변경하거나 채택한 것이 아니다.

## 확인한 프로젝트 문서

- [LONGING current-state](https://github.com/TENDER-SYSTEMS-LAB/longing-lab/blob/main/wiki/current-state.md)
- [LONGING academic-model-survey](https://github.com/TENDER-SYSTEMS-LAB/longing-lab/blob/main/wiki/concepts/academic-model-survey.md)
- [LONGING 기존 교차분야 목록](https://github.com/TENDER-SYSTEMS-LAB/longing-lab/blob/main/raw/surveys/2026-09-06-cross-domain-model-survey.md)
- [OTHER GOODS current-state](https://github.com/TENDER-SYSTEMS-LAB/other-goods-lab/blob/main/wiki/current-state.md)
- [THE RESERVE current-state](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab/blob/main/wiki/current-state.md)
- [TENDER SYSTEMS overview](https://github.com/TENDER-SYSTEMS-LAB/tender-systems/blob/main/wiki/overview.md)

수학적 일관성은 인간적 가치의 정당성을 대신하지 않는다. 그러나 무엇을 측정하고 무엇을 제외했는지를 명확히 하는 데에는 중요한 참고가 될 수 있다.
