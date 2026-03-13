
## 2단계: 초기 애플리케이션 설정 — 디렉터리 구조, Python 요구사항, MongoDB

> [!NOTE]
> **백그라운드 설명:** 이 실습에서는 GitHub Copilot의 응답을 안내하는 **커스텀 지침 파일**을 사용합니다.  
> `.github/instructions/octofit_tracker_setup_project.instructions.md` 지침 파일에는 프로젝트 구조 가이드라인, Python 패키지 요구사항, MongoDB 설정이 포함되어 있으며, Copilot은 이 단계를 위한 코드를 생성할 때 해당 내용을 참조합니다.

이 단계에서는 다음 작업을 수행합니다.

- `octofit-tracker` 애플리케이션 디렉터리 구조 생성
- `octofit-tracker/backend` 및 `octofit-tracker/frontend` 디렉터리 생성
- `octofit-tracker/backend/requirements.txt` 파일 생성

> [!NOTE]
> 아래 프롬프트를 **GitHub Copilot Chat**에 복사하여 붙여넣고, 프롬프트 입력 드롭다운에서 **“Ask”** 또는 **“Edit”** 대신 **“Agent”**를 선택하세요.
> - Copilot agent mode는 대화형이므로 질문을 받을 수도 있고, 질문을 할 수도 있습니다.
> - Copilot의 응답을 잠시 기다린 뒤, 제시된 명령을 실행하려면 **`Continue`** 버튼을 누르세요.
> - Copilot agent mode가 생성하거나 수정한 파일은 작업이 완료될 때까지 유지하세요.
> - Agent mode는 코드베이스를 평가하고 명령을 실행하며, 코드베이스의 일부를 추가/리팩터링/삭제할 수 있고, 과정 중 실수가 발생하면 자동으로 복구(self-heal)할 수 있습니다.

**Copilot Chat 패널에서 플러스 `+` 아이콘을 눌러 새 Copilot Chat 세션을 여세요.**

### :keyboard: 활동: GitHub Copilot agent mode로 애플리케이션 생성을 시작하기 위한 프롬프트

> ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
>
> 다음 단계를 **하나씩** 따라가며 명령을 실행해 주세요.
>
> ```prompt
>
> - OctoFit Tracker 앱 구조를 따릅니다
> 
> - Python 가상 환경 생성을 따릅니다
> 
> - requirements.txt 파일을 생성합니다
> 
> - 생성된 파일에서 Python 요구사항을 설치합니다
> ```

1. 이제 애플리케이션 디렉터리 구조를 생성하고, Python 가상 환경을 설정했으며, Copilot agent mode가 모든 프로젝트 의존성을 설치하기 위한 `requirements.txt` 작성을 도와주었습니다. 이제 변경 사항을 `build-octofit-app` 브랜치에 반영해 봅시다.
1. 새 변경 사항이 완료되었으므로, **커밋(commit)** 하고 **푸시(push)** 하여 `build-octofit-app` 브랜치에 반영하세요.
1. Mona가 작업을 확인하고 피드백을 제공하며 다음 레슨을 공유할 때까지 잠시 기다렸다가 계속 진행하세요!

<details>
<summary>문제가 있나요? 🤷</summary><br/>
피드백이 오지 않는다면 다음 사항을 확인해 보세요.
- 다음 파일이 `build-octofit-app` 브랜치에 커밋되었고 GitHub로 푸시/동기화되었는지 확인하세요.
  - `octofit-tracker/backend/requirements.txt` 파일이 존재하며 `Django==4.1` 패키지를 포함하고 있는지
- Mona가 오류를 발견했다면, 수정 후 다시 푸시하세요. Mona는 필요할 때마다 여러 번 작업을 확인합니다.
</details>
