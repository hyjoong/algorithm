[Daily Algorithm_JavaScript] Level1. K번째수

### Question
배열 array, [i, j, k]를 원소로 가진 2차원 배열 commands가 매개변수로 주어질 때, commands의 모든 원소에 대해 앞서 설명한 연산을 적용했을 때 나온 결과를 배열에 담아 return 하도록 solution 함수를 작성해주세요.
</br>

#### Source https://programmers.co.kr/learn/courses/30/lessons/42748
</br>

### My solution
```javascript
function solution(array, commands) {
    var answer = [];
      for(let i =0;i<commands.length;i++){ 
          let start=(commands[i][0])-1
          let end = (commands[i][1])  
          let sliced = array.slice(start,end);
          sliced.sort((a,b)=>a-b)   // 오름차순
          answer.push(sliced[commands[i][2]-1]);
      }
      return answer;
}
```


#### Other Solutions

```javascript
function solution(array, commands) {
    return commands.map(command => {
        const [sPosition, ePosition, position] = command
        const newArray = array
            .filter((value, fIndex) => fIndex >= sPosition - 1 && fIndex <= ePosition - 1)
            .sort((a,b) => a - b)    

        return newArray[position - 1]
    })
}
```