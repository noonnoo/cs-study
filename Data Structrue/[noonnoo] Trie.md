### Trie (트라이)
- 일반 트리 자료구조 중 하나로, Digital Tree, Prefix Tree라고도 불림  
- m-way 탐색트리 (m개만큼의 자식노드를 가질 수 있는 탐색 트리, B트리도 여기 포함)
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/be/Trie_example.svg/500px-Trie_example.svg.png" width=400px alt="이미지 출처: wikipedia"/>

* Trie 특성
  - 각 노드는 <key, value> map 형태로 
    - key는 하나의 알파벳, value는 key에 해당하는 자식노드 형태이다  
  - 루트노드는 특정 문자를 의미하지 않고 자식노드만 가진다 
  - 루트노드를 제외한 노드의 자손들은 해당 노드와 공통 접두어를 가진다

* Trie 활용
- 텍스트 자동완성 기능 같이 문자열 저장/탐색에 유용
- 키 집합으로 하위노드가 정렬된 트라이를 만들면 집합 전체를 사전순으로 정렬할 수 있음
- 트라이의 특수한 형태인 접미사 트리(suffix tree)는 빠른 전문(全文)검색에 활용됨

### 참고) Radix Tree(trie)
- Radix tree: 모든 노드에 데이터가 포함된다
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Patricia_trie.svg/700px-Patricia_trie.svg.png" width=400px alt="이미지 출처: wikipedia"/>

- Radix trie: 리프노드에만 데이터가 포함된다 (Radix tree보다 빠르지만 메모리가 더 필요)  
  
  
### 참고  
- https://brunch.co.kr/@springboot/75  
- https://github.com/WooVictory/Ready-For-Tech-Interview/blob/master/Data%20Structure/Trie(트라이).md  
- https://ko.wikipedia.org/wiki/트라이_(컴퓨팅)  