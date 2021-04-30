# ruby - bundler설치시 문제

### ruby 설치를 할려고 하는데 설치가 안된다.

```jsx
brew ruby install
```

하지만 나오는 코드

![rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled.png](rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled.png)

이런식이였다.

혹시나 싶어 루비가 이미 설치되어 있는지 확인해봤다.

```jsx
ruby --version
```

![rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled%201.png](rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled%201.png)

MacOS에는 이미 ruby가 설치되어 있다고 해서, 그런것 같았다. 그 뒤 bundler를 다운 받기 위해

```jsx
gem install jekyll bundler
```

을 했는데

![rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled%202.png](rubu%20-%20bundler%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%E1%84%89%E1%85%B5%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%8C%E1%85%A6%207ed7b8b94df147c4ac8a5068f062e6c8/Untitled%202.png)

이런 에러가 발생했다. 대충 시스템 ruby를 이용하고 있기때문에 권한이 없다고 한다.

나는 sudo를 통해 install를 했다.

```jsx
sudo gem install jekyll bundler
```
