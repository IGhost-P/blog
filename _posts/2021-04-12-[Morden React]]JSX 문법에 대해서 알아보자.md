# JSX 문법에 대해서 알아보자

### JSX란?

리엑트에서 컴포넌트의 생김새를 정의할때 사용한다 (Html처럼 생겼지만 Js이다)

babel이라는 도구를 이용해서 JSX ⇒ JS가 된다.

---

### JS문법의 규칙

1. 태그를 열면 무조건 닫아줘야한다.

```jsx
<div> </div>  하지만 <div> 만 하면 에러
```

+만약 그냥 아무것도 안넣고 싶다면?

selfcloseing을 이용

```jsx
<div />
```

2. 2개 이상의 태그는 꼭 하나의 태그로 감싸져야 한다

```jsx
<Hello />
<div> 안녕 </div>

// 이건 에러, 두개 이상 태그를 사용했는데 두개를 묶어 줄 게없음
// 해결 방안 1

<div>
<Hello />
<div> 안녕 </div>
</div>

// Fragment (비어있는태그, Html로 봐도 없다.)
return(
<>
<Hello />
<div> 안녕 </div>
</>
)

//추가적으로 태그를 감싸고 있는 ()는 가독성을 위해 있을뿐 없어도 에러가 x
```

3. JSX내부에서 JS값을 사용하기.

```jsx
안녕 = 'HI'
<>
<Hello />
<div> {안녕} </div>
</>
)
// {}를 하면 값이 나온다
```

4. style

우선 인라인 스타일은 객체 형태, -로 이어져 있는 이름은 대문자로 형태로 네이밍 한다.

```jsx
background-color => backgroundColor
```

```jsx
function App() {
  const name = 'react';
  const style = {
    backgroundColor: 'black',
    color: 'aqua',
    fontSize: 24, // 기본 단위 px
    padding: '1rem' // 다른 단위 사용 시 문자열로 설정
  }

  return (
    <>
      <Hello />
      <div style={style}>{name}</div> // 스타일안에 style란 객체의
값을 가지고 온것을 확인할 수 있다.
    </>
  );
}
```

+ 추가적으로 css calss를 사용할때는 calss→className으로 설정해줘여한다.

5.주석

JSX내부 주석은 {/* 이런 형태로 */} 작성된다.

```jsx
<>
      {/* 주석은 화면에 보이지 않습니다 */}
      /* 중괄호로 감싸지 않으면 화면에 보입니다 */
```
