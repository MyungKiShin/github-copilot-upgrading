# upgraded 디렉터리 파일 구조 설명

```
upgraded/
├── MANIFEST.in                # 패키징을 위한 매니페스트 파일
├── README.rst                 # 프로젝트 설명서 (reStructuredText)
├── distribute-0.6.10.tar.gz   # distribute 패키지 소스 아카이브
├── distribute_setup.py        # distribute 설치 스크립트
├── docs/                      # Sphinx 기반 문서 디렉터리
│   ├── Makefile               # 문서 빌드용 Makefile
│   ├── build/                 # 빌드된 문서 결과물
│   │   ├── doctrees/          # Sphinx 문서 트리 데이터
│   │   └── html/              # HTML 문서 결과물
│   │       ├── _sources/      # HTML 소스 텍스트
│   │       └── _static/       # HTML 정적 파일(css, js, 이미지 등)
│   └── source/                # 문서 원본(rst, conf.py 등)
│       └── _static/           # 문서용 커스텀 CSS 등
├── guachi/                    # 주요 Python 패키지 소스
│   ├── __init__.py            # 패키지 초기화
│   ├── config.py              # 설정 관련 코드
│   ├── database.py            # 데이터베이스 관련 코드
│   └── tests/                 # 테스트 코드
│       ├── test_configmapper.py
│       ├── test_configurations.py
│       ├── test_database.py
│       └── test_integration.py
├── guachi.egg-info/           # 패키징 메타데이터
│   ├── PKG-INFO
│   ├── SOURCES.txt
│   ├── dependency_links.txt
│   └── top_level.txt
└── setup.py                   # 패키지 설치/설정 스크립트
```

- `docs/`는 Sphinx로 생성된 문서와 원본, 빌드 결과를 포함합니다.
- `guachi/`는 실제 Python 소스와 테스트가 들어 있습니다.
- `guachi.egg-info/`는 패키징 시 생성되는 메타데이터입니다.
- `setup.py`, `MANIFEST.in` 등은 Python 패키징 표준 파일입니다.
- 숨김 파일 및 기타 하위 디렉터리도 모두 복사되었습니다.
