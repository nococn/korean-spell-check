---
name: korean-spell-check
description: Use Nara/PNU Korean spell-check surfaces conservatively to proofread Korean text, chunk long input, and return change-focused correction suggestions.
license: MIT
metadata:
  category: writing
  locale: ko-KR
  phase: v1
---

# Korean Spell Check

NomaDamas/k-skill의 korean-spell-check만 분리한 독립 배포입니다. 전체 안내는 [instruction.md](instruction.md)를 읽습니다. Node.js CLI 없이 포함된 Python helper를 직접 사용합니다.

```bash
python3 scripts/korean_spell_check.py --text "아버지가방에들어가신다." --format text
python3 scripts/korean_spell_check.py --file input.md --format json
```

Python 3.10+ 및 인터넷 연결이 필요합니다. 원문은 외부 맞춤법 검사 서비스로 전송됩니다. 민감정보는 먼저 제거하고 개인·학생의 비상업적 저빈도 검수에만 사용합니다. 서비스 응답과 정책은 바뀔 수 있으며 차단을 우회하지 않습니다.
