# Conference Deadline Tracker

보안·프라이버시(Security), AI 상위 학회, PL/SE 학회 마감일 카운트다운 사이트입니다. 현재 총 33개 학회를 추적합니다.

- **Security** (9): USENIX Security, S&P, CCS, NDSS, Euro S&P, AsiaCCS, ACSAC, ESORICS, RAID
- **AI3** (9): AAMAS, ACM MM, AISTATS, CICLing, COLING, CoNLL, EACL, IJCNLP, KDD
- **AI4** (8): AAAI, ACL, EMNLP, ICLR, IJCAI, NAACL, NeurIPS, ICML
- **PL/SE** (7): ICSE, POPL, OOPSLA, ISSTA, ASE, PLDI, FSE — "전체" 필터에는 포함되지 않고 별도 탭에서만 보입니다.

🔗 **사이트**: https://namgyupark22.github.io/mas-sec-deadlines/

카테고리 필터(전체 / Security / AI3 / AI4 / PL/SE)로 원하는 분야만 볼 수 있습니다. "전체"는 Security+AI3+AI4(26개)만 포함하며 PL/SE는 별도 탭에서 확인합니다.

## 데이터 출처
- Security: [sec-deadlines.github.io](https://sec-deadlines.github.io/)
- AI / PL/SE: 각 학회 공식 CFP 페이지를 직접 확인해 반영. 다음 CFP가 아직 공개되지 않은 학회는 날짜를 임의로 채우지 않고 "CFP 대기"로 표시합니다.

## 업데이트 방법
새 CFP가 뜨면 `index.html`의 `CONFS` 배열에서 해당 학회의 `deadlines`(및 `dates`, `place`, `url` 등)를 수정하면 됩니다. 한 회차의 마감이 전부 지나면 매년 열리는 학회는 다음 회차(연도)로 넘기고, 다음 CFP가 아직 없으면 `deadlines: []`로 두어 "CFP 대기"로 표시합니다. 개최 주기가 일정하지 않은 학회(EACL, AACL-IJCNLP 등)는 다음 회차가 확정되기 전까지 현재 회차를 그대로 둡니다. 화면 상단의 `last data sync` 날짜도 함께 갱신하세요. 새 학회를 추가할 때는 `category`를 `security` / `ai3` / `ai4` / `plse` 중 하나로 지정하세요. `plse`는 "전체" 필터(`inFilter` 함수, index.html)에서 자동으로 제외됩니다.
