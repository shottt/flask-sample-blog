### ライブラリインストール
```
pip3 install flask
```

```
pip3 install jinja2
```

```
pip3 install -U Flask-SQLAlchemy
```

```
pip3 install pytz
```

```
pip3 install flask-login
```

```
pip3 install flask-bootstrap
```

### db作成
sqliteをインストールしておく
対話モードに入る
```
python3
```
DB作成（以下コマンドでinstance/blog.dbが出来上がる）
```
from app import app, db
app.app_context().push()
db.create_all()
```

### サーバー起動
```
export FLASK_APP=app
```
```
export FLASK_ENV=development
```
```
flask run
```

### FLASKドキュメント
https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/quickstart/