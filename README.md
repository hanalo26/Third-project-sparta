━━━━━━━━━━━━━━━━━━━
📦 최초 환경 세팅
━━━━━━━━━━━━━━━━━━━

⚠️ uv가 설치되어 있지 않은 경우 먼저 설치해 주세요:
- Windows (PowerShell)
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
- macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
설치 후 터미널을 재시작해 주세요!

1️⃣ 레포 clone
`git clone https://github.com/hanalo26/Third-project-sparta.git`

2️⃣ 폴더 이동
`cd Third-project-sparta`

3️⃣ 환경 세팅
`uv sync`
→ uv sync 한 번으로 **Python 3.12 + 필요한 라이브러리**가 자동으로 설치됩니다!

━━━━━━━━━━━━━━━━━━━
📚 설치된 주요 라이브러리
━━━━━━━━━━━━━━━━━━━

파이썬 3.12 기준

- pandas : 데이터 전처리, 테이블 조작
- numpy : 수치 연산
- scipy : 통계 검정
- statsmodels : 회귀분석, 시계열 등 통계 모델
- matplotlib : 기본 시각화
- seaborn : 통계 시각화
- scikit-learn : 머신러닝 / 전처리 도구
- jupyter : 노트북 환경
- pingouin : 통계 검정 (t-test, ANOVA 등)
- plotly : 인터랙티브 시각화

━━━━━━━━━━━━━━━━━━━
🔄 Git 사용 시 주의사항
━━━━━━━━━━━━━━━━━━━

✅ 작업 시작 전 항상 pull 먼저!
`git pull`

→ 다른 팀원 변경사항을 먼저 받아야 충돌을 방지할 수 있습니다.

✅ 새 라이브러리가 추가된 경우 pull 후 반드시 sync!
`uv sync`

→ `pyproject.toml`이 바뀌었을 수 있으니 꼭 sync 해주세요.

✅ add할 때, 자신이 만든 파일만 업로드하기

-> add하기 전에는 팀원들에게 공유해주세요! 그래야 충돌로 인한 사고를 예방할 수 있습니다.

`git add 파일명.ipynb` 또는 `git add ./하위폴더명/파일명.ipynb`

✅ 커밋 메시지를 작성하는 코드 

`git commit -m "커밋 메세지"`

✅ `git push`로 마무리

⚠️ 데이터 파일(.csv, .xlsx 등)은 Github가 아닌 구글 공유드라이브로 공유해 주세요!
→ `.venv/, 데이터 파일(.csv, .xlsx 등)`은 `.gitignore`에 등록되어 있으니 걱정은 살짝 내려놓으셔도 됩니다.