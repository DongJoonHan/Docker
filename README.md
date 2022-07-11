# Utel

## GitLab Root Password 초기화

```
gitlab-rails console -e production
```

```
user = User.where(id: 1).first
```

```
user.password = '변경할 비밀번호'
user.password_confirmation = '변경할 비밀번호'
user.save
```
