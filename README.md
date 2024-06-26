# 프로젝트 | 템플릿 - 보일러플레이트

> 프로젝트 제목 작성 후 프로젝트에 대한 개괄적인 설명을 작성합니다.

프로젝트를 시작하면 프로젝트 저장소에 프로젝트를 설명하는 `README.md` 파일을 반드시 작성하세요.
README 파일의 형식에 대한 제한은 없으나 프로젝트에 대한 이해를 쉽게 할 수 있도록 중요한 정보를 포함하는 것이 좋습니다.
이 템플릿 프로젝트는 프로젝트 저장소에 대한 기본 가이드라인을 제공하기 위해 만들어졌습니다.
프로젝트 루트 디렉토리레 위치하는 README 파일의 내용에 반드시 포함되어야하는 항목들이 무엇인지 참고하세요.

README 파일 및 설명을 위한 파일은 가급적 마크다운 형식으로 작성하길 권장합니다.
마크다운 형식은 소스코드와 함께 관리되기 용이하며 변경 이력을 관리하기 좋은 포멧입니다.
소스코드와 마찮가지로 코드에디터로 손쉽게 편집할 수 있습니다.
마크다운 문법은 다음의 링크 문서를 참고하세요.

[마크다운 기본 문법 설명 | Markdown Guide](https://www.markdownguide.org/basic-syntax/)

프로젝트 README 파일에는 다음의 내용을 설명해야합니다.

* 프로젝트 정의
  * 프로젝트의 유형, 목표, 상태와 같은 정보를 설명해주세요.
* 설치
  * 프로젝트를 설치하는 방법과 절차 등 필요한 정보를 설명해주세요.
  * 사용자의 환경에(Windows, OSX 또는 Linux) 따른 주의사항이 있다면 최대한 자세한 정보를 알려주세요.
* 실행
  * 프로젝트를 실행하는 방법을 설명해주세요.
  * 개발을 위해 로컬에서 실행하는 방법을 설명해 주세요.
* 배포
  * 프로젝트를 배포하는 방법에 대해 설명해주세요.
  * 개발환경과 운영환경 등 배포환경에 따라 달라지는 배포 방법을 설명해주세요.

그 외에 프로젝트 특성에 맞게 추가되어야하는 정보가 있다고 판단되면 자유롭게 추가해주세요.

## 프로젝트 정의

급여 및 업무 관리 플랫폼은 직원의 급여와 업무를 수행하는데 필요한 도구를 제공합니다.<br>
**급여 시스템**은 고용 계약, 급여 지급, 급여 이력 관리, 퇴직금 관리, 회계 시스템 연동 기능 일체를 제공합니다.<br>
**업무 관리 시스템**은 업무 프로세스 정의, 업무 등록 수정 검색 및 평가와 관련한 유연하고 확장 가능한 시스템을 제공합니다.

## 설치

급여 및 업무 관리 플랫폼은 서버와 클라이언트 시스템으로 구성되며 Javascript 와 Nodejs 기반으로 구성되어있습니다.<br>
프로젝트 저장소를 다음 설명에 따라 개발자 컴퓨터에 복사하고 설치 명령을 입력하여 설치를 할 수 있습니다.

```bash
git clone https://github.com/ibare/devcamp-onboarding-template.git my-project

cd my-project

npm install
```

프로젝트를 다운로드하고 설치하기 위해선 사용자의 컴퓨터에 Git 과 Nodejs가 설치되어있어야합니다.
만약 설치되어있지 않은 도구가 있다면 다음 링크를 통해 사용자 환경에 맞는 버전을 설치해주세요.

* [Git - Downloads](https://git-scm.com/downloads)
* [Node.js — Download Node.js®](https://nodejs.org/en/download/current)

## 실행

개발자 로컬 환경에서 개발 모드로 실행하기 위해선 프로젝트 루트 디렉토리에서 다음의 명령을 실행하세요.

```bash
npm run dev 
```

## 배포

프로젝트의 배포 버전을 생성하기 위해 빌드 스크립트를 실행합니다.

```bash
npm run build:production
```

개발 환경 배포 빌드는 build:develop 스크립트를 사용해주세요. 
운영 환경 빌드는 build:production 스크립트를 사용해주세요.


## 문서

프로젝트 설계 문서는 design 디렉토리에 마크다운 파일로 기록되어있습니다.
각각의 설계 문서는 다음과 같습니다.

* 요구사항 정의서 
  * 제품이 제공해야되는 기능 요구 정의서입니다.
  * 요구사항 정의서에 기술된 기능은 최소 기능 요구사항이며 추상적일 수 있으며 기능의 구체화는 제품 구현 단계에서 이루어집니다.
* 프로젝트 설계서
  * 요구사항 정의서를 기반으로 프로젝트를 설계합니다.
* 기능 정의서
  * 사용자 스토리 기반으로 세부 기능을 정의합니다.
