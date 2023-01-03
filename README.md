# [Kubernetes hands on](https://github.com/algolia/kubernetes-hands-on)

## 목차

1. [Prerequisites](#prerequisites)
1. [클러스터 생성](#클러스터-생성)
1. [Kubernetes api](#Kubernetes-api)

<hr />

## prerequisites

### [Homebrew](https://brew.sh/)
```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### kubectl (macOS)

```sh
$ brew install kubectl

# Kubectl 자동 완성 (zsh)
$ source <(kubectl completion zsh)  # 현재 셸에 zsh의 자동 완성 설정
$ echo "[[ $commands[kubectl] ]] && source <(kubectl completion zsh)" >> ~/.zshrc # 자동 완성을 zsh 셸에 영구적으로 추가한다.
```

### minikube

```sh
$ brew install minikube
$ echo 'eval $(minikube docker-env)' >> ~/.zshrc
```

### helm 설치

```sh
$ brew install helm
```

<hr />

## 클러스터 생성

```sh
$ minikube start

# 확인
$ kubectl get nodes
$ kubectl config current-context
```


## 클러스터 멈춤
```sh
minikube stop
minikube delete
```
