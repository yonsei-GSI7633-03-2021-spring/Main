# FAQ

1. 주피터 노트북에서 텍스트 에디터가 열리지 않습니다.
   1. 컴퓨터의 기본 브라우저를 구글 크롬으로 변경하시고 다시 진행하실게요!
   2. [https://support.google.com/chrome/answer/95417?co=GENIE.Platform%3DDesktop&hl=ko](https://support.google.com/chrome/answer/95417?co=GENIE.Platform%3DDesktop&hl=ko)
2. git bash에서 상위 폴더로 이동은 어떻게 하나요?
   - 다음과 같이 cd 띄어쓰기 그리고 .. 점을 두번 입력해주시면 됩니다.
   ```
   cd ..
   ```
3. git pull시 에러가 발생합니다
   - 다음 순서로 git pull을 다시 실행해주세요!
   ```
   git add .
   git commit -m "sync"
   git pull
   ```
4. git push시 에러가 발생합니다
   - 다음 순서로 git push를 다시 실행해주세요!
   ```
   git pull
   git add .
   git commit -m "submit"
   git push origin main
   ```
5. git commit을 했는데, git bash에서 다음과 같은 메시지가 나오면서 입력이 제대로 안되고, 키보드도 잘 안 움직입니다.
    ```
    # 변경 사항에 대한 커밋 메시지를 입력하십시오. '#' 문자로 시작하는
    # 줄은 무시되고, 메시지를 입력하지 않으면 커밋이 중지됩니다.
    #
    # 현재 브랜치 main
    # 브랜치가 'origin/main'에 맞게 업데이트된 상태입니다.
    #
    # 커밋할 변경 사항:
    #       수정함:        .DS_Store
    #       수정함:        README.md
    #       새 파일:       practice/.DS_Store
    #
    ``` 
    - 먼저 `i`를 누르시고 키보드에서 commit메시지를(submit) 입력하신 뒤에, `esc`를 누르시고, `:wq` 세 글자를 순차적으로 입력하시고 엔터를 쳐주세요!