# Cloud-1
## Stack
<img src="https://img.shields.io/badge/Docker-2496ed?style=flat-square&logo=Docker&logoColor=white"/><br>
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=Amazon AWS&logoColor=white"/><br>
<img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=Terraform&logoColor=white"/><br>

## **[Inception Specification](./README/specification.md)**
![specification](./README/specification.svg)

## **Cloud-1 Mandatory Part**
어플리케이션의 배포는 완전히 자동화되어야 합니다. \
Ansible을 사용하는것 추천합니다, 하지만 원한다면 다른 도구를 사용해도 좋습니다. \
스크립트를 사용하여 Inception과 동일한 기능 사이트를 제공해야 합니다.
### 필수적인 것
* 서버가 재부팅되면, 사이트가 자동으로 다시 사작될 수 있습니다.
* 재부팅 시 사이트의 모든 데이터는 유지되어야 합니다.
* 사이트를 여러 서버에 병렬로 배포 할 수 있습니다.
* 스크립트는 SSH 데몬을 실행하고 Python이 설치된 대상 인스턴스의 OS와 같은 ubuntu 20.04 LTS를 가정할 때만 자동화된 방식으로 작동 할 수 있어야합니다.
* 어플리케이션은 서로 통신할 수 있는 별도의 컨테이너에서 실행됩니다.
* 서버에 대한 공개 접속은 제한되고 보안이 적용되어야 합니다.
* 서비스는 워트프레스에서 직접 설치할 수 있는 여러 구성 요소가 될 것입니다.
* 각 서비스에 대한 전용 도커 파일이 있어야 합니다.
* SQL 데이터베이스가 WordPress 및 PHPMyAdmin과 함께 작동하는지 확인해야 합니다.
* 가능하면 서버가 TLS를 사용할 수 있어야 합니다.
* 요청된 URL에 따라 서버가 올바른 사이트로 리다이렉션 하는지 확인해야 합니다.

## Turn-in and peer-evaluation
이 프로젝트는 사람에 의해서만 평가됩니다. \
이 프로젝트는 보너스가 없습니다. \
사이트 외관에 너무 많은 관심을 기울이지 않을 것입니다. \
기본적인 `WordPress`만으로도 충분합니다. \
도메인 이름이 없는 것은 혀용하지만, 도메인 이름이 있다면 감사하겠습니다. \
도메인이 있다면 이를 통해 `HTTPS`를 이용하여 사이트에 액세스 할 수 있습니다.
