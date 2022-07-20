# Graphs

## bfs
#### 16236번 :  아기 상어 (골드3)
  * 문제 유형 : graphs, bfs, implementation, simulation
  * 시간 복잡도 : O(n^2)
  * 풀이 방식 : 
  ```
  - 상어가 먹을 수 있는 물고기들을 선택할 때 가장 가까운 거리에 위치한 물고기 중 선택해야하기 때문에 bfs를 이용
  - 거리가 같은 물고기일 경우 가장 왼쪽에 위치한 물고기, 왼쪽 거리도 같다면 가작 위쪽에 위치한 물고기를 선택해야하기 때문에 이에 맞게 우선순위큐의 compare 조건을 지정
  - 거리 1당 시간이 1씩 걸리기 때문에 선택한 물고기로 이동할 때마다 떨어진 거리(물고기까지의 bfs시행 횟수)만큼 더하여 총 이동 시간을 구한다
  ```