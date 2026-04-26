
# 2026-04-25

Date: April 25, 2026

Subject: Linux_VI

Parent item: Linux_VI (https://www.notion.so/Linux_VI-34aede1d1e69804c9726e61c54acbaa3?pvs=21)

태그: 실습, 이론

| gg, G | 문서의 맨 첫 줄(마지막줄)로 이동 | :%s/A/B/g | 문서 전체에서 A를 B로 모두 치환 |
| --- | --- | --- | --- |
| o | 다음 줄에 빈 줄을 삽입하여 입력 모드로 전환 | cw, #cw | 단어 삭제 후 바로 입력 모드 전환 |
| dd | 한 줄 삭제 | yy | 한 줄 복사 |

## 📝 [vi 연습 문제 1: 기본 입력 & 이동]

🚩 **목표:** vi의 기본 모드 전환과 커서 이동 익히기

💻 [실습 텍스트]

Seoul
Busan
Incheon
Daegu
Daejeon

 ✅ 미션

1. 파일을 열고 위 텍스트를 입력합니다.
2. 명령 모드에서 `gg`를 눌러 맨 첫 줄로 이동합니다.
3. `j`를 눌러 한 줄씩 아래로 내려가 봅니다.
4. **Busan**을 **Jeju**로 수정합니다. (`cw` 또는 `R` 활용)
5. `G`를 눌러 맨 아래 줄로 이동한 후, `o`를 눌러 다음 줄에 **Gwangju**를 추가합니다.
6. `:wq`를 입력하여 저장하고 종료합니다.

---

## 📝 [vi 연습 문제 2: 삭제, 복사, 붙여넣기]

🚩 **목표:** 편집의 핵심인 복사와 삭제(잘라내기) 및 복구 기능 익히기

💻 [실습 텍스트]
HTML
CSS
JavaScript
Python
Java
C

✅ 미션

1. **CSS** 줄에서 `dd`를 눌러 삭제합니다.
2. **Python** 줄에서 `yy`로 복사한 후, 맨 아래 줄에서 `p`를 눌러 붙여넣습니다.
3. **JavaScript** 줄을 삭제(`dd`)했다가, `u`를 눌러 다시 복구합니다.
4. **C** 줄을 `yy`로 복사한 후, 그 줄 위에서 `P`(대문자)를 눌러 붙여넣습니다.
5. **HTML** 줄을 복사하여 원하는 곳에 두 번 연속으로 붙여넣어 봅니다.

## 📝 [vi 연습 문제 3: 검색 & 치환]

🚩 **목표:** 특정 단어를 찾고 한꺼번에 변경하는 고급 기능 익히기

💻 [실습 텍스트]

error: file not found
info: process started
error: connection lost
warning: low memory
error: timeout

✅ **미션:**

1. `/error`를 입력해 검색한 후, `n`을 눌러 다음 검색 결과로 이동해 봅니다.
2. 문서 전체의 모든 **error**를 **ERROR**로 일괄 변경합니다. (`:%s/error/ERROR/g`)
3. **warning**을 **WARN**으로 변경합니다.
4. **info**가 포함된 줄에서 커서를 **process**에 두고 `cw`를 입력해 **task**로 변경합니다.
5. **timeout**이 포함된 줄을 찾아 삭제합니다. (`dd`)

---

<img width="1003" height="834" alt="화면_캡처_2026-04-25_070759" src="https://github.com/user-attachments/assets/8fe56418-590d-432d-b910-7969711752d9" />
<img width="1010" height="161" alt="화면_캡처_2026-04-25_070854" src="https://github.com/user-attachments/assets/8347bff3-1b9b-4eaf-bf81-567179f06931" />

---
