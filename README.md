# Skills

큰 변경도 한 단계씩 이해할 수 있도록 돕는 AI 에이전트 스킬 모음입니다.

## 스킬

| 스킬 | 설명 |
| --- | --- |
| [walkthrough](skills/walkthrough/SKILL.md) | 코드 변경이나 긴 설명을 작은 단계로 나누고, 사용자의 확인을 받으며 진행합니다. |

## 설치

Node.js 22.20 이상 환경에서 프로젝트 폴더에서 실행합니다.

```bash
npx skills@latest add harrdas/skills --skill walkthrough
```

설치할 에이전트는 실행 중 선택할 수 있습니다. 모든 프로젝트에서 사용하려면 `-g`를 추가하세요. 설치 방법과 지원 에이전트는 [Skills CLI 문서](https://github.com/vercel-labs/skills)를 참고하세요.

수동으로 설치하려면 `skills/walkthrough` 폴더를 사용하는 에이전트의 스킬 디렉터리에 복사하세요. 에이전트별 설치 경로와 호출 방식은 해당 도구의 문서를 따릅니다.

## 사용 예시

설치한 에이전트에 다음과 같이 요청하세요.

```text
walkthrough 스킬로 이번 변경을 한 단계씩 설명해줘.
```

```text
walkthrough 스킬로 방금 제안한 설계를 설명해줘.
내가 이해했다고 하면 다음 단계로 넘어가줘.
```

한 번에 한 단계만 설명하며, `다음으로`, `더 설명해줘` 또는 자유로운 질문으로 진행합니다.

## 호환성

[Agent Skills 형식](https://agentskills.io/specification)의 `SKILL.md`를 사용합니다. 특정 제품의 질문 도구에 의존하지 않으며, 질문 UI를 사용할 수 없는 환경에서는 일반 채팅으로 답을 기다립니다.

사용자의 요청으로 시작하도록 지시합니다. 자동 호출을 차단하는 제품별 설정은 포함하지 않으므로, 앱 수준에서 수동 호출만 허용하려면 사용하는 도구에서 별도로 설정하세요.

## 새 스킬 추가

`skills/<skill-name>/SKILL.md`에 스킬을 추가하고 위 목록에 등록하세요.

## 라이선스

[MIT](LICENSE)
