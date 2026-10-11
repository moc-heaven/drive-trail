# drive-trail

하례마을 프로그램의 차량 이동 구간에서, 참여자 각자의 폰으로 듣는 위치기반 사운드 안내.
꿈꾸는고물상 관리. 주소: https://drive.harye.kr

## 쓰는 법
- 1코스: https://drive.harye.kr/#c1
- 2코스: https://drive.harye.kr/#c2
- 출발 전 '출발 · 소리 켜기'를 한 번 누르고, 화면을 켠 채 거치대에 둡니다.

## 폴더
- `index.html` 앱 본체
- `trails/index.json` 코스 목록
- `trails/c1.json`, `trails/c2.json` 코스별 지점, 대본, 도착 시점, 음원·이미지 경로
- `audio/` 배경음악과 나레이션 (mp3 권장)
- `images/` 지점 이미지 (가로 1200px 정도 jpg)

## 코스 파일 항목
- `bgm`: 배경음악 경로 (예: `audio/c1-bgm.mp3`). 비워 두면 임시 음악
- `points[]`: 순서대로 재생되는 이야기 지점
  - `lat`, `lng`: 이야기 대상의 위치
  - `cue`: 나레이션 시작 후 대상이 보여야 하는 초. 속도에 맞춰 재생 시작 거리를 계산
  - `maxLead`: 재생 시작 거리 상한(m)
  - `audio`, `image`: 파일 경로. 비워 두면 음성 합성과 빈 이미지

## 원칙
작업 중 초안과 메모 녹음은 이 저장소에 올리지 않습니다. 저장소는 공개입니다.
