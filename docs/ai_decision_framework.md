# AI Decision Framework

## Classification Threshold Logic

- Confidence > 85% → Auto Apply
- 60%–85% → Suggested Recommendation
- < 60% → Manual Review Required

## Safeguards

- Amount mismatch tolerance: ±2%
- Date tolerance: ±3 days
- Vendor string similarity threshold: 0.8 cosine similarity

## Continuous Learning Loop

1. Capture user overrides
2. Log misclassifications
3. Weekly retraining cycle
4. Deploy model versioned release
