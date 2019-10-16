# Upstream - Server 설정중입니다

- 기본적으로 사용 할 eslint 및 prettier 설정 예정입니다
- git flow에 대한 이해는 승재님의 영상 참고하면 될 것 같습니다
- 문제 있는 부분은 바로 논의 진행 예정입니다

- 코드 규칙 통일을 위해 VS Code Extension 내 ESLint 및 Prettier 설치가 필요합니다
- 이후 settings(Cmd+) 진입, 우측 상단의 '{}' 버튼을 눌러 json 파일을 오픈합니다
- 아래 설정 내용을 추가합니다

  {
  ...,
  "editor.formatOnSave": true,
  "javascript.format.enable": false,
  "prettier.eslintIntegration": true
  }
  
#### 서버 프로세스 동작처리 (현재 EC2-MONGO에서 서비스중)
: pm2 list
: pm2 start app.py
: pm2 stop [id]

#### 09/01 
: RDS 접속 정보를 비밀로 관리할 예정입니다. 때문에 서버 구동을 위해서 슬랙으로 공유할 파일을 config에 올려주시고 .gitignore에 해당 파일이 있는지 git status에 해당 파일이 있는지 확인해주세요.
#### 10/15
: 다시 배포해놓았습니다. 프로덕트 모드로 서버가 돌아가고 있고 호스팅된 버킷으로 들어가면 사용가능합니다.

