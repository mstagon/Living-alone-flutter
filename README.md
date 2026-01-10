<!-- 포트폴리오 저장소 내 문서입니다. 실제 레포 README로 옮길 땐 이미지 경로를 조정하세요. -->

# 🏠 Moyang

## 모두가 살 수 있는 내 집 마련을 위해, 모두의 양도 모양

```text
COPYRIGHT 2024 Moyang INC. ALL RIGHTS RESERVED.
위 웹사이트는 "Moyang"의 저작물이므로 상업적 이용을 금합니다.
```

<p align="center">
  <img src="./moyanghero.png" width="700" alt="Moyang Hero" />
</p>

---

## 🧑‍🦲 팀원(가나다순)

<table>
  <tbody>
    <tr>
      <td align="center"><a href="https://github.com/astraglus03"><img src="https://avatars.githubusercontent.com/u/123796383?v=4" width="100px;" alt=""/><br /><sub><b>김건동</b></sub></a><br /><sub><b>개발</b></sub></td>
      <td align="center"><a href="https://github.com/mstagon"><img src="https://avatars.githubusercontent.com/u/83182868?v=4" width="100px;" alt=""/><br /><sub><b>최민석</b></sub></a><br /><sub><b>개발</b></sub></td>
    </tr>
  </tbody>
</table>

---

## 🎬 프로젝트 개요

### 01. 프로젝트 주제

> 자취방/시설(주차장·창고 등) **양도 게시글 탐색 + 거래 연결** 커뮤니티 앱

### 02. 프로젝트 소개

Flutter 기반 크로스 플랫폼 앱으로, 게시글 탐색 → 문의(채팅)로 이어지는 흐름이 끊기지 않도록 구성했습니다.

- **게시글**: CRUD, 댓글/찜/신고 등 커뮤니티 기능
- **탐색**: 다중 조건 필터(가격/옵션 등) + 지도 기반 조회(마커)
- **채팅**: STOMP(WebSocket) 기반 실시간 채팅(재연결/오프라인 큐잉)
- **인증/보안**: 토큰 Secure Storage 저장 + 생체 인증(Local Auth)
- **API/상태**: Dio + Retrofit(codegen), Riverpod v2 + GoRouter

### ⌛ Developed Period

##### 2024.12 ~

### 03. 프로젝트 필요성

- **모바일 네트워크 변동(끊김/재연결)**
  - 채팅이 핵심 기능인 앱에서 연결이 끊기지 않도록 상태/재시도/큐잉 처리가 필요했습니다.
- **복잡한 탐색 조건**
  - 가격/옵션/지역 등 조합 필터를 안정적으로 관리할 상태 구조가 필요했습니다.

### 04. 주요 기능

- **STOMP 실시간 채팅**: 재연결 + 오프라인 큐잉 + 순서 보장(타임스탬프)
- **지도 기반 탐색**: 뷰포트 기반 로딩/클러스터링으로 렌더링 부담 완화
- **다중 조건 필터**: 중앙 상태(StateNotifier) 기반으로 조합 로직 단순화
- **타입 안전 API**: Retrofit + JSON serialization + codegen
- **보안 기능**: Secure Storage, Local Auth

---

## 📷 주요 화면

> 화면 GIF/스크린샷은 **추가 예정**입니다.

---

## ⚙️ 기술 스택

### 📚 Tech Stack

#### 💻 Development

<img src="https://skillicons.dev/icons?i=flutter&perline=8" />

#### State management

- Riverpod v2

#### HTTP network

- Dio & Retrofit

#### 기타(프로젝트 내 사용)

- GoRouter
- STOMP(WebSocket)
- Flutter Secure Storage, Local Auth, ScreenUtil

### Backend / Infra

- **미정/추가 예정** (프론트 레포 기준 공개)

---

## 🌐 서버 정보

- **배포**: 미정/추가 예정

---

## 🗓️ WBS / 요구사항 / ERD / DDL / DML

> 문서화 자료는 **추가 예정**입니다.

---

## ⚙️ 로컬 실행 방법

### 1. 레포지토리 클론

```bash
git clone https://github.com/mstagon/MoYang_FrontEnd
cd MoYang_FrontEnd
```

### 2. 실행

- **추가 예정** (Flutter run, 환경 변수/백엔드 URL 설정 포함)

---

## 🎉 회고

채팅(STOMP), 지도(마커), 복잡한 필터처럼 상태가 복잡한 화면에서 Riverpod으로 상태를 정리하는 경험을 했습니다.  
다음에는 테스트/모니터링을 더 일찍 붙이고, 오프라인 동작 범위를 명확히 정의해서 기능을 확장하고 싶습니다.

---

## 📄 라이선스

- 미정 (추가 예정)

---

## 📞 문의

- **Email**: devcms21@gmail.com
- **Portfolio**: https://devcms.me/projects/moyang

---

## 🎯 Commit Convention

- feat: Add a new feature
- fix: Bug fix
- rename: Change the structure, such as changing the file/folder name or moving it
- remove: Delete a file
- refactor: Code refactoring
- test: Test code, adding refactoring tests
