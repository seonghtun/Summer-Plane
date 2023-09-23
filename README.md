# 항공권 조회 서비스

<br>

<p align="center">


![KakaoTalk_20230923_172107133](https://github.com/seonghtun/Summer-Plane/assets/74886046/ba124a00-3abb-45e2-8013-bfb5ff733ff6)

<br>

<img src= "https://img.shields.io/badge/Javascript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=white" />
<img src= "https://img.shields.io/badge/nodedotjs-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
<img src= "https://img.shields.io/badge/mysql-4479A1?style=flat-square&logo=mysql&logoColor=white" />
<img src= "https://img.shields.io/badge/mongodb-47A248?style=flat-square&logo=mongodb&logoColor=white" />
<img src= "https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=CSS3&logoColor=white" />
<img src= "https://img.shields.io/badge/inux-FCC624?style=flat-square&logo=linux&logoColor=white" />

<br>
</p>

## 주제 선정 이유

코로나 유행이 끝난 이후 다시 여행객들이 늘어남에 따라 해외 여행객들에 이용수단인 항공기 항공편에 대한 정보들이 필요할것이라 생각하여 이 항공편 조회 서비스를 선택하여 만들게되었습니다.

### Installing

#### npm 모듈 설치 

```
apt install -y npm
```
```
npm install -g nodemon
```
```
npm init -y
```
```
npm install
```
#### mongodb 설치

```
wget -qO - https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -
```
```
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/4.4 multiverse" | tee /etc/apt/sources.list.d/mongodb-org-4.4.list
```
```
wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1f-1ubuntu2_amd64.deb
```
```
dpkg -i libssl1.1_1.1.1f-1ubuntu2_amd64.deb
```
```
rm -rf libssl1.1_1.1.1f-1ubuntu2_amd64.deb
```
```
apt -y update; apt -y upgrade
```
```
apt -y install mongodb-org
```
```
systemctl start mongod
```
```
systemctl status mongod
```
```
mongod --version
```
```
mongo
```
#### nodejs install

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
```
cat ~/.bashrc
```
```
source ~/.bashrc
```
```
nvm --version
```
```
nvm ls-remote
```
```
nvm install v18.15
```
```
nvm install v16.20
```
```
npm install sync-mysql dotevv async axios
```

## back-end 아키텍쳐 설계

제작중..

### 테스트는 이런 식으로 동작합니다
|                sign in              |                sign up               |
| :----------------------------------: | :----------------------------------: | 
| <img src='https://github.com/LeeMyungdeok/bike-rental-project/assets/115915362/d9b8fd6f-920d-4086-81b4-28481e60e383' width='400px' height='200px'>                                | <img src='https://github.com/LeeMyungdeok/bike-rental-project/assets/115915362/6f8f1f67-5432-4956-a45a-778daa9e633c' width='400px'  height='200px'>                                 |

|                return              |                rental               |
| :----------------------------------: | :----------------------------------: |
| <img src='https://github.com/LeeMyungdeok/bike-rental-project/assets/115915362/ffe5dd42-a87b-46f1-98b3-d673b25a15a4' width='400px' height='300px'>                                 | <img src='https://github.com/LeeMyungdeok/bike-rental-project/assets/115915362/d191e793-e651-4951-bdf1-7bbe480dac17' width='400px' height='400px'>                                 |







## 배포

예정 입니다.

## 팀명: SilverCathle

* [팀원](링크) - 윤성현, 최은재

## 담당 업무

- backend
  - mysql을 활용하여 로그인 정보를 저장하는 데이터베이스 연결 을 구현하였습니다.
  - 참조 관계를 만들어 항공권과 이용객에 정보를 연관되게끔 ERD를 구성하였습니다.
  - 유저 backend API(CRUD) 를 구현하였습니다.
- frontend
  - 로그인 페이지, 회원가입 페이지를 구현했습니다.
 
## 보완점

- 가격에대한 고려를 하지않아 일관된 가격을 가지고있어 좀더 현실적인 가격을 데이터로서 넣어주면 좋겠다.
- ERD는 항공편과 이용객에 정보가 연관되도록 구성하고 테이블 구성 실제 코드 구현이 되어있지않아 구현하면 좋겠다
- 실제 구매 버튼이 동작하는 backend API와 javscript 함수들을 구현하면 좋겠다.
