<!-- 이 파일은 비공개 설정 저장소의 Actions가 만듭니다. 여기서 고치면 다음 빌드에 덮어씁니다. -->

### 만들고 있는 것들

설계부터 배포까지 혼자 맡아 만드는 웹 서비스, 게임, 개발 도구를 모았습니다. 서비스는 대부분 Cloudflare 무료 구성(Pages·Workers·D1)으로 운영합니다.

#### 이렇게 만듭니다

- **AI와 함께, 여러 갈래로 동시에.** Claude Code 세션을 기능마다 나눠 띄우고, 통합 세션이 결과를 모아 병합과 배포를 맡습니다. 휴대폰에서도 진행 상황을 보고 다음 일을 맡깁니다. 최근 30일 동안 저장소 9곳에서 PR 685개를 이렇게 병합했습니다.
- **설계 문서부터, 다른 AI의 검토를 거쳐.** 기능마다 설계와 구현 계획을 문서로 먼저 쓰고, Codex 같은 다른 모델이 짚은 문제를 반영한 뒤에 구현합니다. 기출문항 추출처럼 틀리면 안 되는 일은 두 모델이 따로 만든 결과를 대조합니다.
- **한 번 만들어 같이 쓰기.** 여러 서비스에 필요한 로그인·기기 세션, 카카오 공유, UI 부품, 색 팔레트는 공용 패키지로 만들어 GitHub Packages에 발행하고, 서비스마다 버전을 골라 씁니다. 색 팔레트 10종은 한 번 만들어 앱 다섯 곳에 같은 날 넣었습니다.
- **필요한 도구는 직접.** 리뷰 지적을 싼 모델 둘에게 고치게 하는 cascade-fix, 문서 색인 doclookup, 게임 50장을 혼자 끝까지 깨 보는 규칙 AI, 기출문항 검수 파이프라인처럼 개발하며 되풀이되는 일은 도구로 만듭니다. Claude Code 플러그인은 마켓플레이스 저장소 하나에 모아 공개합니다.
- **기계가 확인하고, 사람은 눈으로 볼 것만.** 테스트·타입 검사·빌드·CI를 통과해야 병합하고, 화면을 직접 봐야 하는 것만 확인 목록으로 남깁니다. 새 기능에는 써 볼 날짜를 정해 두고, 그때까지 쓰지 않은 것은 걷어냅니다.

#### 프로젝트

<sub>프로젝트 14개 · 운영 중인 사이트 4개 · 마지막 업데이트 2026.11.21</sub>

<p>
<a href="https://gazua.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/gazua-dark-2098b65c.svg"><img src="cards/gazua-light-fc3c26d5.svg" width="400" alt="가즈아 — 관심종목을 한 차트에서 비교하고 시험하는 주식 앱"></picture></a>
<a href="https://landmark.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/landmark-dark-312c2b06.svg"><img src="cards/landmark-light-964fc21e.svg" width="400" alt="랜드마크 — 평소에 모아 두고, 여행 때 꺼내 쓰는 장소 보관함"></picture></a>
<a href="https://repass.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/repass-dark-96088a32.svg"><img src="cards/repass-light-364ddb2b.svg" width="400" alt="리패스 — 기출문제로 회차를 섞은 모의고사"></picture></a>
<a href="https://belorn.sch0718.dev"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/belorn-dark-aebbede9.svg"><img src="cards/belorn-light-d594c3fe.svg" width="400" alt="벨로른 변경 전기 — 브라우저에서 하는 칸 전투 전술 RPG"></picture></a>
<a href="https://github.com/sch0718/claude-plugins"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/claude-plugins-dark-45406732.svg"><img src="cards/claude-plugins-light-76d2db8c.svg" width="400" alt="claude-plugins — 직접 만든 Claude Code 플러그인 마켓플레이스"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/cascade-fix"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/cascade-fix-dark-f0254b72.svg"><img src="cards/cascade-fix-light-e3d84112.svg" width="400" alt="cascade-fix — 리뷰 지적을 싼 모델 둘이 고치고, 갈린 것만 Opus가 판가름"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/fanout"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/fanout-dark-7f27d9f8.svg"><img src="cards/fanout-light-6f2d96e5.svg" width="400" alt="fanout — 고칠 것들을 하위 세션에 나눠 맡기고 PR 병합·정리까지"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/doclookup"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/doclookup-dark-a934dfdb.svg"><img src="cards/doclookup-light-5e9d4b1f.svg" width="400" alt="doclookup — 문서를 절 단위로 색인해 쓰임과 같이 고칠 곳을 찾기"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/session-move"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/session-move-dark-3ca373e9.svg"><img src="cards/session-move-light-ed953678.svg" width="400" alt="session-move — Code 탭 세션을 다른 계정·다른 기기로 옮기기"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/offline-doc-bundle"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/offline-doc-bundle-dark-ad058bfd.svg"><img src="cards/offline-doc-bundle-light-ffd9c2b1.svg" width="400" alt="offline-doc-bundle — 마크다운을 인터넷 없이 열리는 HTML·PDF 묶음으로"></picture></a>
<a href="https://github.com/sch0718/claude-plugins/tree/HEAD/plugins/architecture-motion"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/architecture-motion-dark-99d42bb5.svg"><img src="cards/architecture-motion-light-d58ab3c0.svg" width="400" alt="architecture-motion — 구성 변화·요청 흐름·장애 전파를 움직이는 그림으로"></picture></a>
<a href="https://github.com/sch0718/sch0718-toolkit-web"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/sch0718-toolkit-web-dark-6c670a45.svg"><img src="cards/sch0718-toolkit-web-light-3c3f4df5.svg" width="400" alt="toolkit-web — 웹 서비스들이 함께 쓰는 TypeScript 패키지 모음"></picture></a>
<a href="https://github.com/sch0718/sch0718-toolkit-python"><picture><source media="(prefers-color-scheme: dark)" srcset="cards/sch0718-toolkit-python-dark-a623c1d2.svg"><img src="cards/sch0718-toolkit-python-light-6df9611b.svg" width="400" alt="toolkit-python — Python 백엔드가 함께 쓸 패키지 모음"></picture></a>
<picture><source media="(prefers-color-scheme: dark)" srcset="cards/smarthome-dark-e534e101.svg"><img src="cards/smarthome-light-11d8e96e.svg" width="400" alt="smarthome — Home Assistant로 묶는 우리 집과 TV 에이전트"></picture>
</p>
