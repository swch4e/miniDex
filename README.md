# MiniDEX 실습 dApp

탈중앙화금융 제5장 실습용 웹 화면입니다. Sepolia 테스트넷의 MiniDEX 컨트랙트에 MetaMask로 연결합니다.

## 파일
- `index.html` — dApp 화면 전체 (HTML·CSS·JS 한 파일)
- `ethers-6.17.0.umd.min.js` — 블록체인 연결 라이브러리 (ethers v6, MIT 라이선스)

## 설정
`index.html` 맨 아래 `CONFIG`의 두 줄에 교수자가 배포한 주소를 넣습니다.

```js
HSUSD: "0x...",   // HSUSD 컨트랙트 주소
DEX:   "0x...",   // MiniDEX 컨트랙트 주소
```

파일을 고치지 않고 접속 주소 뒤에 `?hsusd=0x...&dex=0x...`를 붙여도 됩니다.

## 실행
- 로컬 확인: 이 폴더에서 `python3 -m http.server 8000` → 브라우저에서 `http://localhost:8000`
- 공개 배포: GitHub 공개 저장소에 두 파일을 올리고 Settings → Pages → Deploy from a branch → `main` / `(root)`

서버·데이터베이스가 없으며, 모든 거래는 학생의 MetaMask에서 직접 서명합니다. 수업용 테스트넷 전용입니다.
