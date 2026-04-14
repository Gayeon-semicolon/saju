# 천명 (天命) — 사주 × MBTI 운명 분석

사주팔자와 MBTI를 결합한 AI 운명 분석 웹사이트입니다.

## 파일 구조

```
cheonmyeong/
├── index.html       ← 프론트엔드 (UI 전체)
├── vercel.json      ← Vercel 설정
├── README.md
└── api/
    └── analyze.js   ← 백엔드 API 프록시 (API 키 보호)
```

## 배포 방법 (Vercel)

### 1단계: Node.js 설치 확인
```bash
node -v   # v18 이상 권장
npm -v
```

### 2단계: Vercel CLI 설치
```bash
npm install -g vercel
```

### 3단계: 배포
```bash
cd cheonmyeong
vercel
```

### 4단계: 환경변수 설정
Vercel 대시보드 → 프로젝트 → Settings → Environment Variables
- Key: ANTHROPIC_API_KEY
- Value: sk-ant-...

### 5단계: 재배포
```bash
vercel --prod
```
