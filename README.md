## 목표

- 알고리즘 능력 향상
- 나의 풀이와 다른 사람의 풀이를 비교해보고 내 풀이에 대한 셀프 피드백
- 다시 봐야 할 문제와 기억하고 싶은 코드는 블로그 포스팅

</br>
 
## 문제 출처

### Sites

- [프로그래머스](https://programmers.co.kr/)
- [백준](https://www.acmicpc.net/)
- [인프런](https://www.inflearn.com/course/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EB%AC%B8%EC%A0%9C%ED%92%80%EC%9D%B4/dashboard)

## tip

- 한 문제를 여러가지 방법으로 풀도록 탐구해보기
- 30분~60분 까지 고민해 본다.
- 어려우면 솔루션을 찾아본다.
- 문제 풀이의 흔적을 남기기 위해서 나의 솔루션을 업로드
- 가능 하면 매일 매일 풀이하여 일일커밋에 도전하기

#### 복습

- 격자판 최대합
  - Math.max(answer, sum1, sum2); // 3개 중의 최대 값 찾아냄
  - Math.max(...arr) // arr 배열안에 요소중의 최대 값 찾아냄 
- 쵀대값 구하는 문제에서 처음 숫자가 할당되게 하려고
  - let temp = Number.MIN_SAFE_INTEGER;
- Math.floor(x) : 소숫점 버리고 내림

- [Array.from](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/from)

- array.sort((a,b)=>a-b)   // 오름차순

- trim() = 문자열 양 끝의 공백을 제거 (모든 공백 제거가 아니라 양 끝의 공백)

- 동적 계획법: 모든 방법을 일일이 검토하여 최적의 해를 찾아내는 방식의 알고리즘
- 그리디 알고리즘: 모든 해를 구하지 않고 순간마다 그 순간에서의 최적의 해를 찾는 방식