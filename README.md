# moat-search

REST µservice for searching Moat.com image database using a tagline.
Usage:
```
curl -H "Content-Type: application/json" -X POST -d '{"prompt":["The quick brown fox"], "num":3}' http://127.0.0.1:8000/api
```
Returns:
JSON list object with moat.com image indices
