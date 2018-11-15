## Quickly used

This dockerfile default install python 3.6.0 , you can change any python version for you need 

```
#you have to ssh on container
$pyenv install 2.7.13
$pyenv global 2.7.13
$python -V
Python 2.7.13
```



1.Download Dockerfile
```
$git clone https://github.com/xxxxsars/docker-pyenv.git
```

2.Create Docker images
```
$cd docker-pyenv
$docker build -t pyenv_ssh
```

3.Run Docker container
```
$docker run -d -p <localh port>:<container port> pyenv_ssh
#example
$docker run -d -p 32782:22 pyenv_ssh
```

4.Connect your container with ssh  default password is "root"
```
$ssh root@localhost -p 32782
```


