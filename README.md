<!-- 이 파일은 비공개 설정 저장소의 Actions가 만듭니다. 여기서 고치면 다음 빌드에 덮어씁니다. -->

### 만들고 있는 것들

설계부터 배포까지 혼자 맡아 만드는 웹 서비스, 게임, 개발 도구를 모았습니다. 서비스는 대부분 Cloudflare 무료 구성(Pages·Workers·D1)으로 운영합니다.

#### 이렇게 만듭니다

- **AI와 함께, 여러 갈래로 동시에.** Claude Code 세션을 기능마다 나눠 띄우고, 통합 세션이 결과를 모아 병합과 배포를 맡습니다. 휴대폰에서도 진행 상황을 보고 다음 일을 맡깁니다. 최근 30일 동안 저장소 12곳에서 PR 734개를 이렇게 병합했습니다.
- **설계 문서부터, 다른 AI의 검토를 거쳐.** 기능마다 설계와 구현 계획을 문서로 먼저 쓰고, Codex 같은 다른 모델이 짚은 문제를 반영한 뒤에 구현합니다. 기출문항 추출처럼 틀리면 안 되는 일은 두 모델이 따로 만든 결과를 대조합니다.
- **한 번 만들어 같이 쓰기.** 여러 서비스에 필요한 로그인·기기 세션, 카카오 공유, UI 부품, 색 팔레트는 공용 패키지로 만들어 GitHub Packages에 발행하고, 서비스마다 버전을 골라 씁니다. 색 팔레트 10종은 한 번 만들어 앱 다섯 곳에 같은 날 넣었습니다.
- **필요한 도구는 직접.** 리뷰 지적을 싼 모델 둘에게 고치게 하는 cascade-fix, 문서 색인 doclookup, 게임 50장을 혼자 끝까지 깨 보는 규칙 AI, 기출문항 검수 파이프라인처럼 개발하며 되풀이되는 일은 도구로 만듭니다.
- **기계가 확인하고, 사람은 눈으로 볼 것만.** 테스트·타입 검사·빌드·CI를 통과해야 병합하고, 화면을 직접 봐야 하는 것만 확인 목록으로 남깁니다. 새 기능에는 써 볼 날짜를 정해 두고, 그때까지 쓰지 않은 것은 걷어냅니다.

#### 프로젝트

<sub>프로젝트 9개 · 운영 중인 사이트 4개 · 마지막 업데이트 2026.11.19</sub>

<p>
<a href="https://gazua.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/gazua-dark-99f53e22.svg"><img src="cards/gazua-light-7c438245.svg" width="400" alt="가즈아 — 관심종목을 한 차트에서 비교하고 시험하는 주식 앱"></picture></a>
<a href="https://landmark.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/landmark-dark-81d15422.svg"><img src="cards/landmark-light-0a2ab4c0.svg" width="400" alt="랜드마크 — 평소에 모아 두고, 여행 때 꺼내 쓰는 장소 보관함"></picture></a>
<a href="https://repass.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/repass-dark-a1b41f88.svg"><img src="cards/repass-light-0f45b17b.svg" width="400" alt="리패스 — 기출문제로 회차를 섞은 모의고사"></picture></a>
<a href="https://belorn.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/belorn-dark-ee4c2cdf.svg"><img src="cards/belorn-light-ab6e7420.svg" width="400" alt="벨로른 변경 전기 — 브라우저에서 하는 칸 전투 전술 RPG"></picture></a>
<picture><source media="(prefers-color-scheme: dark)" srcset="cards/cascade-fix-dark-cead8864.svg"><img src="cards/cascade-fix-light-358e5cd0.svg" width="400" alt="cascade-fix — 리뷰 지적을 싼 모델 둘이 고치고, 갈린 것만 Opus가 판가름"></picture>
<picture><source media="(prefers-color-scheme: dark)" srcset="cards/doclookup-dark-60461c94.svg"><img src="cards/doclookup-light-4be60124.svg" width="400" alt="doclookup — 문서를 절 단위로 색인해 쓰임과 같이 고칠 곳을 찾기"></picture>
<a href="https://github.com/sch0718/sch0718-toolkit-web"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/sch0718-toolkit-web-dark-04b3efe9.svg"><img src="cards/sch0718-toolkit-web-light-0c20868f.svg" width="400" alt="toolkit-web — 웹 서비스들이 함께 쓰는 TypeScript 패키지 모음"></picture></a>
<a href="https://github.com/sch0718/sch0718-toolkit-python"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/sch0718-toolkit-python-dark-7d7ec207.svg"><img src="cards/sch0718-toolkit-python-light-14c08554.svg" width="400" alt="toolkit-python — Python 백엔드가 함께 쓸 패키지 모음"></picture></a>
<picture><source media="(prefers-color-scheme: dark)" srcset="cards/smarthome-dark-e534e101.svg"><img src="cards/smarthome-light-11d8e96e.svg" width="400" alt="smarthome — Home Assistant로 묶는 우리 집과 TV 에이전트"></picture>
</p>
