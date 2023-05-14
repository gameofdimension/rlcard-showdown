### build image
```
docker build -tag douzero .
```

### run the demo
1. download pretrained model as [here](https://github.com/gameofdimension/rlcard-showdown#run-rlcard-showdown) it says
2. update docker-compse.yaml, specify your model path
```
- /path/to/pretrained:/rlcard-showdown/pve_server/pretrained
```