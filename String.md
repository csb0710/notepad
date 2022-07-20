# String

#### 9251번 :  LCS (골드5)
  * 문제 유형 : dp, String
  * 시간 복잡도 : O(nm)
  * 풀이 방식 : 
  ```
  두 문자열의 위치를 나타내는 2차원 int 배열 dp 선언(0으로 초기화, 인덱스는 i, j로 표현)
  각 문자열의 현재 문자가 같을 경우 dp[i][j] = dp[i-1][j-1]
  다를 경우 dp[i][j] = Math.max(dp[i-1][j], dp[i][j-1]) -> 현재까지 구한 LCS의 길이를 뜻함
  dp의 마지막 값이 LCS의 길이를 뜻함
  ```
  
#### 9252번 :  LCS2 (골드4)
  * 문제 유형 : dp, String
  * 시간 복잡도 : O(nm)
  * 풀이 방식 : 
  ```
  9251번과 같은 방식으로 dp 배열을 구하고 마지막 값부터 시작하여 dp[i-1][j]와 dp[i][j-1] 중 dp[i][j]가 같은 값이 존재할 경우 해당 위치로 이동
  같은 값이 없을 경우 해당 위치의 문자를 Stack에 추가 후 dp[i-1][j-1]로 이동 -> 해당 dp의 위치가 두 문자열에서 현재 문자를 찾은 순간이기 때문에 현재 문자를 stack에 추가하고 현재 문자 전 위치의 dp로 이동
  ```