# PGR2M_Demo

Motion Generation and Editing Gallery - comparing CoMo and PGR2M results.

## 🌐 GitHub Pages Setup

### 1. GitHub Pages 활성화하기

1. GitHub 저장소로 이동
2. **Settings** 탭 클릭
3. 좌측 메뉴에서 **Pages** 클릭
4. **Source** 섹션에서:
   - Branch: `main` (또는 `master`) 선택
   - Folder: `/ (root)` 선택
5. **Save** 버튼 클릭
6. 몇 분 후 `https://<username>.github.io/PGR2M_Demo/` 에서 사이트 확인 가능

### 2. GIF 파일 업로드하기

다음 폴더에 GIF 파일들을 업로드하세요:

#### Text-to-Motion Generation
- 경로: `assets/text-to-motion/`
- 파일명 예시:
  - `como_example1.gif`, `como_example2.gif`, ...
  - `ours_example1.gif`, `ours_example2.gif`, ...

#### Motion Editing
- 경로: `assets/motion-editing/`
- 파일명 예시:
  - `como_example1.gif`, `como_example2.gif`, ...
  - `ours_example1.gif`, `ours_example2.gif`, ...

### 3. 콘텐츠 추가/수정하기

`index.html` 파일을 편집하여:
- 프롬프트 텍스트 수정 (`<h3 class="prompt-text">` 부분)
- 더 많은 예시 추가 (comparison-item 블록 복사/붙여넣기)
- GIF 파일 경로 업데이트

### 4. 디자인 커스터마이징

`style.css` 파일에서 색상, 레이아웃, 크기 등을 조정할 수 있습니다.

## 📁 프로젝트 구조

```
PGR2M_Demo/
├── index.html              # 메인 갤러리 페이지
├── style.css               # 스타일시트
├── assets/
│   ├── text-to-motion/     # Text-to-Motion GIF 파일들
│   │   ├── como_example1.gif
│   │   ├── ours_example1.gif
│   │   └── ...
│   └── motion-editing/     # Motion Editing GIF 파일들
│       ├── como_example1.gif
│       ├── ours_example1.gif
│       └── ...
└── README.md
```

## 🎨 페이지 구성

- **좌측 섹션**: Text-to-Motion Generation
- **우측 섹션**: Motion Editing
- 각 섹션에서 CoMo와 Ours 방법을 나란히 비교
- 반응형 디자인 (모바일/태블릿 지원)

## 🚀 로컬에서 테스트하기

```bash
# 간단한 HTTP 서버로 로컬 테스트
python -m http.server 8000

# 또는
python3 -m http.server 8000
```

그런 다음 브라우저에서 `http://localhost:8000` 접속