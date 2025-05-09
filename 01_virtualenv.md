# venv
- PowerShell 실행 정책 조정 (최초 1회 필요)
가상 환경의 활성화 스크립트는 기본 정책상 실행되지 않을 수 있으니, 정책을 완화해 줍니다. (관리자 권한으로 실행 권장)

```sh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

- 가상환경 만들기
```
# 프로젝트 폴더 만들기
mkdir test_project
cd test_project

# 가상환경 만들기
python3 -m venv venv

# 가상환경 활성화
.\venv\Scripts\Activate.ps1
# source ./venv/Scripts/activate

# 가상환경 비활성화
deactivate
```

> 윈도우 터미널 : https://github.com/microsoft/terminal
- 파이썬 특정 버전으로 가상 환경 만들기
```
mkdir test_project
cd test_project
py -3.12 -m venv .venv  #<<==
.\venv\Scripts\Activate.ps1
```

# uv
- Astral이 만든 uv는 2024년 초에 출시되어, pip, poetry, conda 등 다양한 도구들의 장점을 통합하고, Rust를 활용한 초고속 의존성 해석(Resolver)으로 큰 주목을 받고 있다.
- Anthropic, OpenAI 를 포함한 실제 ML/DS(데이터 사이언스), 백엔드, 오픈소스 프로젝트 등 여러 분야에서 uv 도입 사례가 급격히 늘고 있다.
> 사이트 : [https://www.datacamp.com/tutorial/python-uv](https://docs.astral.sh/uv/getting-started/installation/)

- 



