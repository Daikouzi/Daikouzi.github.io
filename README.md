# PROMISEON VINA — Static Website

[PROMISEON VINA](https://daikouzi.github.io/)의 다국어 홈페이지 정적 사이트입니다. WordPress에서 콘텐츠를 export한 뒤 순수 HTML/CSS/JS 정적 페이지로 변환하여 GitHub Pages로 호스팅합니다.

## 사이트 구성

기본 언어는 베트남어(`vi`)이며, 한국어/영어 페이지가 별도 경로로 제공됩니다.

| 경로 | 설명 |
| --- | --- |
| `/index.html` | 메인 페이지 (베트남어) |
| `/introduction/` | 회사 소개 |
| `/introduction_kr/`, `/introduction_en/` | 회사 소개 (한국어 / 영어) |
| `/main_page_kr/`, `/main_page_en/` | 메인 페이지 (한국어 / 영어) |
| `/select_promiseon/`, `/select_promiseon_kr/`, `/select_promiseon_en/` | PROMISEON을 선택하는 이유 |
| `/contract_kr/`, `/contract_en/` | 계약 안내 (한국어 / 영어) |
| `/contact/` | 연락처 및 문의 |

각 경로는 `index.html`을 포함한 정적 디렉터리이며, 별도의 라우팅 없이 GitHub Pages가 경로를 그대로 서빙합니다.

## 기술 구성

- **콘텐츠 소스**: WordPress(wordpress.com) 사이트에서 export한 정적 페이지
- **정적 자산**: `wp-content/`, `wp-includes/`, `i/`, `_static/`에 테마 CSS, 미디어, 아이콘 폰트 등 원본 리소스 보존
- **호스팅**: GitHub Pages (빌드 과정 없이 저장소 파일을 그대로 배포)

## 로컬에서 확인하기

별도의 빌드 도구 없이 정적 파일을 그대로 서빙하면 됩니다.

```bash
# 저장소 루트에서
python3 -m http.server 8080
# 브라우저에서 http://localhost:8080 접속
```

## 페이지 수정 방법

1. 수정할 언어/섹션에 해당하는 디렉터리의 `index.html`을 직접 편집합니다.
2. 이미지·문서 등 신규 미디어는 `wp-content/uploads/`에 연도별 폴더 구조를 유지하며 추가합니다.
3. 변경 사항을 커밋 후 `main` 브랜치에 푸시하면 GitHub Pages에 자동 배포됩니다.

## 연락처

- Email: hongthu.promise@gmail.com
- Tel: 039 496 5617
- Zalo: [zalo.me/0394965617](https://zalo.me/0394965617)
- Facebook: [facebook.com/promiseonvn](https://www.facebook.com/promiseonvn)
- Instagram: [instagram.com/promiseon](https://instagram.com/promiseon)
- YouTube: [youtube.com/promiseon](https://youtube.com/promiseon)
