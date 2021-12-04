
## 오픈소스 2번째 과제 vimgolf 

### 1번


* $ vimgolf put 5f0f5fbe280fbf000c233304

![1번](https://user-images.githubusercontent.com/76933278/144704455-c0c4a36c-a73b-4f33-9d77-2d15db49c3f1.gif)

##### 실행한 명령어 :G W i (end) (esc) ZZ
  
 * G:파일 끝으로 이동
 * W: 다음 단어
 * i: 입력모드 (커서 앞에 삽입)
 * (end): 끝으로 이동
 * (esc): 입력모드 해제 
 * ZZ: 저장하고 종료
  
--------------------------------------------
### 2번

* $ vimgolf put 603ba26a01b4d00009c10a49

![2번](https://user-images.githubusercontent.com/76933278/144704457-0699991b-85cc-4050-aed5-844557a63137.gif)

##### 실행한 명령어 :%s/sublime\|emacs/vim/g   ZZ
  
* %s/sublime\|emacs/vim/g : 전체 범위에서 sublime 과 emacs를 vim 으로 치환 
* ZZ:저장하고 종료  
  
----------------------------------------------
### 3번

* $ vimgolf put 5f1063aa8361810006e73210

![3qjs](https://user-images.githubusercontent.com/76933278/144704452-11dfe427-09fb-4e0f-b93c-9404b7039eaf.gif)
  
##### 실행한 명령어 : 5G qq Y P i // (esc) 2W C TODO (esc) q k @q ZZ

* 5G: 5번째 줄 이동
* qq: 매크로 'q'로 저장하기
* Y: 복사
* P: 붙이기
* i: 입력모드 (커서 앞에 삽입) 
* //: // 입력
* (esc): 입력모드 해제
* 2W: 2번째 단어로 이동 
* C: 단어 삭제
* TODO: TODO 입력 
* (esc): 입력모드 해제 
* q: 매크로 종료 
* k: 위로 올라가기 
* @q: ("Version string")에 매크로 출력하기
* ZZ:저장하고 종료
--------------------------------------------
### 4번

* $ vimgolf put 9v0060da5177000000000209

![4번](https://user-images.githubusercontent.com/76933278/144705103-9b37895a-d869-4315-973f-a7541dd85ac9.gif)
##### 실행한 명령어 : 3G 11e i (del) b (down) (BS) r (down) (BS) g (esc) :%s/y1/abs(y1)/g  :3s/1/2/g  :4s/1/3/g  :5s/1/4/g/ ZZ

* 3G :3번째 줄로 이동
* 11e :11번째 단어
* i : 입력 모드
* (del) : 지우기
* b: b입력
* (down) : 내려가기
* (BS) :'k'지우기
* r :r 입력
* (down) :내려가기
* (BS) :'k'지우기
* g : g 입력
* (esc) :입력모드 해제
* :%s/y1/abs(y1)/g  : 전체 범위에서 "y1"을 "abs(y1)"로 바꾸기
* :3s/1/2/g : 3번째 줄에서 1을 2로 바꾸기
* :4s/1/3/g : 4번째 줄에서 1을 3로 바꾸기
* :5s/1/4/g/: 5번째 줄에서 1을 5로 바꾸기
* ZZ : 저장하고 종료


----------------------------------------------
### 5번

* $ vimgolf put 6013804df3308e0009368f1c

![5번](https://user-images.githubusercontent.com/76933278/144705099-51b9edcb-074d-4211-91c3-82722c743356.gif)
##### 실행한 명령어 : 5G q f v w y 10G (end) P q 6G @F7G @F8G @F  :10s/:/,/g (end) i (BS) (esc) ZZ


* 5G: 5번째 줄로 이동 
* qf: 매크로 'f'로 지정하고 시작 
* v: 비주얼 모드
* w: 단어 선택
* y: 복사
* 10G: 10번째 줄로 이동
* (end): 문장 끝으로 이동
* P :복사
* q :매크로 저장
* 6G :6번째 줄로 이동
* @F: 매크로 실행 (10번째 줄 " " 따옴표 안에 name 이 추가됨)
* 7G :7번째 줄로 이동
* @F :매크로 실행 (10번째 줄 " " 따옴표 안에 age 가 추가됨)
* 8G :8번째 줄로 이동
* @F :매크로 실행 (10번째 줄 " " 따옴표 안에 score 이 추가됨)
* :10s/:/,/g :10번째 줄에서 ":" 를 ","로 변경
* (end) : 10번째 줄 뒤로 이동
* i : 입력모드 실행
* (BS): "," 삭제
* (esc): 입력모드 종료
* ZZ : 저장하고 종료
