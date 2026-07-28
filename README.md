# Conference Deadline Tracker

보안·프라이버시(Security) 및 AI 상위 학회 마감일 카운트다운 사이트입니다. 현재 총 26개 학회를 추적합니다.

- **Security** (9): USENIX Security, S&P, CCS, NDSS, Euro S&P, AsiaCCS, ACSAC, ESORICS, RAID
- **AI3** (9): AAMAS, ACM MM, AISTATS, CICLing, COLING, CoNLL, EACL, IJCNLP, KDD
- **AI4** (8): AAAI, ACL, EMNLP, ICLR, IJCAI, NAACL, NeurIPS, ICML

🔗 **사이트**: https://namgyupark22.github.io/mas-sec-deadlines/

카테고리 필터(전체 / Security / AI3 / AI4)로 원하는 분야만 볼 수 있습니다.

## 데이터 출처
- Security: [sec-deadlines.github.io](https://sec-deadlines.github.io/)
- AI: 각 학회 공식 CFP 페이지를 직접 확인해 반영. 다음 CFP가 아직 공개되지 않은 학회는 날짜를 임의로 채우지 않고 "CFP 대기"로 표시합니다.

## 업데이트 방법
새 CFP가 뜨면 `index.html`의 `CONFS` 배열에서 해당 학회의 `deadlines`(및 `dates`, `place`, `url` 등)를 수정하면 됩니다. 새 학회를 추가할 때는 `category`를 `security` / `ai3` / `ai4` 중 하나로 지정하세요.
