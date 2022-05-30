# study-Vuejs
## 5/31
- CDN을 통하여 Vue.js 사용해보기
    - Vue객체를 사용할 수 있음.
    - Vue.createApp(객체).mount(선택자) 형식으로 해당 선택자를 가진 html태그에 객체에 해당하는 내용을 적용
- 반응성(Reactivity)를 갖는다. 
- CLI를 이용하여 Vue.js 환경 구축해보기 
    - 내부적으로 webpack을 이용한다.
    - vue-cli-service를 통해 숨겨져 있는 부분 제공 
    - 구성 옵션들을 감추어두어 입문하기 쉽다. 
- .vue 파일은 template, script, css부분으로 나누어져있다. 
# Error Log
- Vue Cli설정을 한 이후에 No Babel config file detected for ~ 에러가 발생하는 경우 vscode설정(Preference: Open Setting(JSON))을 다음과 같이 변경해준다. 
```json
"eslint.workingDirectories": [
{"mode": "auto"}
],
```
- Eslint에러로 The template root requires exactly one element가 발생하는 경우 vscode설정(Preference: Open Setting(JSON))을 다음과 같이 변경해준다. 
```json
"vetur.validation.template": false,
"vetur.validation.script": false,
"vetur.validation.style": false,
```
- 프로젝트 루트를 vue-cli로 생성한 폴더로 두지 않으면 vetur warning이 뜨는데, `cmd` + `,` 를 통해 설정창을 열고 `vetur.ignoreProjectWarning: true`로 변경해준다. 