# DFS, BFS

 DFS(깊이우선탐색), BFS(너비우선탐색) 두 개 모두 그래프를 탐색하는 방법들이다
 
 그래프란 정점(node)과 연결선(edge)으로 이뤄진 자료구조의 일종을 말하며
 
 그래프를 탐색한다는 것은 하나의 정점으로부터 시작하여 차례대로 모든 정점들을 한 번씩 방문하는 것을 한다
 
  [출처] https://blog.naver.com/newbongman/222987762797
 
 ---
 
 ### DFS (깊이우선탐색)
 
 하나의 노드에서 시작하 분기끝까지 탐색 반복
 
![이미지](https://postfiles.pstatic.net/MjAyMzAxMThfMTY2/MDAxNjc0MDEzNzg2MzY3.wzOFOwqTgKt0Ldd0aFlGPmy-vbFMd-s34yCQo3mWiG0g.BS6n4lgIGBW4FA-DSj7k1GxD37h-Z9hUz2G7DsG9iVAg.GIF.newbongman/DFS_ani_images_lucky-korma_post_30737a15-9adf-49a6-96a0-98c211cab1cc_R1280x0.gif?type=w580)

[이미지출처] https://blog.naver.com/newbongman/222987762797

루트 노드(혹은 다른 임의의 노드)에서 시작해서 다음 분기로 넘어가기 전에 해당 분기를 완벽하게 탐색하는 방식을 말한다

예를 들어 미로찾기를 할 때 최대한 한 방향으로 갈 수 있을 때까지 쭉 가다가 더 이상 갈 수 없게 되면

다시 가장 가까운 갈림길로 돌아와서 그 갈림길부터 다시 다른 방향으로 탐색을 진행하는 것이 깊이 우선 탐색 방식이라고 할 수 있다

이 과정을 토대로 선입후출 방식인 Stack을 사용해야 하는 것이다

1. 모든 노드를 방문하고자 하는 경우에 이 방법을 선택함

2. 깊이 우선 탐색(DFS)이 너비 우선 탐색(BFS)보다 좀 더 간단함

3. 검색 속도 자체는 너비 우선 탐색(BFS)에 비해서 느림

[내용출처] https://blog.naver.com/newbongman/222987762797

---

 ### BFS (너비우선탐색)
 
 하나의 노드에서 시작하며 시작점과 가까운 지점부터 줄기별로 탐색
 
 ![이미지](https://postfiles.pstatic.net/MjAyMzAxMThfMTUg/MDAxNjc0MDEzODcwODM4.b8y8kLMcxCkFGf6mJ3XwRFwiL7I6CGVHYMziG_e-RH8g.pZHtsy_0t75nQnA7ENX9Q_x0SVvr1tMqqhdjhn5xj8wg.GIF.newbongman/BFS_ani_images_lucky-korma_post_2112183b-bfcd-427e-8072-c9dc983180ba_R1280x0.gif?type=w580)
 
 [이미지출처] https://blog.naver.com/newbongman/222987762797
 
루트 노드(혹은 다른 임의의 노드)에서 시작해서 인접한 노드를 먼저 탐색하는 방법으로

시작 정점으로부터 가까운 정점을 먼저 방문하고 멀리 떨어져 있는 정점을 나중에 방문하는 순회 방법이다

주로 두 노드 사이의 최단 경로를 찾고 싶을 때 이 방법을 선택한다

ex) 지구 상에 존재하는 모든 친구 관계를 그래프로 표현한 후 Sam과 Eddie사이에 존재하는 경로를 찾는 경우

깊이 우선 탐색의 경우 - 모든 친구 관계를 다 살펴봐야 할지도 모름

너비 우선 탐색의 경우 - Sam과 가까운 관계부터 탐색

BFS는 이런식으로 선입선출 방식인 queue를 활용하는 것이다

[내용출처] https://blog.naver.com/newbongman/222987762797
 
---

# DFS, BFS 비교

![이미지](https://postfiles.pstatic.net/MjAyMzAxMThfMTkg/MDAxNjc0MDEzOTI0NDk3.gW44P8-YN7aSSfIAxknMgdn7eqbEQtXRRvEljfXh-B0g.BLSRjcioL0YtuWl--hVp55aCqjsly42iL1op2uRkwEog.GIF.newbongman/DFSvsBFS_ani_images_lucky-korma_post_e2ef7ac3-14e6-42e7-a768-224c5f773e29_R1.gif?type=w580)

 [이미지출처] https://blog.naver.com/newbongman/222987762797
 
 - DFS(깊이우선탐색) : 현재 정점에서 갈 수 있는 점들까지 들어가면서 탐색 - 스택 또는 재귀함수로 구현

 - BFS(너비우선탐색) : 현재 정점에 연결된 가까운 점들부터 탐색 - 큐를 이용해서 구현
 
 [출처] https://blog.naver.com/newbongman/222987762797

---

## 깊이 우선 탐색(DFS)과 너비 우선 탐색(BFS) 활용한 문제 유형/응용

DFS, BFS은 특징에 따라 사용에 더 적합한 문제 유형들이 있다

- 그래프의 모든 정점을 방문하는 것이 주요한 문제

- 단순히 모든 정점을 방문하는 것이 중요한 문제의 경우 DFS, BFS 두 가지 방법 중 어느 것을 사용하셔도 상관없습니다 둘 중 편한 것을 사용하면 됨

- 경로의 특징을 저장해둬야 하는 문제 (예를 들면 각 정점에 숫자가 적혀있고 a부터 b까지 가는 경로를 구하는데 경로에 같은 숫자가 있으면 안 된다는 문제 등, 각각의 경로마다 특징을 저장해둬야 할 때는 DFS를 사용함) (BFS는 경로의 특징을 가지지 못합니다)

- 최단거리 구해야 하는 문제

- 미로 찾기 등 최단거리를 구해야 할 경우, BFS가 유리 (왜냐하면 깊이 우선 탐색으로 경로를 검색할 경우 처음으로 발견되는 해답이 최단거리가 아닐 수 있지만, 너비 우선 탐색으로 현재 노드에서 가까운 곳부터 찾기 때문에경로를 탐색 시 먼저 찾아지는 해답이 곧 최단거리기 때문)

이밖에도

- 검색 대상 그래프가 정말 크다면 DFS를 고려

- 검색대상의 규모가 크지 않고, 검색 시작 지점으로부터 원하는 대상이 별로 멀지 않다면 BFS

[출처] https://blog.naver.com/newbongman/222987762797
