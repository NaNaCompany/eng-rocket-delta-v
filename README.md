# 치올콥스키 로켓 Δv 계산기

질량 감소와 유효 배기속도로 한 번의 이상적인 로켓 연소가 제공하는 Δv를 계산한다.

- ID: E101
- App: https://nanalab.kr/eng-rocket-delta-v/
- Repository: https://github.com/NaNaCompany/eng-rocket-delta-v
- Formula: Δv = v_e ln(m₀/m_f)

## Model and data

m₀≥m_f>0, 0<v_e<c. 두 질량은 해당 연소 직전·직후의 전체 기체 질량이다. 일정한 유효 배기속도와 같은 방향의 연속 배기를 쓰는 고전적 모델이다. 유효 배기속도에는 압력 추력의 등가 기여를 포함할 수 있다. 중력 손실·항력·외력·질량 투하·다단 분리는 제외한다. Δv≥c는 거부하며 광속에 가까운 운동에는 상대론 로켓식이 필요하다.

Inputs normalize to SI. Repeated-input models support adding/removing actual input rows. Calculations, finite-number checks and physical-domain checks run locally; no external property database or solver API is used.

## Validation

Run node --test tests/*.test.mjs and python scripts/build-locales.py --check. tests/reference.json contains independently computed high-precision default and boundary references. The source notices distinguish original MIT work from citation-only external references.

## Static languages

Korean (existing root), English (`en/`), Spanish (`es/`), Simplified Chinese (`zh/`), Japanese (`ja/`) and German (`de/`). Each page has its own canonical URL, reciprocal hreflang, localized metadata, interface, validation messages and preview image. The language links work without JavaScript. Calculation code is shared and no runtime translation API is used.

Edit `localization/*.json` for text, `src/template.html` for the shared page, and run `python scripts/build-locales.py`. Run `python scripts/build-locales.py --check` and `npm test` before publishing. Decimal commas are accepted in Spanish and German; thousands separators are not supported.
