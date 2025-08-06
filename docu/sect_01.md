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
- 운영환경에서 빛을 발하는 도커
- 새로운 개발 스타일
  - 서버 및 인프라의 존재를 전혀 의식하지 않아도 된다
  - 애플리케이션 개발에 집중

<br/>

[[TOP]](#index)

---
### 로컬 도커 환경 구축
- 윈도우용 도커 설치
- macOS용 도커 설치
- 윈도우용/macOS용 도커 기본 설정
  - 도커 자동 실행
- 도커 툴박스(Docker Toolbox)
  - 도커 툴박스는 VirtualBox로 게스트 운영체에를 구축한 다음 그위에 도커를 실행하므로 순수하에 윈도우용/macOS용 도커를 실행하는 것보다는 리소스 효율면에서 불리
  - 그러나 호스트 운영체제의 리소스를 공유하지 않는 만큼 환경 구축에서 일어날 수 있는 말썽이 적다.
  - 도크 툴박스는 VirtualBox를 사용하므로 윈도우용 도커를 설치할 때와 마찬가지로 물리 머신의 BIOS 설정에서 가상화 기능을 활성화해야 한다.
  - 또한 VirtualBox와 Hyper-V 기능을 동시에 사용할 수 없으므로 Hyper-V 기능이 활성 상태라면 `제어판` - `프로그램` - `Window 기능 켜기/끄기`에서 다음과 같이 **Hyper-V를 비활성화** 한다. 설정이 반영되려면 윈도우 재시작해야 한다. 
  - 설치에서 `Select Additional Tasks`에서 `Install VirtualBox with NDIS5 driver[default NDIS6]` 항목에 체크해야 한다. NDIS6은 Host Only Network와 관련된 버그가 있으므로 이전 버전인 NDIS5를 선택할 수 있다.
  - 설치가 끝나면 Docker Quickstart Termianl 아이콘을 클릭해 도커 환경을 실행한다.
  - 곧 터미널이 실행되는데, 도크 툴박스를 처음 실행했다면 먼저 VirtualBox에서 도커를 실행할 가상환경을 만들어야 하므로 조금(몇분 정도) 시간이 걸린다.
  - 터미널은 호스트 운영체계에서 동작하지만, docker 명령은 VirtualBox에서 동작하는 게스트 운영체제에 구축된 도커환경과 연결해 있다. 
  - 그러므로 Docker Quickstart Terminal에서 마치 도커가 로컬에 설치된 것처럼 사용할 수 있다. 
  - 그리고 윈도우용 Docker Quickstart Terminal을 사용되기 때문에 도커 툴박스를 사용하면 macOS와 거의 동일한 명령을 사용할 수 있다. 
   

[[TOP]](#index)

---
