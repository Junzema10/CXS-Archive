# CXS ARCHIVE — 데모

CXS ARCHIVE 프로젝트 아카이빙 웹앱의 정적 빌드본입니다. GitHub Pages로 바로 배포해
누구나 링크로 접속해볼 수 있는 라이브 데모용으로 준비되었습니다.

## 안내

- 이 저장소에는 **빌드된 결과물만** 들어있습니다 (React/TypeScript 원본 소스코드는
  포함되어 있지 않습니다).
- 로그인은 데모용 계정 선택 방식이며 실제 인증 서버는 없습니다. 모든 데이터는
  각 방문자의 브라우저(localStorage)에만 저장되므로, 방문자마다 별도로 보이고
  서로 영향을 주지 않습니다. 새로고침해도 그 브라우저에 저장한 내용은 유지되지만,
  다른 사람 화면에는 반영되지 않습니다.
- 프로젝트/브랜드명은 전부 가상의 데모 데이터입니다.

## GitHub Pages로 처음 배포하는 방법

1. GitHub에서 새 저장소를 만듭니다 (예: `cxs-archive-demo`). Public으로 만들어야
   무료 GitHub Pages를 사용할 수 있습니다. (README, .gitignore 등은 체크하지 않고
   빈 저장소로 만들어주세요.)
2. 이 폴더를 다운로드한 뒤, 폴더 안에서 명령 프롬프트(CMD)를 열고 아래 명령어로
   방금 만든 저장소에 올립니다 (저장소 생성 후 뜨는
   "…or push an existing repository from the command line" 안내와 동일합니다):

   ```
   git remote add origin https://github.com/<본인계정>/<저장소이름>.git
   git branch -M main
   git push -u origin main
   ```

3. GitHub 저장소 페이지에서 **Settings → Pages**로 이동합니다.
4. "Build and deployment" → Source를 **Deploy from a branch**로 두고,
   Branch를 **main** / **/(root)**로 선택한 뒤 저장(Save)합니다.
5. 1~2분 정도 기다리면 같은 화면에 `https://<본인계정>.github.io/<저장소이름>/`
   형태의 주소가 표시됩니다. 그 주소로 접속하면 데모 페이지가 공개된 것입니다.

※ 저장소 이름을 다른 걸로 바꿔도 상관없습니다 — 이 빌드는 상대 경로(`./assets/...`)
로 만들어져 있어서 어떤 저장소 이름(서브 경로)에서 열어도 정상 동작하도록
이미 확인해 두었습니다.

## 나중에 내용을 업데이트하고 싶을 때

이 폴더의 파일을 새 빌드 결과물로 교체한 뒤, 같은 폴더에서 CMD로

```
git add -A
git commit -m "update"
git push
```

를 실행하면 1~2분 후 같은 주소에 반영됩니다. 저장소를 새로 만들 필요는 없습니다.
