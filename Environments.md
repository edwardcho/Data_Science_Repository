
#### CUDA version vs NVIDIA DRIVER

1. ubuntu 에서 다음과 같이 설치한다.

    - ubuntu 16.04 : Host
        - NVIDIA DRIVER : Host
            - CUDA VERSION (docker)     vs  NVIDIA DRIVER VERSION (host)
            - CUDA 11.0 (11.0.171)      >= 450.36.06
            - CUDA 10.2 (10.0.89)       >= 440.33
            - CUDA 10.1 (10.1.105)      >= 418.39
            - CUDA 10.1 (10.0.130)      >= 410.48
            - CUDA 9.2 (9.2.88)         >= 396.26
            - CUDA 9.1 (9.1.85)         >= 390.46
            - CUDA 9.0 (9.0.76)         >= 384.81
            - CUDA 8.0 (8.0.61)         >= 375.26
            - CUDA 7.5 (7.5.16)         >= 352.31
            - CUDA 7.0 (7.0.28)         >= 346.46
        - docker
            - client
            - server
        - nvidia-docker
            - version 2.0.3 이상
          
