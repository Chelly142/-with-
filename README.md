# 알고리즘 공부 wirh 파이썬
파이썬을 기본언어로 한 알고리즘 공부를 기록합니다.


# 그리드
- 탐욕법이라고도하며 가장 효율적인 방법을 찾는 알고리즘 
- 지금 이 순간 당장 최적의 답을 선택해 결과를 도출하자라는 마인드가 중요하다.
- 하지만 종합적으로 가장 최적의 답이 아닐수도 있다.
- 사실 이 유형의 문제는 문제에 대한 이해와 코딩 피지컬(코드 구현 속도)이 중요하지 특이한 방법이 있는 것은 아니다.

# 구현
- 코딩 피지컬을 가장 요하는 문제로 자신이 생각한것을 코드로 짤수 있어야한다.
- 필요한 지표를 list를 사용해 사전에 정의하는것을 고려해봐야한다.(ex.채스 문제)

# DFS. BFS
- 깊이 우선 탐색(DFS), 너비 우선 탐색(BFS)
- DFS의 경우에는 재귀함수나 자료구조 스택을 이용하고 모든 경우의수를 다 알아봐야하는경우에 사용 
- BFS의 경우에는 큐를 사용하고 시작점에서 가장 짧은 경로의 끝점을 찾는대 유리

# 정렬
- 선택 정렬
간단하게 첫 원소 부터 선택해서 그 이후 원소들과 비교해 가장 작은 값을 넣는다. 이중 for문을 사용함으로 O(N^2)
- 삽입 정렬
두번째요소 부터 기준 값보다 왼쪽 값들과 비교해 기준값이 더 작으면 교체 아니라면 다음 요소를 기준값으로 잡는다.
이미 정렬이 대부분 되어있을때 굉장히 빠른 정렬 하지만 결국 시간 복잡도는 O(N^2)
- 퀵 정렬
첫번째 원소를 pivot값으로 잡고 그 값보다 작으면 왼쪽 크면 오른쪽 리스트에 넣고 각각의 리스트를 다시 같은 방식으로 정렬해 리스트들을 합친다.
재귀함수를 이용하고 시간복잡도는 O(NlogN)이다.
- 계수 정렬 
새로운 리스트를 생성해 그 리스트의 인덱스를 정렬하고픈 요소들의 값으로 생각하고 리스트에서 값이 등장할때마다 +1 해준다.
이후 for문을 이용해 표현한다.

# 탐색
- 완전탐색
니가 떠올린 그 탐색
- 이진 탐색
시작 값, 끝 값, 중간값을 설정해 원하는 값과 중간값을 비교해 다시 시작 값과 끝 값을 정의해주는 방식으로 탐색
꽤 빠르고 시간 초과가 나거나 주어진 데이터들이 너무 크다면 활용을 고려!

# 동적 프로그래밍
- 어떤 규칙 내에서 원하는 값을 구하기 위해선 그 값을 구성하고있는 값 역시도 같은 규칙에 적용되어 분석해야할때 쓰임
- 쉽게 수열의 점화식을 생성가능한지 생각해보면 됨

# 최단 경로
- 최단 경로 알고리즘은 말 그대로 가장 짧은 경로를 찾는 알고리즘이다.
- 다익스트라 최단 경로
시작 노드에 대해 나머지 노드까지의 최단 경로를 구함 힙을 이용해 시간 복잡도를 줄임 
https://namu.wiki/w/%EB%8B%A4%EC%9D%B5%EC%8A%A4%ED%8A%B8%EB%9D%BC%20%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98
- 플로이드 워셜 알고리즘
가능한 모든 노드쌍들에대한 최단 경로를 모두 구하는 알고리즘 3중첩반복문 사용 시작 노드 a 와 끝 노드 b에 대해 지나가는 노드 k중 최단 경로에 포함되는 지 반복문을 이용해 구함
https://namu.wiki/w/%ED%94%8C%EB%A1%9C%EC%9D%B4%EB%93%9C-%EC%9B%8C%EC%85%9C%20%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98

# 참고서적
- 이것이 취업을 위한 코딩 테스트다 with 파이썬
- 파이썬 자료구조와 알고리즘
