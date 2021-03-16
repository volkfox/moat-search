# moat-search

REST µservice for searching Moat.com image database using a tagline.
Requires: 
1. t2.medium AWS instance, 200GB storage (no CUDA)
2. moat.com features dataset in directory moat-dataset/ available here: https://moat-dataset.s3-us-west-2.amazonaws.com/features.npy

Usage:
```
curl -H "Content-Type: application/json" -X POST -d '{"prompt":["The quick brown fox"], "num":3}' http://127.0.0.1:8000/api
```
Returns:
JSON list object with moat.com image indices
