## ArrayList vs LinkedList
---
### Dynamic Array (ArrayList)
- 크기가 가변적으로 변하는 선형 리스트 (C++에서는 Vector, Java에서는 ArrayList)
- 내부적으로 순차적 메모리 할당하는 배열을 이용해서 리스트 구현한 것
- Java 기준, 배열보다 느릴수 있으나 사용에 용이함
- 데이터 크기가 변하면 2배 크기의 공간을 찾아 할당, 데이터 복사하고 이전 메모리 지워버림
* 장점  
  내부적으로 배열과 같기 때문에 인덱스 이용한 접근이 빠르다.
* 단점  
  데이터 삽입/삭제가 느리다.  
  (배열과 마찬가지로 뒤의 요소 모두 밀어내고 삽입, 삭제 후 뒤 요소 모두 당겨와야하기 때문에)

### LinkedList
- 앞서 정리했던것 과 마찬가지로 각 노드가 이전노드와 다음 노드 상태를 알고있어야 한다.
- 데이터 검색, 접근시 처음부터 노드를 순회하기때문에 성능상 좋지 않다.
- 데이터의 삽입과 삭제는 비교적 빠르다.  
  
---

### 정리 표
operation|LinkedList 시간복잡도|ArrayList 시간복잡도|preferred|  
---|---|---|---|  
마지막에 삽입|O(1)|O(1)|LinkedList  
주어진 인덱스에 삽입|O(N)|O(N)|LinkedList  
값으로 검색|O(N)|O(N)|ArrayList  
인덱스로 검색|O(N)|O(1)|ArrayList  
값 삭제|O(N)|O(N)|LinkedList|  
인덱스로 삭제|O(N)|O(N)|LinkedList|  