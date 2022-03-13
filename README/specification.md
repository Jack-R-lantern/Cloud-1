# Specification
## Diagram
![Diagram](specification.svg)
## Container
>### Nginx
> port: 443, 9000
> TLSv1.2 or TLSv1.3
>### WordPress+PHP
> port: 3306, 9000
>### DB
> port: 3306
> MariaDB
## Network
> 위에 언급된 3 컨테이너는 하나의 Docker Network에 속해야함.
## volume
>### WordPress
> WordPress Websitefiles \
> WordPress Container와 마운트
>### DB
> WordPress Database \
> DB Container와 마운트
## 가상화 기술 사용 유무
- [x] Container

## Cloud Service
### ECS
### EKS
### Docker