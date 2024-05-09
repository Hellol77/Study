# RSC(React Server Component)

RSC 란 React Server Component 서버에서 렌더링되는 컴포넌트를 의미한다.

서버 컴포넌트는 async를 함수로 선언하고 내부에서 await을 사용하여 비동기 데이터를 가져와 이를 렌더링하는 것이 가능하다.(비동기 컴포넌트)

- RSC 에서는 useState, useEffect 등 클라이언트에서 사용되는 훅을 사용할 수 없다.
- OnClick onFocus 와 같은 이벤트 핸들러는 사용이 불가능하다
- 렌더가 완료되기 전까지 클라이언트에서는 React의 Suspense로 RSC 자리에 다른 컴포넌트를 대신 보여줄 수 있다.
- RSC에서 사용되는 패키지들은 모두 서버에서 import 되고 서버에서만 사용되기 때문에 js번들로 클라이언트에 전달되지 않는다

