# s3_ele
wrapper for elephant


Install
=======

1. Elasticsearch v2.4.1
2. pip install -r requirements.txt

Run
===

```
honcho start web
```

Usage
=====

using httpie client

```
http -j POST http://127.0.0.1:5000/ X-Key:xxxxxx first_name=Bob last_name="Monkey-Lucky"
http -j POST http://127.0.0.1:5000/ X-Key:xxxxxx first_name=Isabelle last_name="Lucky"
http -j GET http://127.0.0.1:5000/?q='first_name:Bob' X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/?q='first_name:Bob OR first_name:Isabelle' X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/\?q\="last_name:Monkey" X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/\?q\="last_name:Lucky" X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/67c7b7bd-6b6e-4997-a673-76a65c662278 X-Key:xxxxxx
```