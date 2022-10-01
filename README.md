# React test library jest-dom 사용한 소스

Eslint, Prettier, gest-dom 등 테스트 케이스 작성에 필요한 eslint 설정
expect, tobe 간단한 작성법 숙지 
dom element 선택, screen 메소드
e.g., 
test('minus button has correct text', () => { 
  render(<App />)

  const buttonElement = screen.getByTestId('minus-button')
  expect(buttonElement).toHaveTextContent('-')
 })

## 깃허브 액션을 통한 aws 컨테이너 자동배포

node.js configure 안의 yml 파일 작성 및 aws s3 컨테이너 정보 붙여넣기
참고한 s3-action: https://github.com/awact/s3-action

정적 웹 사이트 호스팅 편집 - 정적 호스팅을 위한 엔드포인트 제공

aws s3 컨테이너 설정, IM 사용자 생성 및 인증키 - 깃허브에서 시크릿으로 환경변수화

퍼블릭 액세스 차단(버킷설정) 정책 JSON 변경 
https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-policy-language-overview.html

빌드 된 결과물 (정상작동 확인 후 현재는 비활성화)
Prototype: http://react-deploy-action-test-bucket.s3-website.ap-northeast-2.amazonaws.com/
