---
layout: single
title: "while roop"
---


[문제상황]  
DAUM에서는 주기적으로 비밀번호를 변경하여 개인정 보를 
안전하게 보호하고 있습니다. ID는 ‘알파벳+숫자’ 의 조합으로, 
‘kyunghee8323’과 같이 만들 수 있습니다. 새로 변경하려는 
비밀번호에서 연속된 3글자가 ID에들어 있다면 그것은 사용이 
허락되지 않습니다. 위에서 설명한 것과 같이 비밀번호 변경 가능 
여부를 체크한 후에 비밀번호를 변경하는 프로그램을 작성하시오.
[문제해결]  
~~~  
ID=input('ID를 입력하세요 : ')
PW=input('PW를 입력하세요 : ')

for x in range(len(PW)-3) :
  if PW[x:x+3] in ID:
    print('사용 불가한 비밀번호입니다.')
    break
else:
  print('사용 가능한 비밀번호입니다.')
   
~~~

[결과]  
ID를 입력하세요 : gohyeonseung5916
PW를 입력하세요 : gohaaaaaaaa5555
사용 불가한 비밀번호입니다.
