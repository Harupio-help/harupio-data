# Harupio(하루피오) — 받는 자료 (공개 사본)

이 폴더의 `.json` 파일은 앱스토어판 「하루 한 문장」이 사용자가 「추가 자료 받기」를 누를 때 받는 자료입니다. 허가 조건(크리에이티브 커먼즈의
기술적 보호조치 금지 · Arphic Public License 의 「받는 이에게 더 제한을 두지 말 것」)을 지키려고 앱 묶음(App Store)에 넣지 않고, 여기에 DRM 없이 공개합니다.
누구나 같은 허가 조건으로 받고, 바꾸고, 다시 나눌 수 있습니다.
각 파일은 JSON 객체 `{"변수 이름": 값}` 이고(실행 코드 없음), 큰 자료는 gzip + base64 문자열로 묶었습니다. 파일 이름의 끝 12자리와 `manifest.json` 은 sha256 입니다.

| 파일 | 원 자료 · 저작자 | 허가 | 바꾼 것 |
|---|---|---|---|
| `ja-stroke-*.json` (`STROKE_B64`) | KanjiVG © Ulrich Apel (kanjivg.tagaini.net) | CC BY-SA 3.0 — https://creativecommons.org/licenses/by-sa/3.0/ | 이 앱에 나오는 글자만 골라 좌표를 소수 한 자리로 줄이고 JSON 으로 묶음, 가나 · 々 등을 더함 |
| `en-voc-*.json` (`LV_VOC`, 영어 과정 레벨 단어) | 낱말 고르기: wordfreq © Robyn Speer (데이터 CC BY-SA 4.0) 빈도 상위 원형 8,000개 · 원형 묶기 simplemma (MIT) | CC BY-SA 4.0 — https://creativecommons.org/licenses/by-sa/4.0/ | AI 가 CEFR 수준 · 학술 어휘 여부를 판정(공식 목록 아님) · 뜻 · 예문 · 일본어 번역은 AI 가 새로 씀 |
| `zh-stroke-*.json` (`STROKE_B64`, 중국어 획순) | Make Me a Hanzi (github.com/skishore/makemeahanzi) graphics.txt — Arphic PL KaitiM GB · Arphic PL UKai 글꼴에서 만든 자료 | Arphic Public License — 전문 `ARPHICPL.TXT` | 이 앱의 중국어 자료에 나오는 글자의 줄만 골라 그대로(줄 안은 바꾸지 않음) gzip · base64 로 묶음. 바꾼 내력은 `hanzi-stroke-README.md` |

원 자료의 저작자는 이 앱과 관계가 없으며 이 앱을 보증하지 않습니다. 자료에는 어떤 보증도 없습니다.
