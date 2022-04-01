로컬개발시 라이브러리 프로젝트를 로컬로 연결하기

yarn link 활용

1. local package
2. global node_modules 링크생성
3. 로컬 node_modules 링크생성

yarn link 디텍토리에 링크가 생성되어 관리됨

## 라이브러리 프로젝트

```json
{
  "name": "custom_module"
}
```

링크생성

```sh
yarn link
```

## 프로덕트 프로젝트

```sh
yarn link custom_module
```

라이브러리 사용

```js
import customModule from 'custom-module';
```
