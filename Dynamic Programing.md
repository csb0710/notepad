#### 9251번 :  LCS (골드5)
  * 문제 유형 : dp, 문자열
  * 시간 복잡도 : O(nm)
  * 풀이 방식 : 
  *
  ```
  두 문자열의 위치를 나타내는 2차원 int 배열 dp 선언(0으로 초기화, 인덱스는 i, j로 표현)
  각 문자열의 현재 문자가 같을 경우 dp[i][j] = dp[i-1][j-1]
  다를 경우 dp[i][j] = Math.max(dp[i-1][j], dp[i][j-1]) -> 현재까지 구한 LCS의 길이를 뜻함
  dp의 마지막 값이 LCS의 길이를 뜻함
  ```