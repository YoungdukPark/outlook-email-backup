# Outlook Email Archiver (아웃룩 메일 아카이버)  
> **한 번의 클릭으로 아웃룩 메일을 로컬 폴더에 HTML + 첨부 파일 형태로 백업합니다**

![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue.svg)
![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)

---

## 📖 개요
아웃룩 기본 폴더(받은 편지함·보낸 편지함)를 범위·날짜별로 선택하여  
✓ 본문 ✓ 첨부 ✓ 인라인 이미지를 *완전 보존*한 채 HTML로 저장하고,  
진행률·로그를 실시간으로 표시합니다.  
오프라인에서도 메일을 브라우저로 쉽게 열람할 수 있습니다.

---

## ✨ 주요 기능
| 기능 | 설명 |
|------|------|
| **날짜 범위 선택** | 오늘·최근 7일·최근 30일·사용자 지정 |
| **폴더 지정** | 받은 편지함•보낸 편지함 개별/동시 백업 |
| **첨부 파일 보존** | 원본 파일명 유지, `attachments/` 하위 폴더에 저장 |
| **인라인 이미지 추출** | CID 이미지를 `inline/` 에 저장 후 HTML 경로 수정 |
| **HTML 렌더링** | 헤더(발신·수신·제목·날짜) + 본문(HTMLBody) |
| **폴더 구조화** | `YYMM/` → `YYYYMMDD_보낸사람_제목[_첨부]/mail.htm` |
| **실시간 진행률** | ProgressBar·남은 개수·속도 표시 |
| **로깅** | `backup.log` 에 정보·오류 기록, 재시도 가능 |

---

## 🎬 데모
> `docs/demo.gif` 또는 `docs/screenshots/` 경로에 GIF·PNG를 넣어주세요  

---

## ⚙️ 사전 요구 사항
* **Python 3.10 이상**
* Outlook (2016 이상 / Microsoft 365 버전 권장)
* Windows 10/11
* 의존 패키지  
  ```bash
  pip install -r requirements.txt  # pywin32, tkcalendar, pillow 등
