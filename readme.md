# KAIST-AI Server 설정

## SSH 설정 (비밀번호 없이 SSH 접속하기)

```bash
# 사용자의 컴퓨터에서 실행
ssh-keygen
# 이후 프로그램이 종료될 때까지 계속 enter 키 입력
```

![](images/ssh-keygen.png)

```bash
# 사용자의 컴퓨터에서 실행
cat ~/.ssh/id_rsa.pub
# 이후 출력된 키 복사 (Ctrl+C)
```

![](images/id_rsa.png)

```bash
# 서버에서 실행
mkdir -p ~/.ssh
echo "복사한 id_rsa.pub 키" >> ~/.ssh/authorized_keys
```

![](images/authorized_keys.png)

## ZSH 설치

