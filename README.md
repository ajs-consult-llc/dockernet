# dockernet
A demo that prototypes a pattern for communicating between dockers using grpc with python.  
https://lmjw.github.io/blog/2017/12/26/docker-grpc-network.html

## get the repo
```
git clone https://github.com/free-soellingeraj/dockernet.git

```

## compile the proto buffer
Creates `test_pb2.py` and `test_pb2_grpc.py`
```
# alter import in test_pb2_grpc.py
sed -i 's~from app import test_pb2 as app_dot_test__pb2~import test_pb2 as app_dot_test__pb2~g' app/test_pb2_grpc.py
```

## TODO
  - Figure out how to encapslate this capability into other modules
