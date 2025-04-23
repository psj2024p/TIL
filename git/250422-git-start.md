## 1. Shell과 Git Bash 기본

### Shell
- 사용자와 운영체제의 커널 사이를 연결하는 소프트웨어
- 커널(Kernel): 운영체제의 핵심으로, 하드웨어를 제어

### Git Bash (Windows)
- Windows 환경에서 Git을 사용할 수 있도록 도와주는 도구
- Bash 쉘을 에뮬레이션하여 Git 명령어 사용 가능
- 설치 사이트: https://gitforwindows.org

---

## 2. 셸 명령어 기초

### 위치 및 조회
| 명령어 | 설명 |
|--------|------|
| `pwd` | 현재 경로 출력 (print working directory) |
| `ls` | 현재 디렉토리의 목록 출력 |
| `ls -a` | 숨김파일 포함 목록 출력 |
| `ls -l` | 상세 정보 출력 |
| `ls -al` | 숨김파일 포함 + 상세 정보 출력 |
| `clear` | 터미널 화면 초기화 |

### 디렉토리 이동
| 명령어 | 설명 |
|--------|------|
| `cd 디렉토리명` | 해당 디렉토리로 이동 |
| `cd ..` | 상위 디렉토리로 이동 |

### 디렉토리 및 파일 작업
| 명령어 | 설명 |
|--------|------|
| `mkdir 폴더명` | 새 디렉토리 생성 |
| `touch 파일명` | 새 파일 생성 |
| `mv 파일 대상` | 파일 이동 또는 이름 변경 |
| `rm 파일명` | 파일 삭제 |
| `rm -rf 폴더명` | 폴더 및 하위 파일 강제 삭제 |

---

## 3. Vim 기본 사용법

### 모드
- Normal Mode: 기본 모드 (Esc)
- Insert Mode: 입력 모드 (`i` 키)
- Visual Mode: 선택 모드 (`v` 키)
- Command Mode: 명령 모드 (`:` 키)

### 주요 명령
| 명령어 | 설명 |
|--------|------|
| `:wq` | 저장하고 종료 |
| `:q!` | 저장하지 않고 강제 종료 |
| `u` | 실행 취소 |
| `yy` | 한 줄 복사 |
| `p` | 붙여넣기 |

---

## 4. Git 사용 흐름

### 저장소 복제
```bash
git clone <저장소 주소>
```

### 파일 상태 확인
```bash
git status
```

### 변경사항 저장
```bash
git add 파일명       # 스테이징
git commit           # 커밋 (편집기 열림)
git log              # 커밋 내역 확인
```

### 원격 저장소 푸시
```bash
git push origin main
```

---

## 5. Markdown 작성법

- `README.md` 파일 작성 시 사용
```markdown
# 제목
## 소제목
- 목록 항목
```

---

## 6. Git 커밋 메시지 규칙 (Conventional Commits)

| 접두어 | 의미 |
|--------|------|
| `feat` | 새로운 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 관련 변경 |
| `refactor` | 코드 리팩토링 |

예시:
```
feat: Add login feature
fix: Correct typo in error message
```

---

## 7. 브랜치 사용

### 브랜치 작업 흐름
```bash
git branch 브랜치명        # 브랜치 생성
git switch 브랜치명        # 브랜치 전환
```

### 병합
```bash
git switch main
git merge 브랜치명
```

### 브랜치 삭제
```bash
git branch -D 브랜치명
```

---

## 8. 기타 유용한 명령어

| 명령어 | 설명 |
|--------|------|
| `cat 파일명` | 파일 내용 출력 |
| `python 파일.py` | 파이썬 실행 |
| `Ctrl + C` | 실행 중단 |
| `Tab` | 경로 자동완성 |
| `git config --global core.autocrlf true` | Windows 환경 줄바꿈 문제 방지 설정 |

---

