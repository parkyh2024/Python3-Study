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

[출처] https://blog.naver.com/newbongman/222987762797

[내용출처] https://blog.naver.com/bbbisskk2/222966159315

---

 ### BFS (너비우선탐색)
 
 하나의 노드에서 시작하며 시작점과 가까운 지점부터 줄기별로 탐색
 
 ![이미지](https://postfiles.pstatic.net/MjAyMzAxMThfMTUg/MDAxNjc0MDEzODcwODM4.b8y8kLMcxCkFGf6mJ3XwRFwiL7I6CGVHYMziG_e-RH8g.pZHtsy_0t75nQnA7ENX9Q_x0SVvr1tMqqhdjhn5xj8wg.GIF.newbongman/BFS_ani_images_lucky-korma_post_2112183b-bfcd-427e-8072-c9dc983180ba_R1280x0.gif?type=w580)
 
 [이미지출처] https://blog.naver.com/newbongman/222987762797
 
 위의 그림과 같이 노드 0부터 시작하는데 시작점과 인접한 노드 1,2,3을 먼저 싹 확인한 후 다음 노드로 진행된다

BFS는 Queue(FIFO)의 자료구조 방식을 사용한다

노드 0부터 시작해보자

빈 리스트에 0을 넣고 [0] 인접한 노드 1,2,3을 차례로 삽입한다

[0,1,2,3]그리고 인접한 노드가 없으므로 0을 꺼낸다. [1,2,3] 그리고 제일 먼저 들어왔었던(선입) 1을 확인 해 1의 인접한 노드인 4를 넣는다

이후 인접 노드가 없으므로 1을 출력한다(선출)

BFS는 이런식으로 선입선출 방식인 queue를 활용하는 것이다

[내용출처] https://blog.naver.com/bbbisskk2/222966159315
 
