# complete:13: command not found: compdef

정확한 이유는 모르겠으나, homebrew를 설치하고 난뒤에 생긴것 같다.

일단 대충 이유는 compdef는 zsh에서 자동완성을 위해 사용되는 기능인데. 자동완성이 활성화가 되어있어야한다는것이다.

근데 내가 homebrew를 다운 받으면서. M1용이 아닌, 이전 Mac 버전으로 설치하다 보니, zsh랑 기존 Mac 쉘인 bash가 설치 돼서 서로 에러가 났는지? 저런 에러가 나왔다.

해결방법은

1. zsh를 재설치 한다.
2. oh-my-zsh를 설치한다.

oh-my-zsh는 zsh테마만 바꿔준건데, 저렇게 바꿔주니깐 에러가 해결됐다. 뭔가 찜찜하다.

하지만 덕분에 brew, ruby, rbenv 등등 설치할떄 로제타 2 에러가 생기지 않는다. version 확인도 확실하다.
