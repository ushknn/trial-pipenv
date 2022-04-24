# trial-pipenv
pythonの開発環境をpipenvで作成

## 使ってるもの

### 1. docker
pythonをコンテナ内で動かす
### 2. python
version = 3.9
### 3. pipenv
python のライブラリ管理
### 4. pytest
テスト実行
### 5. github actions
テストの自動実行

### jupyter notebookの使い方

1. コンテナ起動してコンテナ内に入る
```
$ docker-compose up -d
$ docker-compose exec bash
```

2. コンテナ内で以下実行
```
# pipenv install
# pipenv shell
# jupyter notebook --ip=0.0.0.0 --allow-root --NotebookApp.token='' --notebook-dir 'works'
```

3. `localhost:8888`にブラウザでアクセス
