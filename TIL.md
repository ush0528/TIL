# 2026/11/10
- 배운 것:
  1. git commit
 
  2. git branch (브랜치이름): 브랜치 만들기
     
     2-1. git merge (브랜치이름): 다른 브랜치의 커밋을 현재 브랜치로 합치기
     
     2-2. git branch -f (브랜치이름) HEAD~(올라갈커밋수): 브랜치이름 옮기기
  3. git rebase (브랜치이름): 머지 커밋 없이 선형 히스토리 만들기
  4. git switch (브랜치이름): HEAD를 다른 브랜치로 변경(분리되어 있는 HEAD를 해당 브랜치에 붙임)
     
     4-1. git switch --detach (해시/HEAD/비워놓기): HEAD를 브랜치에서 분리
  
       4-1-1. git switch --detach (브랜치이름)^: 상위 커밋으로 HEAD 옮기기(1)
     
       4-1-2. git switch --detach (브랜치이름)~(올라갈커밋수): 상위 커밋으로 HEAD 옮기기(1이상)

  5. 작업 되돌리기
     
     5-1. git reset HEAD~(돌아갈커밋): 예전 커밋으로 브랜치를 옮김(local)
  
     5-2. git revert HEAD~(취소할커밋): 브랜치의 끝에 새로운 커밋(전 버전) 추가(pushed)
     
- 막힌 것:
  1. git switch --detach를 하고 바로 커밋하면, HEAD가 특정 커밋에 붙고 브랜치에 속하지 못한다.
  2. main VS HEAD: main은 브랜치 이름(여러 개), HEAD는 지금 내가 있는 곳(하나 뿐)
  3. 브랜치 이름 옮기기: git branch -f (브랜치이름) (위치)

     HEAD 옮기기: git switch --detach (위치)

  4. <img width="1142" height="402" alt="image" src="https://github.com/user-attachments/assets/1808853b-e7ae-4549-b161-328336539f28" />

- 내일 할 것: learn git branching 3-4 단계
