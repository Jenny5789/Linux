
# 2026-04-23

Date: April 23, 2026

Subject: Linux_VI

Parent item: Linux_VI (https://www.notion.so/Linux_VI-34aede1d1e69804c9726e61c54acbaa3?pvs=21)
태그: 실습, 이론

<aside>
💡

- ‘i’(현재 커서 위치, insert) ,’a’(다음 칸, append) 텍스트 입력, ‘o’( 현재 줄 바로 아래 새로운 줄 만들며 입력 시작, open line)
- ‘x’(문자 1개 삭제), ‘dd’(커서 있는 줄 삭제),  ‘u’ (되돌리기)
- ‘yy’( 현재 줄 복사), ‘P’(위에 붙이기, upper case), ‘p’(아래 붙이기, lower case)  ‘5yy’는 5줄 복사  {‘yy’  후 ‘P’ : 현재 줄 복사 후 위에 붙이기}
- ‘/apple’ 입력 후 enter → ‘n’ (next, 다음 찾기)누르면 다음 ‘ apple’ 로 커서가 이동, ’N’ (이전 찾기,‘shift + n’)을 누르면 반대 방향으로 이동
- ‘gg’ ( 1번째 줄, 문서의 최상단으로 이동), ‘G’(마지막 줄, 문서의 최하단으로 이동)
- ‘0’(숫자 0 , 해당 줄의 맨 앞으로 이동), ‘$’ (해당 줄의 맨 끝으로 이동)
- ‘:wq’(write & quit) 로 저장 후 종료, ’:q!’(저장하지 않고 강제 종료), ‘:w’(종료하지 않고 저장만 하기)
</aside>

---

## 📝 [기본 생존 & 편집 복습]

🚩 목표: 오타 수정과 저장 익히기

💻 [실습 텍스트]
Linux is a free and open-source operating system.
The kernel was first released on October 5, 1991, by Linus Torvalds.
Vi is a powerfull text editor. (← 일부러 오타 'powerfull')

✅ 미션:

1. 위 세 줄을 입력합니다 (i 누르기).
2. 'Esc'를 누르고 'l'키로 이동해 'powerfull'의 마지막 'l'을 'x'로 지웁니다.
3. ':wq'로 저장하고 나옵니다.

---

## 📝  [복사왕의 기술 (yy, p)]

🚩 목표: 반복되는 코드를 순식간에 작성하기

💻 [실습 텍스트]

AllowUser: admin
Permission: ReadOnly

✅ 미션:

1. 'AllowUser: admin' 줄에 커서를 두고 'yy'를 누릅니다.
2. 'p'를 5번 눌러서 똑같은 줄을 5개 만듭니다.
3. 'Permission: ReadOnly' 줄을 'dd'로 지우고 'u'로 다시 살려봅니다.

---

## 📝  [번개 같은 단어 찾기 (/)]

🚩 목표: 수백 줄의 파일에서 내가 원하는 단어 찾기

💻 [실습 텍스트]
apple banana cherry apple graph apple melon orange apple strawberry

✅  미션:

1. 위 단어들을 한 줄에 쭉 적습니다.
2. 'Esc' 상태에서 '/apple'을 치고 엔터를 누릅니다.
3. 'n'을 계속 누르면서 다음 'apple'로 커서가 튄 자국을 확인합니다.
4. 'Shift + n'을 눌러 반대 방향으로도 가봅니다.

---

## 📝 [고급 이동 (gg, G, $)]

🚩 목표: 마우스 휠 대신 키보드로 순간이동

💻 [실습 텍스트] (내용을 많이 채울수록 좋습니다)

1. Start of the file
... (아무 글이나 10줄 정도 입력) ...
2. End of the file

 ✅ 미션:

1. 'G'를 눌러 10번 줄로 단번에 내려갑니다.
2. 'gg'를 눌러 1번 줄로 올라옵니다.
3. '$'를 눌러 현재 줄의 맨 끝으로 이동해 봅니다.:wq

---

<img width="1025" height="352" alt="스크린샷_2026-04-23_064317" src="https://github.com/user-attachments/assets/8b6b3093-ab8b-496b-9ff8-4ad07f93b081" />
