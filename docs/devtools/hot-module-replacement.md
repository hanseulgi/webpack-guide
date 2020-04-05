---
title: Hot Module Replacement
---

## HMR(Hot Module Replacement)

HMR은 브라우저를 새로 고치지 않아도 웹팩으로 빌드한 결과물이 웹 애플리케이션에 실시간으로 반영될 수 있게 도와주는 설정입니다. 브라우저 새로 고침을 위한 LiveReload 대신에 사용할 수 있으며 웹팩 데브 서버와 함께 사용할 수도 있습니다.

## HMR 설정하기

리액트, 앵귤러, 뷰와 같이 대부분의 프레임워크에서 이미 HMR을 사용할 수 있는 로더들을 지원하고 있지만 만약 개별적으로 설정하고 싶다면 아래와 같은 방식으로 설정할 수 있습니다.

```js {3}
module.exports = {
  devServer: {
    hot: true
  }
}
```

데브 서버에 옵션으로 `hot:true`를 추가하고 자바스크립트나 CSS 스타일시트를 변경하면 해당 모듈이 바로 업데이트가 됩니다. 그리고 화면에서는 브라우저가 다시 로딩되지 않고도 변경된 내용을 확인할 수 있습니다.