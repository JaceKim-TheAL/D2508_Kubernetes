[kubernetes]: https://github.com/JaceKim-TheAL/D2508_Kubernetes
[![적용기술](https://skillicons.dev/icons?i=docker,kubernetes&theme=dark)][kubernetes]

# 도커/쿠버네티스를 활용한 컨테니어 개발

### INDEX

<table>
  <tr>
    <td><b href="sect_01.md">1.DK기초 </b></td>
    <td><a href="sect_02.md">2.DK배포 </a></td>
    <td><a href="sect_03.md">3.CT입문 </a></td>
    <td><a href="sect_04.md">4.KB입문 </a></td>
    <td><a href="sect_05.md">5.SW이용 </a></td>
    <td><a href="sect_06.md">6.KB구축 </a></td>
    <td><a href="sect_07.md">7.KB실전 </a></td>
    <td><a href="sect_08.md">8.CT운영 </a></td>
    <td><a href="sect_09.md">9.DK이미지   </a></td>
    <td><a href="sect_10.md">10.DK활용법  </a></td>
    <td><a href="sect_ABC.md">부록        </a></td>
  </tr>
</table>

---
# S01. 도커의 기초
- [01. 도커란 무엇인가](#도커란-무엇인가)
- [02. 도커를 사용하는 의의](#도커를-사용하는-의의)
- [03. 로컬 도커 환경 구축](#로컬-도커-환경-구축)

---
### 도커란 무엇인가

- 도커(Docker) : 컨테이너형 가상화 기술을 구현하기 위한 상주 애플리케이션과 이 애플리케이션을 조작하기 위한 명령행 도구로 구성되는 프로덕트
- 2013년 닷클라우드(dotCloud, 현재는 Docker) 사의 엔지니어엿던 솔로몬 하익스(Solomon Hykes)가 최초로 도커를 오픈 소스로 공개
- 도커가 인기를 얻게 되자 도커사는 오케스트레이션 도구인 Fig를 시작으로 도커의 지원도구를 하나씩 인수하면서 세력을 확대
- 현재는 컨테이너 관련 기술의 사실상 표준 지위를 차지
- 도커의 기본개념
  - 컨테이너형 가상화 기술
  - 애프리케이션이 중심이 되는 도커

<br/>

[[TOP]](#index)

---
### 도커를 사용하는 의의

- 코드로 관리하는 인프라와 불변 인프라 : Infrastruture as Code & Immutable Infrastructure
- 애플리케이션과 인프라 묶어 구축하기
- 애플리케이션 구성 관리의 용이성
  - 도커 컨테이너는 애플리케이션고 인프라를 함께 담은 상자
  - 도커 컴포저 사용 : yaml 포맷으로 작성된 실정 파일로 컨테이너를 정의하거나 컨테이너 간의 상호 의존 관계를 정의해 시작 순서를 제어
  
<br/>

[[TOP]](#index)

---
### 로컬 도커 환경 구축

<br/>

[[TOP]](#index)

---

