---

# Today I learned

20191219

Today what I learned

SyntheticEvent는 풀링됩니다. 성능상의 이유로 SyntheticEvent 객체는 재사용되고 모든 속성은 이벤트 핸들러가 호출된 다음 초기화됩니다. 따라서 비동기적으로 이벤트 객체에 접근할 수 없습니다.

20191218

Today what I did

몇달 전 부터 진행 해온 [리팩토링구루](https://refactoring.guru/) 에 있는 Design pattern을 2개씩 읽고 토론 하는 것을 종료 하였다. 처음 부터 끝까지 모든 디자인 패턴을 한번씩 훓고 나니 디자인 패턴에 대해 좀 이해가 생겼다. 비록 react개발을 해서 functional programming을 하지만 디자인 패턴이 개발에 미약하게라도 도움이 되고 있지 않나 생각한다.

20191217

Today what I heard
Dan Abramov가 내가 자주쓰던 lodash의 cloneDeep을 사용하지 않고 대신 부분만 변경하여 업데이트 하는 방식으로 immer를 추천 하였다. 역시 immer를 써야 하나 보다.

20191214

Today what I did
useEffect 완벽 가이드를 한번 더 읽었다. 아무래도 이건 좀 더 이해가 필요 할거 같아 한번 죽 정리를 해서 최소한 내가 이해한 만큼은 블로그에 포스팅 해야겠다.

20191213

Today what I did

- async await을 사용 할때 여러개의 await을 빠른 속도로 처리 하기 위해 할 수 있는 방법은 await을 promise all로 한꺼번에 받아서 처리하면 좀더 나은 속도로 처리가 가능하다.

20191209

Today what I did

- thunk를 사용 하다 dispatch를 중간에 하나 더 추가 하여 비동기로 받은 데이터에서 필요한 데이터 하나만 다른 reducer로 보내는걸 해봤다. 이런 식으로 사용 한다면 thunk로 좀 더 복잡한 개입이 가능하다는 걸 알게 되었다. pyramid 알고리즘을 연습했다.

20191208

Today what I did

- redux thunk의 loading 함수를 만들어서 적용 해보았다. pender를 사용하기 싫어서 써보았는데 나름 괜찮은 방법이였다. redux-saga와 redux-observable도 있다고 하는데 이것들도 살펴 봐야겠다.
- 복습겸 지금까지 풀었던 AlgoCasts 중 어려웠던 문제를 다시 한번 보았다.

20191207

Today what I did

- redux thunk에 연동 시킬 loading 연습을 시작하였다. 오늘은 간단히 시작만 하고 내일 마무리 까지 해야지. 유틸 loading 함수를 만드는 것으로 알고 있지만 다른 방법(예를 들어 customer hooks 같은)이 있는지도 찾아봐야겠다.
