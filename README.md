# GC Care 헬스 데이터 인사이트 포털

## 폴더 구조

```
gc-health-portal/
├── index.html          ← 디자인 엔진 (건드리지 않음)
├── data/
│   └── latest.json     ← 매주 이 파일만 업데이트
├── scripts/
│   └── fetch_data.py   ← 데이터 자동 수집 (추후 연결)
└── README.md
```

## 매주 업데이트 방법

1. GitHub에서 `data/latest.json` 파일 열기
2. 숫자/텍스트 수정 후 Commit
3. Vercel 자동 배포 완료

## latest.json 구조

| 항목 | 설명 |
|------|------|
| `meta` | 주차, 기간, 발행일 |
| `symptoms` | 주간 급상승 증상 리스트 |
| `heatmap` | 히트맵 타이틀, 범례, 출처 |
| `healthDebt` | 건강 부채 추적기 출처 |
| `activeSaver` | 검진자 개선 추이 출처 |
| `prescription` | 처방 현황 수치 |
