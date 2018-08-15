# Win上でのgitの使い方

##コマンドの基礎と順序

```
	git --bare init --shared	=> リモートに空のリポジトリ作成
	git remote add origin [Local Path]　	=> ローカルリポジトリとリモートを紐付け
	git push origin master		=> masterへのpush

	git init				
	
	$vi .gitignore			=> 対象ファイル/ディレクトリ
	
	git add -A 				=> カレントディレクトリのignore以外をindexにあげる。
	
	git status				=> Commit対象を見る。
	
	git commit				=> ローカルリポジトリに格納される
	
	
	git clone [path]		リポジトリをコピーしてくる
	認証
	git config 				ユーザ・メールアドレス指定
	git status				リポジトリのStatus見れる
	ファイル変更
	git status    			ファイルの変更状態を見る
	git diff				差分調べる
	git add					インデックスに入れる(Commitの候補に入れる・キャッシュに入れるみたいな)
	git commit				ローカルリポジトリへのコミット
	git push				リモートリポジトリへのコミット

	git checkout [ファイル名] HEAD						ファイルのロールバック
	git checkout -b [ブランチ名] [SHA1・ハッシュ]		新しいブランチをつくる
	git checkout [ブランチ名] 							ブランチを移動する

	git branch
	git remote 
	git remote -v
	git push -u origin(初期のリモート) old(ブランチ名)
	
	git branch -d old		ブランチを削除する

	git clean -n			git対象外のファイルを削除する前に候補を表示する
	git clean				git対象外のファイルを削除する
	git clean -xf			gitで通常無視されるファイルを削除する
```
