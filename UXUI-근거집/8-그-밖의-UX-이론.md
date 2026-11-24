# 그 밖의 UX 이론 (노먼, 인지 부하, 정보 구조, 법칙과 효과, 슈나이더만, 접근성 4원칙, 감정과 기만적 설계, 검증 방법)

- 이 문서는 휴리스틱 10개, 피츠, 힉, 제이콥, 밀러, 게슈탈트 근접성과 유사성과 공통 영역, 시각 위계, 점진적 공개, 재인과 회상, 일관성, 접근성 대비와 누름 크기, 움직임 시간, 다크 모드, 토스 라이팅, 마이크로카피를 뺀 나머지 이론을 모았어요.
- 모든 출처는 2026-11-24에 직접 열어 확인했어요. 열지 못하고 검색 요약만 본 것은 맨 아래 '확인 못 한 것'에 따로 적었어요.
- 근거 세기는 세 단계예요. 강함은 반복 연구나 공식 표준, 보통은 고전 연구 하나나 실무 관찰이 쌓인 것, 약함은 원 연구를 확인하기 어렵거나 재현이 안 된 것이에요.

## 요약표

| 묶음 | 화면 점검에 바로 쓸 것 | 근거가 약해 조심할 것 |
|---|---|---|
| 사람이 기계를 이해하는 방식 | 누를 수 있다는 표시(기표), 누른 뒤 상태가 보이는지(평가의 간극) | 없음 |
| 주의와 기억 | 광고처럼 생긴 칸은 안 읽힘, 멀리서 바뀐 것은 못 봄 | 자이가르닉 효과(기억 우위는 재현 실패) |
| 정보 구조와 찾기 | 메뉴 이름만 보고 갈 곳이 짐작되는지, 카드 소팅 뒤 트리 테스트 | 없음 |
| 법칙과 효과 | 기본값, 끝 장면, 진행 표시, 입력은 너그럽게 | 도허티 400ms, 테슬러 법칙, 선택 과부하(조건부) |
| 설계 원칙 모음 | 슈나이더만 8원칙, 접근성 4원칙 | 없음 |
| 감정과 윤리 | 쓸모와 사용성이 먼저, 기만적 설계 금지(한국 전자상거래법 2025-02-14 시행) | 즐거움 피라미드는 실무 모형 |
| 제품과 검증 | 5명 테스트 반복, 소리 내어 생각하기, AI 평가는 시험을 대신 못 함 | 카노 모형은 시간이 지나면 분류가 바뀜 |

## 사람이 기계를 이해하는 방식

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 행동 유도성과 기표 (affordance, signifier) | 행동 유도성은 대상과 사람 사이에 가능한 행동이고, 기표는 그 행동을 알아보게 하는 눈에 보이는 단서예요. 노먼은 디자이너가 챙길 것은 기표라고 했어요 | 처음 보는 사람에게 화면을 보여 주고 "어디를 누를 수 있어요?"를 물어요. 누를 수 있는 것과 없는 것이 모양만으로 갈리는지 봐요 | 평평한 글자를 단추로 쓰거나, 장식을 단추처럼 그려 누르게 만들기 | 강함 (HCI 교과서의 기본 개념, 저자 본인 정리) | Don Norman, "Signifiers, not affordances", https://jnd.org/signifiers-not-affordances/, 2008-11-17 (ACM Interactions 15권 6호) |
| 노먼의 기본 원칙 (대응, 제약, 피드백, 개념 모형) | 대응은 조작과 결과의 자리 관계, 제약은 틀린 행동을 막는 장치, 피드백은 행동의 결과 알림, 개념 모형은 사용자가 머릿속에 그리는 작동 방식이에요 | 슬라이더를 오른쪽으로 밀면 값이 커지는지(대응), 못 하는 동작은 아예 막혔는지(제약), 누른 뒤 1초 안에 변화가 보이는지(피드백) 확인해요 | 조작 위치와 결과 위치가 떨어져 있음, 틀린 입력을 받은 뒤에야 오류를 알림 | 강함 (디자인 교과서 표준, 다만 아래 출처는 목차 확인) | Don Norman, "The Design of Everyday Things, Revised and Expanded" 책 소개, https://jnd.org/the-design-of-everyday-things-revised-and-expanded/, 2013년 판 |
| 실행의 간극과 평가의 간극, 행동 7단계 | 실행의 간극은 하고 싶은 것을 어떻게 하는지 모르는 거리, 평가의 간극은 지금 상태가 어떤지 모르는 거리예요. 행동은 목표, 의도, 행동 정하기, 실행, 지각, 해석, 평가의 7단계로 나뉘고 앞 셋이 실행, 뒤 셋이 평가 쪽이에요 | 과제를 주고 "다음에 뭘 누를지"와 "지금 된 건지"를 각각 물어요. 둘 중 하나라도 머뭇거리면 그쪽 간극이 커요 | 켜짐과 꺼짐이 헷갈리는 스위치처럼 표시와 실제 동작이 어긋남 | 강함 (고전 모형, NN/g가 실무 사례로 정리) | Kathryn Whitenton (NN/g), "The Two UX Gulfs: Evaluation and Execution", https://www.nngroup.com/articles/two-ux-gulfs-evaluation-execution/, 2018-03-11. 7단계는 위 노먼 책 2장 |
| 멘탈 모델 | 사용자가 믿는 시스템의 작동 방식이에요. 사실이 아니라 믿음이라 틀릴 수 있고, 만든 사람과 쓰는 사람의 모델 차이가 클수록 실수가 늘어요 | 소리 내어 생각하기 시험에서 사용자가 "이건 아마 ~겠지"라고 짐작하는 말을 받아 적어 실제 동작과 비교해요 | 만든 사람만 아는 구조를 그대로 메뉴로 드러냄, 새 조작 방식을 이유 없이 도입 | 강함 (반복 관찰된 현상, NN/g 장기 정리) | Megan Chan (NN/g, Jakob Nielsen 2010년 글 개정), "Mental Models and User Experience Design", https://www.nngroup.com/articles/mental-models/, 2024-01-26 |
| 직접 조작 | 화면의 대상을 끌고 누르며 바로 바꾸고, 결과가 즉시 보이며, 되돌릴 수 있는 방식이에요. 슈나이더만이 1983년에 이름 붙였어요 | 바꾸는 동안 결과가 실시간으로 보이는지, 되돌리기가 있는지, 화면 밖 대상도 닿을 수 있는지 봐요 | 몸짓만 있고 단추나 키보드 대안이 없음, 많은 대상을 한꺼번에 바꿀 방법이 없음 | 강함 (40년 넘은 표준 방식, 단점도 함께 정리됨) | Samyukta Sherugar, Raluca Budiu (NN/g), "Direct Manipulation: Definition", https://www.nngroup.com/articles/direct-manipulation/, 2016-08-21 (2024-10-14 재검토) |

## 주의와 기억

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 인지 부하 (내재 부하, 외재 부하) | 내재 부하는 내용을 이해하는 데 꼭 드는 노력이고, 외재 부하는 장식 글꼴처럼 이해에 도움 안 되는 노력이에요. 줄일 것은 외재 부하예요 | 화면의 요소마다 "이걸 빼면 사용자가 잃는 게 있나"를 물어요. 앞에서 적은 값을 다시 적게 하는지, 기본값으로 채울 수 있는지 봐요 | 뜻 없는 장식, 같은 링크 중복, 앞 화면 정보를 외워 오게 만들기 | 강함 (교육 심리학의 인지 부하 이론을 UX에 옮긴 것) | Kathryn Whitenton (NN/g), "Minimize Cognitive Load to Maximize Usability", https://www.nngroup.com/articles/minimize-cognitive-load/, 2013-12-22 |
| 선택적 주의와 터널 시야 | 사람은 목표와 관련된 좁은 곳만 보고 나머지는 걸러요. 만든 사람에게 뻔한 정보도 사용자는 놓쳐요 | 과제 중 사용자의 눈이 머무는 자리를 보고, 중요한 정보가 그 근처에 있는지 확인해요 | 핵심 숫자를 시선이 가는 본문 밖 모서리에 두기 | 강함 (수천 건 시험 관찰, 주의 연구와 일치) | Jakob Nielsen (NN/g), "Tunnel Vision and Selective Attention", https://www.nngroup.com/articles/tunnel-vision-and-selective-attention/, 2012-08-26 |
| 배너 맹시 | 광고처럼 보이는 요소는 진짜 내용이어도 건너뛰어요. 위쪽 띠, 오른쪽 기둥, 움직이거나 튀는 색, 광고 옆자리가 신호예요 | 중요한 안내를 광고 같은 자리나 모양으로 두지 않았는지 봐요. 시험에서 그 칸을 실제로 봤는지 물어요 | 눈에 띄게 하려고 반짝이는 띠 배너로 만들어 오히려 무시당함 | 강함 (1997, 2007, 2018 시선 추적에서 반복 확인) | Kara Pernice (NN/g), "Banner Blindness Revisited", https://www.nngroup.com/articles/banner-blindness-old-and-new-findings/, 2018-04-22 |
| 변화 맹시 | 시선이 머문 곳에서 먼 자리의 변화는 움직임 단서가 없으면 못 알아채요 | 누른 뒤 바뀌는 것이 누른 자리 근처인지, 바뀔 때 짧은 움직임이 있는지 봐요. 한 번에 여러 곳이 바뀌지 않는지 확인해요 | 결과를 화면 반대편 구석에 소리 없이 바꿔 넣음, 여러 애니메이션이 동시에 돌아 서로 가림 | 강함 (지각 심리 실험과 UI 관찰이 일치) | Raluca Budiu (NN/g), "Change Blindness in UX: Definition", https://www.nngroup.com/articles/change-blindness-definition/, 2018-09-23 |
| 무주의 맹시 | 한 가지 일에 집중하면 눈앞의 뚜렷한 뜻밖의 것도 못 봐요. 고릴라 실험이 대표 예이고, 전문 영상의학과 의사 24명 중 20명(83%)이 CT 속 고릴라를 못 봤어요 | 사용자가 과제에 몰두한 상태에서 경고나 새 정보가 눈에 들어오는지, 과제 흐름 안에 넣었는지 봐요 | 과제와 상관없는 자리에 경고를 띄우고 "보여 줬으니 됐다"고 여김 | 강함 (여러 실험 반복, 다만 지각 실패인지 기억 실패인지 논쟁 있음) | Drew, Vo, Wolfe, "The Invisible Gorilla Strikes Again", Psychological Science 24(9), https://pmc.ncbi.nlm.nih.gov/articles/PMC3964612, 2013 |
| 고립 효과 (폰 레스토프 효과) | 비슷한 것들 사이에서 하나만 다르면 그것이 더 잘 기억돼요 | 화면에서 강조된 것이 정말 하나뿐인지 세어 봐요. 색만으로 구분하지 않았는지 봐요 | 강조를 여러 개 써서 아무것도 안 튐, 튀게 만든 칸이 광고처럼 보여 배너 맹시를 부름 | 보통 (1933년 고전 기억 실험, UI 적용은 실무 추론) | Jon Yablonski, Laws of UX, "Von Restorff Effect", https://lawsofux.com/von-restorff-effect/, 날짜 표기 없음 (원 연구 Hedwig von Restorff 1933, 안내용으로만 사용) |
| 자이가르닉 효과와 오브시안키나 효과 | 자이가르닉은 끝내지 못한 일이 더 잘 기억된다는 주장이고, 오브시안키나는 끊긴 일을 다시 하려는 경향이에요. 2025년 메타분석에서 기억 우위는 확인되지 않았고 다시 하려는 경향만 확인됐어요 | "이어서 하기", 진행 중 표시처럼 끊긴 일을 다시 잡게 돕는 장치는 근거가 있어요. "미완료라 기억에 남는다"를 이유로 일부러 끊는 설계는 근거가 없어요 | UX 법칙 목록을 믿고 미완료 표시로 기억을 늘린다고 주장 | 약함 (자이가르닉 쪽은 재현 실패), 오브시안키나 쪽은 보통 | Ghibellini, Meier, "Interruption, recall and resumption: a meta-analysis of the Zeigarnik and Ovsiankina effects", Humanities and Social Sciences Communications 12권, https://ideas.repec.org/a/pal/palcom/v12y2025i1d10.1057_s41599-025-05000-w.html, 2025 |

## 정보 구조와 찾기

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 정보 구조 (IA)와 내비게이션의 차이 | 정보 구조는 어떤 내용이 있고 어떻게 묶고 이름 붙일지 정한 뼈대예요. 메뉴, 경로 표시, 필터 같은 내비게이션은 그 위에 보이는 끝부분이에요 | 화면을 그리기 전에 내용 목록과 묶음, 이름을 표로 먼저 만들었는지 봐요. 메뉴 단계가 내용 깊이와 맞는지 봐요 | 보기 좋은 메뉴 모양부터 고르고 내용을 끼워 맞춤 | 강함 (실무 표준 정의) | Jen Cardello (NN/g), "The Difference Between Information Architecture (IA) and Navigation", https://www.nngroup.com/articles/ia-vs-navigation/, 2014-06-22 |
| 카드 소팅 | 사용자가 카드에 적힌 내용을 스스로 묶고 이름 붙이게 해서 머릿속 분류를 알아내는 방법이에요. 열린 방식이 기본이고, 질적 연구는 15명 이상, 양적 연구는 30~50명, 카드는 30~50장을 권해요 | 메뉴 이름과 묶음이 만든 사람 회의에서 나왔는지, 사용자 분류에서 나왔는지 확인해요 | 회사 조직도대로 메뉴를 나눔, 닫힌 방식으로 검증까지 끝냈다고 여김 | 강함 (표준 조사법) | Samhita Tankala, Katie Sherwin (NN/g), "Card Sorting: Uncover Users' Mental Models", https://www.nngroup.com/articles/card-sorting-definition/, 2024-02-02 |
| 트리 테스트 | 디자인 없이 메뉴 나무만 보여 주고 "이건 어디서 찾을까요?"를 시켜 성공률, 걸린 시간, 곧장 갔는지(직진성)를 재요. 카드 소팅으로 만든 안을 검증하는 짝이에요 | 핵심 과제 몇 개를 정해 메뉴 이름만으로 찾아가게 해 봐요. 헤매며 돌아오는 곳이 이름이 모호한 곳이에요 | 카드 소팅 결과를 그대로 최종 메뉴로 확정 | 강함 (표준 조사법) | Page Laubheimer (NN/g), "Tree Testing: Evaluate Menu Labels and Categories", https://www.nngroup.com/articles/tree-testing/, 2023-08-06 (2026-08-19 재검토) |
| 정보 냄새와 정보 수렵 이론 | 사람은 먹이를 찾는 동물처럼 얻을 가치와 드는 시간을 견주어 갈 곳을 고른다는 이론이에요(피롤리와 카드). 링크 이름, 곁들인 설명, 그림, 앞선 경험이 '냄새'가 되어 그 짐작을 이끌어요 | 링크나 단추 이름만 읽고 눌렀을 때 나올 화면을 맞힐 수 있는지 봐요. 도착 화면 첫 화면에 "맞게 왔다"는 단서가 있는지 봐요 | "더 보기", 브랜드 용어, 뜻 없는 장식 그림, 낚시성 제목 | 강함 (인지 모형 논문과 다수 사용성 관찰) | Raluca Budiu (NN/g), "Information Scent: How Users Decide Where to Go Next", https://www.nngroup.com/articles/information-scent/, 2020-02-02. Peter Pirolli, Stuart Card, "Information Foraging in Information Access Environments", CHI '95, https://www.chi1995.chistatic.hosting.acm.org/proceedings/papers/ppp_bdy.htm, 1995 |
| 시각 정보 탐색 주문 | "먼저 전체를 보여 주고, 확대하고 거르고, 자세한 것은 원할 때." 데이터가 많은 화면의 출발점이라고 슈나이더만이 정리했어요 | 첫 화면이 전체 모습(개수, 분포)을 보여 주는지, 거르기와 확대가 쉬운지, 상세는 눌러야 나오는지 봐요 | 첫 화면부터 상세 표를 다 펼침, 전체 그림 없이 검색창만 둠 | 강함 (정보 시각화 분야에서 가장 널리 인용되는 원칙 중 하나, 단 저자도 "출발점"이라고 함) | Ben Shneiderman, "The Eyes Have It: A Task by Data Type Taxonomy for Information Visualizations", IEEE Symposium on Visual Languages, https://webspace.science.uu.nl/~telea001/uploads/VACourse/Shneiderman96.pdf, 1996-07 |

## 법칙과 효과

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 도허티 임계 (400ms) | 컴퓨터와 사람이 400ms 안에 주고받으면 서로 기다리지 않아 생산성이 오른다는 주장이에요 | 누른 뒤 400ms 안에 무언가(눌림 표시, 스켈레톤)가 보이는지 재요 | 결과가 늦는 동안 아무 반응도 없음, 반대로 일부러 기다리게 해서 "믿음직해 보이게" 하는 꾀를 남용 | 약함 (1982 IBM 보고서 원문을 공개본으로 확인 못 함, 400이라는 숫자는 2차 해석. 반응 시간 한계는 닐슨의 0.1초, 1초, 10초가 더 널리 쓰임) | Jon Yablonski, Laws of UX, "Doherty Threshold", https://lawsofux.com/doherty-threshold/, 날짜 표기 없음 (원 보고서 Doherty, Thadani 1982). 비교 근거 Jakob Nielsen (NN/g), "Response Times: The 3 Important Limits", https://www.nngroup.com/articles/response-times-3-important-limits/, 1993 (2014 보강) |
| 테슬러 법칙 (복잡성 보존) | 모든 시스템에는 없앨 수 없는 복잡함이 있고, 시스템이 떠안거나 사용자가 떠안을 뿐이에요 | 사용자가 직접 정해야 하는 값 중 시스템이 대신 정할 수 있는 것이 있는지 세어 봐요 | "단순하게"라며 옵션만 숨겨 결국 사용자가 다른 곳에서 더 헤맴 | 약함 (실험이 아닌 설계자 경험칙, 래리 테슬러 인터뷰가 출처) | Jon Yablonski, Laws of UX, "Tesler's Law", https://lawsofux.com/teslers-law/, 날짜 표기 없음 (원 출처 Dan Saffer, "Designing for Interaction"의 테슬러 인터뷰, 안내용으로만 사용) |
| 포스텔 법칙 (견고함 원칙) | 원래는 통신 규약의 원칙이에요. "보낼 때는 엄격하게, 받을 때는 너그럽게." UX에서는 입력을 넓게 받아 시스템이 바꿔 주라는 뜻으로 써요 | 전화번호에 띄어쓰기나 붙임표를 넣어도 받는지, 날짜를 여러 형식으로 적어도 알아듣는지 봐요 | 형식이 조금만 달라도 오류를 냄. 반대로 너무 너그러워 뜻이 모호한 입력까지 받아 엉뚱하게 처리 | 보통 (원 출처는 확실한 공학 원칙, UX 적용은 비유) | Jon Postel, RFC 761 "DoD Standard Transmission Control Protocol" 2.10절, https://www.rfc-editor.org/rfc/rfc761, 1980-01. 안내용 Laws of UX, https://lawsofux.com/postels-law/ |
| 피크엔드 규칙 | 사람은 경험 전체가 아니라 가장 강렬한 순간과 끝 장면으로 기억하고 평가해요. 원 실험에서 32명 중 22명(69%)이 더 길지만 끝이 덜 아픈 쪽을 다시 하겠다고 골랐어요 | 흐름에서 가장 답답한 순간(나쁜 정점)이 어디인지 찾고, 마지막 화면이 완료감을 주는지 봐요 | 끝에 "정말 나가시겠어요?" 붙잡기 창, 실패 화면에서 사용자 탓하기 | 보통 (원 실험은 탄탄하나 UI 적용은 사례 중심. NN/g 글은 80%라고 적었지만 원 논문은 69%) | Lexie Kane (NN/g), "The Peak-End Rule", https://www.nngroup.com/articles/peak-end-rule/, 2018-12-30. 원 논문 Kahneman 외, "When More Pain Is Preferred to Less", Psychological Science 4(6), https://ius.uzh.ch/dam/jcr:5ae9adc9-61ec-4174-b37c-4b752f36c23b/Kahnemann%20et%20al.%20-%20When%20More%20Pain%20is%20Preferred%20to%20Less%20(1993).pdf, 1993-11 |
| 목표 경사 효과 | 목표에 가까워질수록 더 빨리 움직여요. 커피 도장 10개 카드에서 끝으로 갈수록 구매 간격이 약 20% 줄었고, 도장 12칸 중 2칸을 미리 찍어 준 카드는 빈 10칸 카드보다 빨리 채웠어요(12.7일 대 15.6일) | 진행 표시가 실제 남은 양을 보여 주는지, 시작하자마자 조금 차 있는지(이미 한 단계 끝난 상태로 시작) 봐요 | 진행 표시가 처음부터 0에서 오래 멈춤. 거짓 진행으로 속이기(기만적 설계와 경계가 얇음) | 강함 (현장 실험, 학술지 게재) | Chicago Booth Review, "Going for the Goal" (Urminsky 인터뷰), https://www.chicagobooth.edu/review/going-goal, 2008-11-01 (원 논문 Kivetz, Urminsky, Zheng, Journal of Marketing Research 43권, 2006) |
| 프레그난츠 (단순성의 법칙) | 사람은 주어진 자극을 가장 단순한 짜임으로 읽어요 | 아이콘이나 배치가 의도와 다른 더 단순한 모양으로 읽히지 않는지 처음 보는 사람에게 물어요 | 겹친 도형을 의도와 달리 한 덩어리로 읽게 그림 | 보통 (현상은 분명하나 정의가 모호하다는 비판이 오래됨, 최근 베이즈 모형으로 정밀화 중) | Wagemans 외, "A Century of Gestalt Psychology in Visual Perception: II. Conceptual and Theoretical Foundations", Psychological Bulletin 138(6), https://pmc.ncbi.nlm.nih.gov/articles/PMC3728284, 2012 |
| 폐쇄성, 좋은 연속성, 공동 운명 | 폐쇄성은 끊긴 윤곽을 닫힌 모양으로 채워 보는 것, 연속성은 매끄럽게 이어지는 선을 하나로 보는 것, 공동 운명은 같이 움직이는 것을 한 묶음으로 보는 것이에요 | 카드 테두리를 없앴을 때도 묶음이 읽히는지, 같이 움직이는 요소가 정말 한 묶음인지 봐요 | 관계없는 요소를 함께 움직이게 해 한 묶음으로 오해하게 만듦 | 강함 (100년 넘게 실험, 일부는 수치로 측정됨) | Wagemans 외, "A Century of Gestalt Psychology in Visual Perception: I. Perceptual Grouping and Figure-Ground Organization", Psychological Bulletin 138(6), https://pmc.ncbi.nlm.nih.gov/articles/PMC3482144, 2012 |
| 전경과 배경 | 화면은 앞에 선 대상(전경)과 뒤(배경)로 나뉘어 읽혀요. 볼록함, 대칭, 작은 영역, 둘러싸임이 전경 단서예요 | 시트나 창이 뒤 화면과 분명히 갈리는지(가림막, 그림자), 글자가 배경 무늬에 묻히지 않는지 봐요 | 사진 위에 글자를 바로 얹어 어느 쪽이 앞인지 흔들림 | 강함 (위와 같은 리뷰) | 위 Wagemans 외 2012, https://pmc.ncbi.nlm.nih.gov/articles/PMC3482144 |
| 균일 연결성 | 선으로 잇거나 같은 바탕에 붙은 요소는 근접성이나 유사성보다 강하게 한 묶음으로 보여요 | 관계를 보여 주려는 요소가 같은 바탕이나 연결선으로 이어졌는지, 반대로 관계없는 것이 이어져 있지 않은지 봐요 | 다른 묶음의 요소를 한 줄 띠 안에 같이 넣음 | 보통 (팔머와 록의 제안, "가장 먼저 처리된다"는 주장에는 반론 있음) | Peterson 1994 논평 요약(팔머와 록 1994 주장 소개), https://experts.arizona.edu/en/publications/the-proper-placement-of-uniform-connectedness/, 1994. 위 Wagemans 외 2012도 같은 논쟁을 정리 |
| 기본값 효과 | 사람은 미리 정해진 값을 대부분 그대로 둬요. 검색 1위와 2위를 몰래 바꿔도 1위 자리가 계속 더 많이 눌렸어요(34% 대 12%) | 기본값이 가장 흔한 사용자의 값인지, 회사에 유리한 값인지 따져요. 알파벳 순서처럼 아무렇게나 정한 기본값이 없는지 봐요 | 기본값을 늘 가장 비싼 선택으로 둠. 동의나 유료 옵션을 미리 체크(한국에서는 법으로 금지) | 강함 (현장 연구 다수, 장기 기증 기본값 연구 등) | Jakob Nielsen (NN/g), "The Power of Defaults", https://www.nngroup.com/articles/the-power-of-defaults/, 2005-09-25 |
| 기준점 효과 (앵커링) | 처음 본 숫자 하나가 뒤의 판단을 끌고 가요. 관계없는 숫자여도 그래요 | 추천 금액, 걸리는 시간 안내, 원래 가격이 실제와 맞는지 봐요. 안내한 시간보다 오래 걸리지 않는지 재요 | 판 적 없는 정가에 취소선, 실제보다 짧게 적은 소요 시간 | 강함 (행동 경제학에서 반복 확인) | Therese Fessenden (NN/g), "The Anchoring Principle", https://nngroup.com/articles/anchoring-principle/, 2018-12-09 |
| 선택 과부하 | 고를 것이 많으면 못 고르거나 만족이 떨어진다는 주장이에요. 2010년 메타분석(50개 실험, 5,036명)은 평균 효과가 거의 0이었고, 2015년 메타분석(99개 관찰, 7,202명)은 선택지가 복잡하고, 과제가 어렵고, 선호가 불확실하고, 빨리 끝내려 할 때만 뚜렷하다고 봤어요 | 선택지 수보다 비교하기 어려운지를 봐요. 초보에게 추천 하나와 기본값이 있는지, 비교 기준이 한 줄로 보이는지 확인해요 | "잼 실험"만 믿고 무조건 선택지를 줄여 필요한 것까지 뺌, 반대로 비교 기준 없이 목록만 늘어놓음 | 약함 (조건부로만 성립, 평균 효과는 재현 논쟁) | Scheibehenne, Greifeneder, Todd, "Can There Ever Be Too Many Options?", Journal of Consumer Research 37(3), https://edoc.unibas.ch/20586, 2010. Chernev, Böckenholt, Goodman, Journal of Consumer Psychology 25(2), https://www.kellogg.northwestern.edu/faculty/research/detail/2015/when-product-assortment-leads-to-choice-overload-a-conceptual, 2015 |

## 설계 원칙 모음

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 슈나이더만의 8가지 황금률 | 일관성, 누구나 쓸 수 있게, 알려 주는 피드백, 끝맺음이 있는 대화(시작, 중간, 끝과 완료 알림), 오류 예방, 쉬운 되돌리기, 사용자가 주도, 단기 기억 부담 줄이기예요 | 8개를 점검표로 화면마다 돌려요. 특히 완료를 알리는지(4번)와 앞 화면 정보를 외워 오게 하는지(8번)는 휴리스틱 10개와 겹치지 않게 따로 봐요 | 작업이 끝났는지 알 수 없는 흐름, 되돌리기 없이 확인 창만 남발 | 강함 (HCI 교과서 6판까지 이어진 원칙) | Ben Shneiderman, "The Eight Golden Rules of Interface Design", https://www.cs.umd.edu/~ben/goldenrules.html, 출처 책 "Designing the User Interface" 6판 2016-05 |
| 접근성 4원칙 (POUR) | 인식할 수 있게(Perceivable), 조작할 수 있게(Operable), 이해할 수 있게(Understandable), 여러 보조 기술에서 견고하게(Robust). WCAG의 모든 기준은 이 넷 아래에 있어요 | 화면 읽기 프로그램으로 읽어 보기(인식), 키보드만으로 끝까지 가기(조작), 오류 문구가 고칠 방법을 말하는지(이해), 표준 요소를 썼는지(견고) 봐요 | 대비와 누름 크기만 맞추고 키보드 이동과 화면 읽기는 안 해 봄 | 강함 (W3C 국제 표준) | W3C WAI, "Understanding WCAG 2.1: Introduction", https://www.w3.org/WAI/WCAG21/Understanding/intro, 2025-07-15 갱신 |

## 감정과 윤리

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 감정 디자인 3단계 (본능, 행동, 성찰) | 본능 단계는 첫인상과 겉모습, 행동 단계는 쓰는 동안의 느낌, 성찰 단계는 쓰고 난 뒤 "이게 나를 어떻게 보이게 하나"예요 | 첫 화면 5초 인상(본능), 핵심 과제를 막힘 없이 끝내는지(행동), 결과를 남에게 보여 주고 싶은지(성찰)를 따로 물어요 | 겉모습만 다듬고 쓰는 중 막힘을 남겨 성찰 단계에서 배신감을 줌 | 보통 (영향력 큰 이론 틀이지만 실험으로 검증된 모형은 아님) | Don Norman, "Emotional Design", https://jnd.org/emotional-design/, 2008-11-17. Therese Fessenden (NN/g), "The 3 Levels of Emotional Processing" 영상, https://www.nngroup.com/videos/3-levels-emotional-processing/, 2022-05-27 |
| 즐거움과 사용성의 순서 (표면 즐거움, 깊은 즐거움) | 쓸모, 믿을 만함, 쓰기 쉬움이 먼저 채워져야 즐거움이 의미가 있어요. 애니메이션과 재치 있는 문구 같은 표면 즐거움은 바탕이 약하면 오히려 거슬려요 | 즐거움 요소를 다 빼고도 과제가 막힘 없이 끝나는지 먼저 봐요 | 막히는 흐름은 두고 축하 효과와 캐릭터 대사부터 넣음 | 보통 (실무 모형, 아론 월터의 욕구 피라미드에 기댐) | Therese Fessenden (NN/g), "A Theory of User Delight", https://www.nngroup.com/articles/theory-user-delight/, 2017-03-05 |
| 기만적 설계 (다크 패턴) | 속임, 주의 돌리기, 창피 주기, 방해로 사용자를 회사에 유리한 쪽으로 미는 설계예요. 몰래 끼워 넣기, 해지 어렵게, 미리 체크, 숨은 비용, 헷갈리는 말, 가짜 긴급함, 반복 조르기, 창피 주기 등이 있어요. 설득과의 차이는 내용이 사실이고 정보를 숨기지 않는지예요 | 가입과 해지 단계 수를 비교해요. 미리 체크된 항목, 거절 단추 문구("아니요, 혜택 필요 없어요"), 결제 직전 늘어나는 금액, 거짓 재고와 마감을 찾아요. 가장 취약한 사용자(바쁜 사람, 글 읽기 어려운 사람)를 가정해 걸어 봐요 | 전환율을 위해 미리 체크와 거절 창피 주기를 둠, 긍정 후기만 앞에 두고 부정 후기는 "더 보기" 안에 숨김 | 강함 (FTC 보고서, 법 집행 사례 다수, 한국 법 시행) | Maria Rosala (NN/g), "Deceptive Patterns in UX", https://www.nngroup.com/articles/deceptive-patterns/, 2023-12-01. Harry Brignull 외, "Types of deceptive pattern", https://www.deceptive.design/types, 날짜 표기 없음. FTC, "Bringing Dark Patterns to Light", https://www.ftc.gov/system/files/ftc_gov/pdf/P214800%20Dark%20Patterns%20Report%209.14.2022%20-%20FINAL.pdf, 2022-09 |
| 한국 규제 메모 | 개정 전자상거래법이 2025-02-14부터 6개 유형을 직접 규율해요. 숨은 갱신(정기결제 증액이나 유료 전환 때 따로 동의), 순차 공개 가격, 특정 옵션 미리 선택, 잘못된 계층 구조(해지 단추를 흐리게 등), 취소와 탈퇴 방해, 반복 간섭이에요. 위반하면 시정조치, 영업정지나 과징금, 500만 원 이하 과태료가 가능해요 | 유료 기능이 생기면 이 6개를 결제와 해지 화면마다 점검해요. 이전 배송지 미리 고르기 같은 단순 편의는 예외예요 | 무료 기간 끝나면 알림 없이 유료로 넘어감 | 강함 (법률) | 뉴시스, "다크패턴 신규 규제에 혼선 없도록, 6개 유형별 궁금증 해소[Q&A]", https://www.newsis.com/view/NISX20250213_0003063585, 2025-02-13 |

## 제품과 검증

| 이론 | 무엇을 말하나 | 화면에서 이렇게 확인 | 흔한 실수 | 근거 세기 | 출처 |
|---|---|---|---|---|---|
| 카노 모형 | 기능을 기본(없으면 화나고 있어도 당연), 성능(좋을수록 비례해 만족), 감동(없어도 괜찮지만 있으면 크게 기쁨)으로 나눠요. 감동은 시간이 지나며 성능, 기본으로 내려가요 | 기능 후보표에 세 칸을 두고, 기본 기능이 흠 없이 되는지부터 확인한 뒤 감동 기능에 손대요 | 기본 기능이 불안한데 감동 기능부터 만듦, 경쟁사 감동 기능을 베껴 감동이 안 됨 | 보통 (1980년대 품질 경영 이론, 설문 분류법은 있으나 UX 연구 근거는 실무 중심) | Christian Holst (Baymard Institute), "UX and the Kano model", https://baymard.com/blog/kano-model, 2012-02-07 |
| 해야 할 일 이론 (JTBD) | 사람은 자기 상황에서 나아지려고 제품을 '고용'해요. 나이나 기능 목록이 아니라 그 일의 기능적, 사회적, 감정적 이유를 봐요. 아침 밀크셰이크의 진짜 경쟁자는 바나나와 베이글이었어요 | "사용자가 이 화면을 켜는 순간 어떤 상황이고 무엇을 끝내고 싶은가"를 한 문장으로 적을 수 있는지 봐요 | 사용자 유형 설명만 있고 상황과 목적이 없음, 같은 경쟁 제품만 봄 | 보통 (경영학 사례 연구 중심, 통제 실험 근거는 적음) | Christensen Institute, "Jobs to Be Done", https://www.christenseninstitute.org/theory/jobs-to-be-done/, 날짜 표기 없음. Christensen 외, "Know Your Customers' Jobs to Be Done", Harvard Business Review, https://hbr.org/2016/09/know-your-customers-jobs-to-be-done, 2016-09 |
| 5명 사용성 시험 | 한 사람이 문제의 약 31%를 찾고, 5명이면 약 85%를 찾아요. 큰 시험 한 번보다 5명씩 여러 번 고치며 시험하는 편이 나아요. 사용자 집단이 뚜렷이 다르면 집단마다 3~4명이에요 | 기능 하나 끝날 때마다 5명 안쪽으로 시험했는지, 고친 뒤 다시 시험했는지 봐요 | 5명으로 숫자(성공률 몇 %)까지 주장함, 다른 집단을 섞어 5명만 봄 | 강함 (모형과 오랜 실무 근거, 단 질적 시험에 한함) | Jakob Nielsen (NN/g), "Why You Only Need to Test with 5 Users", https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/, 2000-03-18 |
| 소리 내어 생각하기 | 사용자가 과제를 하며 생각을 말로 계속 꺼내게 하고, 진행자는 조용히 들어요. 왜 틀리게 짐작했는지가 드러나요 | 진행자가 힌트를 주거나 유도 질문을 하지 않았는지 기록을 다시 봐요 | 진행자가 설명을 해 버림, 말한 의견(좋아요)을 실제 행동보다 믿음 | 강함 (가장 널리 쓰이는 사용성 방법) | Jakob Nielsen (NN/g), "Thinking Aloud: The #1 Usability Tool", https://www.nngroup.com/articles/thinking-aloud-the-1-usability-tool/, 2012-01-15 |
| SUS (시스템 사용성 척도) | 시험 뒤 10문항 5점 척도로 0~100점을 내요. 약 500개 연구 평균이 68점이라 68보다 높으면 평균 이상이에요 | 같은 화면을 고치기 전후로 같은 설문을 돌려 점수를 비교해요 | 점수를 백분율로 읽음(68점은 68%가 아님), 5명 점수로 큰 결론 | 강함 (1986년부터 쓰인 표준 설문, 대규모 기준값) | Jeff Sauro (MeasuringU), "Measuring Usability with the System Usability Scale (SUS)", https://measuringu.com/sus/, 2011-02-03 |
| AI 평가와 실제 시험 | AI가 만든 가짜 사용자는 얕고 너무 호의적인 답을 하고, 실제 행동 자료를 만들 수 없어요. 가설 만들기와 시험 준비에는 쓰되 결과를 실제 사용자 결과처럼 쓰면 안 돼요 | AI 화면 점검 결과를 "가설"로 적고, 실제 사람 시험으로 확인한 것과 나눠 적었는지 봐요 | AI 비평만 받고 "검증 끝"이라고 보고 | 보통 (NN/g 비교 연구, 분야가 빠르게 변함) | Maria Rosala, Kate Moran (NN/g), "Synthetic Users: If, When, and How to Use AI-Generated Research", https://www.nngroup.com/articles/synthetic-users/, 2024-06-21 |

## 뺀 것과 이유

| 뺀 것 | 이유 | 다시 볼 조건 |
|---|---|---|
| 파레토 법칙 (80/20) | UX 쪽 1차 연구나 NN/g 근거를 못 찾았고, 경제학 관찰을 비유로 옮긴 경험칙이에요 | 기능별 사용량 자료가 생겨 실제 분포를 잴 수 있을 때 |
| 오컴의 면도날 | 철학 원칙이라 화면 점검 기준으로 바꿀 근거가 없어요. "같은 일을 하면 단순한 쪽"은 이미 인지 부하와 테슬러 법칙 줄에서 다뤄요 | 없음 |
| 사회적 증거, 희소성 같은 설득 기법 | 사실이면 설득, 거짓이면 기만이라 기만적 설계 줄의 판단 기준으로 대신해요 | 판매나 결제 화면을 만들 때 따로 정리 |

## 확인 못 한 것

- 도허티와 타다니 1982 IBM 보고서 원문: IBM 페이지가 열리지 않아(인증서 오류 뒤 "표시할 수 없음") 400ms라는 숫자가 원문에 있는지 확인 못 했어요.
- 폰 레스토프 1933 원 논문과 헌트 1995 리뷰("What von Restorff really did"): 검색 요약만 봤어요. 요약에 따르면 헌트는 "눈에 띄는 것"이 기억 향상의 필수 조건은 아니라고 했어요. 원문은 열지 못했어요.
- 테슬러 법칙의 원 출처(Dan Saffer 책의 테슬러 인터뷰): 책을 열지 못했고, NN/g 복잡한 앱 글(Kate Kaplan, 2020-11-08)에도 이 법칙 언급은 없었어요.
- 목표 경사 효과 원 논문(Kivetz 외 2006): 컬럼비아 대학 페이지가 접근 거부(403)여서 시카고 부스 리뷰 기사로 숫자를 확인했어요.
- 존슨과 골드스타인 2003 "Do Defaults Save Lives?"의 나라별 동의율 숫자: 요약 페이지에 숫자가 없어 표에 넣지 않았어요.
- 자이가르닉 메타분석에 들어간 연구 수: 초록 페이지에 없었고, 검색 요약의 "37개 연구, 비율 0.99"는 원문으로 확인 못 했어요.
- 사이먼스와 차브리스 1999 고릴라 원 실험의 못 본 비율: 열린 자료에 숫자가 없었어요. 표의 83%는 2013년 영상의학과 의사 실험 숫자예요.
- NN/g의 카노 모형 글과 게슈탈트 폐쇄성, 전경과 배경 글: 검색으로 찾지 못해 바이마드 글과 학술 리뷰로 대신했어요.
- 카노 모형과 JTBD의 원전(카노 1984 논문, 크리스텐슨 책)은 열지 않았어요.
- 한국 전자상거래법 조문 원문: 법제처 원문 대신 기사로 확인했어요. 과태료 금액과 조항 번호는 법제처에서 다시 확인하면 좋아요.
