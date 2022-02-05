# Github 대용량 파일 push 실패 해결 방법



```
(error message : "RPC failed" & "fatal: The remote end hung up unexpectedly")
```



##### 1. POST 요청의 max buffer-size를 늘려준다.

* 참고링크

​      : https://j.mp/2PcS7uu

​      : https://j.mp/3bEzZkP

* git config --global http.postBuffer 157286400  (숫자는 직접 지정)

* 하나의 파일 용량이 지나치게 클 경우 1번을 적용해도 에러날 수도 있음



##### 2. Git LFS (Git Large File Storage)를 활용

* 참고링크

  : https://j.mp/37QJWdP (간단)

  : https://j.mp/3uw7PAV (상세)