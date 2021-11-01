### Yarn2 설정
```cmd
yarn set version berry
```
+ .yarnrc.yml 파일 맨 위에 nodeLinker: pnp

### 프로젝트 생성
```code 
yarn init -2
```

### TypeScript(workspace) 설치
```cmd
yarn add --dev typescript
```

### TypeScript package 자동 설치
```cmd
yarn plugin import typescript
```

### TypeScript 초기화
```cmd
yarn tsc --init
```
+ tsconfig.json 수정
 ```json
 ...
"jsx": "react-jsx",
...
"rootDir": "./src",
```

### Parcel 설치
```cmd
yarn add --dev parcel
```

### React 설치
```cmd
yarn add react react-dom
```

### Eslint for React
```cmd
yarn add --dev eslint eslint-plugin-react @typescript-eslint/eslint-plugin eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y
yarn add --dev eslint-plugin-react-hooks @typescript-eslint/parser eslint-config-airbnb-typescript eslint-config-airbnb-base eslint-import-resolver-node
```

### Eslint 초기화
```cmd
yarn eslint --init
```

### Editor SDK 설치
yarn dlx @yarnpkg/sdks vscode

### gitignore: using Zero-Install
.yarn/*
!.yarn/cache
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/sdks
!.yarn/versions

### gitignore: not using Zero-Install
.pnp.*
.yarn/*
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/sdks
!.yarn/versions

# Script
"scripts": {
  "start": "parcel public/index.html",
  "build": "parcel build public/index.html --dist-dir www"
},
