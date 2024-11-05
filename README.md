# Ansible 미니 프로젝트 
## 목표
1. 우분투 서버 머신 3대에 대한 코드 기반의 환경 설정 관리
2. 마스터 노드 1 / 워커 노드 2 로 구성된 쿠버네티스 클러스터 구축
3. 마스터 노드에 CICD를 위한 TeamCity Server 구성
4. 워커 노드에 Build를 위한 TeamCity Client 구성
---
## 시스템 정보
1. Intel(R) Core(TM) i7-9700 CPU @ 3.00GHz   3.00 GHz
2. RAM 16.0GB / 2667MHz / Single
3. Ubuntu Server 22.04 LTS
4. Network Speed
   * Inner Network - 100Mb<br>
     ![image](https://github.com/user-attachments/assets/e3e0dccd-5d24-44cf-b334-70ff5a30c84b)
   * External Network - 100Mb<br>
     ![image](https://github.com/user-attachments/assets/034db063-17bc-49d9-9c82-c0a74bc5c4a9)
## 노드 구성
1. k8s-master [192.168.20.184] username/master
2. k8s-worker1 [192.168.20.182] username/worker
3. k8s-worker2 [192.168.20.180] username/worker
## 작업 방법
1. VSCode를 이용해 마스터 노드에 SSH 접속, /home/master/ SFTP 연결
2. 쉘을 이용해 Ansible 설치 및 노드 연동
3. 플레이북을 이용한 기본 패키지 구성 및 k8s 노드 구축
