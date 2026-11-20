# 디버깅 가이드

## 원인을 확인한 뒤 수정하기

1. 오류 메시지와 재현 절차를 기록합니다. 기대 동작과 실제 동작을 구분합니다.
2. 로그, 최근 변경, 입력 데이터, 환경 차이를 확인합니다.
3. 정상 동작하는 코드와 비교해 어디에서 문제가 시작되는지 좁힙니다.
4. 근거를 붙여 한 가지 가설을 세우고 최소한의 변경으로 확인합니다.
5. 원인을 확인하면 회귀를 잡을 재현 방법 또는 테스트를 준비하고 수정합니다.
6. 원래 재현 절차를 다시 실행하고 관련 기능에 영향이 없는지 확인합니다.

같은 방향의 수정이 반복 실패하면 변경을 계속 쌓지 말고 가설과 구조를 다시 확인합니다. 재현이나 검증이 불가능하면 그 사실과 수집한 근거를 남깁니다. 디버깅 로그에 토큰·비밀번호·개인정보를 노출하지 않습니다.

## Superpowers 관련 원문

- [systematic-debugging](../references/superpowers/skills/systematic-debugging/SKILL.md): 원인 조사, 패턴 비교, 가설 검증, 수정 절차.
- [verification-before-completion](../references/superpowers/skills/verification-before-completion/SKILL.md): 해결을 주장하기 전 검증.
- [diagnosing-superpowers](../references/superpowers/skills/diagnosing-superpowers/SKILL.md): Superpowers 자체의 세션 동작 문제 분석.

세션 로그를 외부에 내보내거나 이슈로 게시하는 일은 단순한 로컬 조사와 별개로 취급합니다.
