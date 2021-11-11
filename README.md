# Movie App 2021

React JS Fundamentals Course 2021

<h3>컴포넌트</h3>
<p>리액트 앱을 구성하는 요소로 ReactDom.render() 함수의 첫번째 인자로 <Component /> 전달 시 해당 컴포넌트가 반환하는 것들을 화면에 그리고, 두번째 인자로 해당 컴포넌트가 그려질 위치를 전달한다.</p>
<pre><code>ReactDom.render(<App />, document.getElementById('root'));</code></pre>
 -> App 컴포넌트가 id가 root인 element 사이에 그려진다.(render)<br>
 -> 리액트는 최종적으로 단 한 개의 컴포넌트를 그릴 수 있다.</p>

<h3>JSX</h3>
<p>자바스크립트+HTML -> js 파일에 import React from 'react'; 문을 통해 JSX를 이해</p>

<h3>props</h3>
<p>컴포넌트에서 컴포넌트를 전달하는 데이터<br>
컴포넌트에 데이터 보내기 : <Component props이름={저장 데이터} /><br> 
  -> 저장 데이터는 boolean, 숫자, 배열, 문자열 가능(문자열은 큰따옴표)<br>
  -> props에 있는 데이터가 하나의 객체로 변환되어 컴포넌트의 인자로 전달<br>
컴포넌트에서 정의 : <br>
<pre><code>function Food(props) {
    return { props.props이름 };
  }
</code></pre>

<h3>map() 함수</h3>
<p>배열의 모든 원소마다 특정 작업을 하는 함수를 적용하고, 그 함수가 반환한 결과를 모아서 배열로 반환<br>
<pre><code>배열.map(current => {
    cosole.log(current);
    return 0;
  })
</code></pre>
<ul>
 <li>map() 함수의 인자로 전달한 함수는 배열의 원소를 대상으로 실행한다. -> 배열의 원소 개수만큼 함수 실행, 해당 인자에 배열의 원소가 1개씩 넘어옴</li>
 <li>그 함수가 반환하는 값이 모여 배열이 되고 해당 배열이 map() 함수의 반환값이 된다.</li>
</ul>
</p>

<h3>실행</h3>
<a href="https://winkite1226.github.io/movie_app_2021/#/">play</a>

<h3>출처</h3>
Do it! 클론 코딩 영화 평점 웹서비스-노마드 코더 니꼴라스, 김형태 저
