# VITE로 REACT 프로젝트 구축하기

</br>

### vite란?

빠르고 간결한 모던 웹 프로젝트 개발 경험에 초점을 맞춰 만들어진 빌드 도구이다. </br>
시작은 vue를 위한 빌드도구였지만, 현재는 vanilla, vue, react,svelte 등 에서 사용이 가능하며, javascript, typescript도 모두 사용 가능하다.

</br>

### vite를 사용하는 이유

1. 빌드속도가 빠르다. </br>
기존에 사용하던 webpack의 빌드 도구는 자바크립트 언어로 만들어졌지만, 
vite가 내부적으로 사용하는 ESBulid는 Go라는 네이티브 언어로 만들어진 도구를 이용해 빌드하기 때문에 
빌드 속도가 아주 빠르다.

2. 개발 서버가 빠르게 구동된다.</br>
기존 webpack과 같은 모듈 번들러를 이용할 때는 모듈 번들링을 끝낸 후 개발 서버를 구동하므로 시간이 오래걸렸지만,  </br>
vite는 native ESM이라는 브라우저의 자체적인 모듈 기능을 사용하여 vite가 실행하는 개발 서버는 브라우저가 요청하는 모듈을 전송해주고, 모듈 번들링 기능을 브라우저가 수행하기 때문에 (번들링하지 않고 바로 로컬개발서버의 ESM 방식을 사용) </br>
명령어를 실행함과 동시에 개발 서버가 구동된다.

3. HMR(Hot Module Replacement) </br>
   vite도 HMR 기능을 지원한다. </br>
   어떤 모듈이 수정되면 전체가 아닌 수정된 모듈과 관련된 부분만 교체하고, 브라우저에 교체된 모듈을 전달한다.
  
</br>

### 설치 방법

</br>

```

npm init vite
Project name : 프로젝트 이름 설정
Select a framework : 프레임워크 설정(vanilla, vue, react, preact, lit svelte)
Select a varant : javaScript or typeScript 선택
cd 프로젝트 명
npm install
npm run dev

```

### 화면
</br>
<img width="523" alt="image" src="https://github.com/yejz0715/vite-project/assets/86754632/8ebf1d07-cdcf-4099-9ab9-9fe606bb9b42">
