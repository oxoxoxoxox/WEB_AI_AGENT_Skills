# 코드 리뷰와 완료 확인

## 리뷰할 것

- 요구한 사용자 동작과 실제 변경이 일치하는가?
- 오류·빈 데이터·권한·동시 요청 등 관련 경계 상황을 다루는가?
- 기존 구조, 디자인 토큰, 공통 컴포넌트와 일관적인가?
- 입력 처리와 데이터 접근에 문제가 없는가?
- 테스트가 중요한 동작을 검증하고 실제로 실행되었는가?
- 불필요한 파일과 무관한 변경이 포함되지 않았는가?

지적에는 파일 위치, 재현 조건, 영향, 수정 방향을 적습니다. 다른 에이전트의 리뷰도 실제 코드와 근거로 확인합니다. 피드백이 틀리면 이유를 설명하고, 맞으면 수정 후 다시 검증합니다.

## 완료 보고에 남길 것

- 무엇을 왜 바꿨는지.
- 실행한 검사와 실제 결과.
- 실제로 확인한 화면과 사용자 흐름.
- 검증하지 못한 부분과 남은 일.
- 커밋·원격 반영·배포가 각각 어디까지 진행됐는지.

빌드 성공이 화면 정상 동작을 보장하거나, 스크린샷이 API 동작을 보장하지는 않습니다. 주장마다 그에 맞는 확인 결과를 사용합니다.

## Superpowers 관련 원문

- [requesting-code-review](../references/superpowers/skills/requesting-code-review/SKILL.md)
- [receiving-code-review](../references/superpowers/skills/receiving-code-review/SKILL.md)
- [verification-before-completion](../references/superpowers/skills/verification-before-completion/SKILL.md)
