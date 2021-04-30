# npx create-react-app 이 안되는 경우 (M1)

어느날 새롭게 react 파일을 만들려고 했는데, creat-react-app이 안되는 경우가 있다.

```jsx
npx creat-react-app begin-react
```

= begin이라는 폴더에 react를 폴더들을 만든다는뜻.

경우는 찾아보니 

### 인터넷 연결이 글로벌이 아니여서

이와 같은 경우는 요즘 react가 글로벌 cil툴이 deprecated화 되고 있기 때문이다.

해결 방안

- 인터넷 연결을 바꾸고 재입력한다
- 제거하고 다시 만든다.

```jsx
sudo npm uninstall -g create-react-app //제거하고

$ npx create-react-app my-app //다시 설치
```

그리고 해당 폴더에 들어가서 npm start 를 하면 된다.
