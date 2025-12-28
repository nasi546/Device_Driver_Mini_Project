# Device Driver Mini Project (Raspberry Pi 4B)
**Linux Device Driver + User-space Daemon + systemd/udev 자동화**로 구성된 미니 프로젝트입니다.  
DHT11(온습도) / DS1302(RTC) / Rotary Encoder / SSD1306 OLED / 8ch LED Bar를 하나의 흐름으로 묶어 **부팅 시 자동 동작**하도록 만들었습니다.

> 목표: “드라이버만 만든 데모”가 아니라, **커널 ↔ 유저스페이스 ↔ 운영(systemd/udev)** 까지 연결된 작은 제품 형태로 완성하기

---

## ✨ What it does
- **DHT11**에서 온/습도 읽기
- **Rotary Encoder**로 임계값(예: 습도 경고 기준) 조절
- **OLED(SSD1306 I2C)**에 시간/온습도/임계값 표시
- **8채널 LED Bar**로 온습도 레벨 게이지 표현
- **DS1302 RTC**로 시간 유지(전원 오프 후에도 시간 보존)
- systemd/udev로 **커널 모듈 로드 + 데몬 실행 자동화**

---

## 🎬 Demo (영상/스크린샷)
> 아래 자료는 곧 추가됩니다.

- ✅ **Demo Video**: `docs/videos/demo.mp4` (or YouTube Link)
- ✅ **GIF Preview**: `docs/videos/demo.gif`
- ✅ **Photos**: `docs/images/real-wiring.jpg`, `docs/images/oled-screen.jpg`

예시(파일 추가 후 자동 표시):
```text
docs/
 ├─ images/
 │   ├─ schematic.png
 │   ├─ real-wiring.jpg
 │   └─ oled-screen.jpg
 └─ videos/
     ├─ demo.gif
     └─ demo.mp4
```
