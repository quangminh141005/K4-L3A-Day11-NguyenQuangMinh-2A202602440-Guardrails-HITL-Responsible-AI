# Lab 11 — Auto Report

> File này **tự sinh** bởi `scripts/grade.py`. **Không** viết / sửa tay.

- Generated (UTC): `2026-09-26T16:16:54.917802+00:00`
- Framework: `openai-sdk/openrouter`
- Technical failure: **False**

## Packaging

| File | Status |
|------|--------|
| results.json | OK |
| attack_results.json | OK |
| audit_log.json | OK |
| metrics.json | OK |

## Schema (`results.json`)

- Valid: **True**
- Error: `None`

## Defense snapshot (từ `results.json`)

- Safe queries blocked: `0/5`
- Attack queries blocked: `6/7`
- Edge cases blocked: `2/3`
- Rate limit blocked/sent: `3/13`

## Red Team snapshot (từ `attack_results.json`)

- Provider / model: `gemini` / `gemini-3.5-flash-lite`
- Unsafe leaks (Red): `9/10`
- Guards leaks (Red Advance): `0/10`

## Public tests

- Return code: `1`
- Technical failure: `False`

```text
.F........                                                               [100%]
=========================== short test summary info ============================
FAILED tests/public/test_lab_contracts.py::test_detect_indirect_unicode_injection_without_blocking_benign_external_data
1 failed, 9 passed in 0.63s
```

## Notes

- Artifact chấm chính: `outputs/results.json` + `outputs/attack_results.json`.
- Bonus B1/B2 do grader replay quyết định — JSON chỉ là bằng chứng.
- Không nộp `report/*.md` viết tay; dùng file này nếu cần xem tóm tắt.
