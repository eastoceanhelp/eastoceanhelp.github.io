# eastoceanhelp.github.io

GitHub Pages のルート（ユーザーサイト）。主目的は **TWA（Android アプリ）の Digital Asset Links 検証**。

- `/.well-known/assetlinks.json` … TWA `io.github.eastoceanhelp.studyalmanac` の署名鍵を検証させるための必須ファイル。Android はアプリのパスに関係なく**ドメインのルート**を見るため、ここに置く必要がある（アプリ本体は別repo `studyplan-app` の `/studyplan-app/` 配信）。
- `index.html` … 素のドメインに来た人をアプリ `./studyplan-app/` へリダイレクト。
- `.nojekyll` … `.well-known` などドット始まりを GitHub Pages が配信するために必要。

assetlinks.json の指紋を更新する手順は本体repo `studyplan` の `引継ぎ.md`「Androidストア公開」節を参照。
