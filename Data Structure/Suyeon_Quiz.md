# 📁 자료구조

## 1. 비선형 구조에 대해 설명해주세요. 
<details>
<summary>1번 정답</summary>
<div markdown="1">      
<strong><em>하나의 자료 뒤(안)에 여러개의 자료가 존재할 수 있는 형태</em></strong>입니다.<br>
1:N 또는 N:N 관계를 가집니다.<br>
대표적으로 트리, 그래프가 있습니다.<br>
<a href="https://jud00.tistory.com/entry/Data-Structure-%EC%84%A0%ED%98%95Linear-%EB%B9%84%EC%84%A0%ED%98%95NonLinear-%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0">참고1</a>
</div>
</details>
<hr>

## 2. 트리와 그래프의 차이를 말해주세요.
<details>
<summary>2번 정답</summary>
<div markdown="1">      
트리는 사이클이 존재할 수 없지만 그래프는 사이클이 존재합니다.<br>
트리는 부모-자식 관계를 가지지만 그래프는 부모-자식 관계라는 개념이 없다.<br>
<a href="https://github.com/gyoogle/tech-interview-for-developer/blob/master/Computer%20Science/Data%20Structure/Tree.md">참고1</a>
<a href="https://velog.io/@jeewoo1025/%ED%8A%B8%EB%A6%AC-Tree">참고2</a>
</div>
</details>
<hr>

## 3. 트리 순회 방식 4가지에 대해 말해주세요.
<details>
<summary>3번 정답</summary>
<div markdown="1">      
1. 전위 순회는 각 루트를 순차적으로 먼저 방문하는 방식(Root -> 왼쪽 자식 -> 오른쪽 자식)입니다.<br>
2. 중위 순회는 왼쪽 하위 트리를 방문 후 루트를 방문하는 방식(왼쪽 자식 -> Root -> 오른쪽 자식)입니다.<br>
3. 후위 순위는 왼쪽 하위 트리부터 하위를 모두 방문 후 루트를 방문하는 방식(왼쪽 자식 -> 오르쪽 자식 -> Root)입니다.<br>
4. 레벨 순회는 루트부터 계층별로 방문하는 방식입니다.<br>
<a href="https://github.com/gyoogle/tech-interview-for-developer/blob/master/Computer%20Science/Data%20Structure/Tree.md">참고1</a>
</div>
</details>
<hr>

## 4. 이진 트리(Binary Tree)와 이진 탐색 트리(BST)에 대해 설명해주세요. 
<details>
<summary>4번 정답</summary>
<div markdown="1">      
이진 트리는 자식 노드가 최대 두개인 노드로 구성된 트리입니다.<br>
이진 탐색 트리는 이진 탐색과 연결 리스트 합쳐진 구조입니다.<br>
 <strong><em>즉, 이진 탐색 트리는 이진 탐색과 연결 리스트를 결합한 자료구조로
이진 탐색의 효율적 탐색 능력을 유지하면서, 빈번한 자료 입력과 삭제가 가능하다는 장점을 가지고 있습니다.</em></strong><br>
<a href="https://github.com/gyoogle/tech-interview-for-developer/blob/master/Computer%20Science/Data%20Structure/Binary%20Search%20Tree.md">참고1</a>
<a href="https://dev-coco.tistory.com/159">참고2</a>
</div>
</details>
<hr>

## 5. 이진 탐색 트리의 특징과 시간 복잡도에 대해 설명해주세요. 
<details>
<summary>5번 정답</summary>
<div markdown="1">      
특징<br>
- 각 노드의 자식이 2개 이하<br>
- 각 노드의 왼쪽 자식은 부모보다 작고, 오른쪽 자식은 부모보다 큼<br>
- 중복된 노드가 없어야 함<br>
시간복잡도<br>
- 균등 트리 : 노드 개수가 N개일 때 O(logN)<br>
- 편항 트리 : 노드 개수가 N개일 때 O(N)<br>
이진 탐색 트리의 연산(검색, 삽입, 삭제)은 결국 트리를 순회하며 타겟 데이터의 위치를 찾는 연산이 공통적으로 필요하므로, <strong><em>트리의 높이에 비례하여 시간 복잡도가 증가</em></strong><br>
<a href="https://velog.io/@haero_kim/%EC%9D%B4%EC%A7%84-%ED%83%90%EC%83%89-%ED%8A%B8%EB%A6%AC-Binary-Search-Tree">참고1</a>
<a href="https://github.com/gyoogle/tech-interview-for-developer/blob/master/Computer%20Science/Data%20Structure/Binary%20Search%20Tree.md">참고2</a>
</div>
</details>
<hr>


## 6. 이진 탐색 트리의 최악의 경우의 예에 대해 설명해주세요. 
<details>
<summary>6번 정답</summary>
<div markdown="1">      
예를들어 1부터 10까지 순차적으로 BST에 저장했다면, BST의 형태는 리스트와 같아집니다.<br>
즉 오른쪽이나 왼쪽 자식노드로 쭉 이어어지는 극단적인 경우(편향 트리)를 최악의 경우라고 하며 시간복잡도는 O(n)입니다.<br>
<a href="https://github.com/ksundong/backend-interview-question#CS-%EA%B4%80%EB%A0%A8-%EC%A7%80%EC%8B%9D">참고1</a>
<a href="https://velog.io/@cchloe2311/%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0-%EC%9D%B4%EC%A7%84%ED%83%90%EC%83%89%ED%8A%B8%EB%A6%AC-Binary-Search-Tree-BST">참고2</a>
</div>
</details>
<hr>

## 7. 트라이에 대해 설명해주세요. 
<details>
<summary>7번 정답</summary>
<div markdown="1">      
<strong><em>문자열을 저장하고 효율적으로 탐색하기 위한 트리 형태의 자료 구조</em></strong><br>
자동완성 기능, 사전 검색 등 문자열을 탐색하는데 특화되어 있는 자료 구조<br>
장점<br>
- 문자열 검색이 빠름<br>
- 문자열을 탐색할 때, 하나하나씩 전부 비교하면서 탐색을 하는 것보다 시간 복잡도 측면에서 효율적<br>
단점<br>
- 각 노드에서 자식들에 대한 포인터들을 배열로 모두 저장하고 있다는 점에서 저장 공간의 크기가 큼(메모리 측면에서 비효율적)<br>
<a href="https://velog.io/@kimdukbae/%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0-%ED%8A%B8%EB%9D%BC%EC%9D%B4-Trie">참고1</a>
<a href="https://rebro.kr/86">참고2</a>
</div>
</details>
<hr>

## 8. 그래프를 구현하는 두 가지 방법에 대해 말해주세요. 
<details>
<summary>8번 정답</summary>
<div markdown="1">      
정방 행렬(배열)을 사용하는 방법(인접 행렬)과 연결 리스트를 사용하는 방법(인접 리스트)이 있습니다.<br>
인접 행렬의 장단점<br>
- 두 정점을 연결하는 간선의 존재 여부를 O(1)의 시간 복잡도 내에 알 수 있다.<br>
- 정점의 차수는 O(N)안에 알 수 있다.<br>
- 어떤 노드에 인접한 노드들을 찾기 위해서는 모든 노드들을 순회해야 한다.<br>
- 그래프에 존재하는 모든 간선의 수를 파악하는데 O(N^2)의 시간복잡도가 걸린다.(인접행렬 전체 조사)<br>
즉, <strong><em>인접배열을 사용하는 방법은 간선의 개수가 많은 밀집 그래프를 구현하는데 적합</em></strong>하다.<br>
인접 리스트의 장단점<br>
- 특정 정점의 인접 정점들을 쉽게 찾을 수 있다.<br>
- 그래프의 존재하는 모든 간선의 수를 O(N+E)안에 알 수 있다. 이때 간선의 수를 알기 위해 인접리스트 전체를 조사한다.<br>
- 간선의 존재를 파악하기 위해 모든 정점의 리스트에 있는 모든 노드의 수를 확인해야하므로 정점의 연결여부를 파악하는데 많은 시간이 소요된다.<br>
즉, <strong><em>인접리스트를 사용하는 방법은 간선의 개수가 적은 희소 그래프를 구현하는데 적합</em></strong>하다.<br>
<a href="https://github.com/JaeYeopHan/Interview_Question_for_Beginner/tree/master/DataStructure">참고1</a>
<a href="https://velog.io/@alkwen0996/%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0-%EA%B7%B8%EB%9E%98%ED%94%84Graph">참고2</a>
</div>
</details>
<hr>

## 9. 트리가 속해있는 그래프는 무엇인가요? 
<details>
<summary>9번 정답</summary>
<div markdown="1">      
트리는 사이클이 존재하지 않는 방향 그래프(DAG)의 한 종류입니다.<br>
!! 추가자료로 더 공부하기 !!<br>
<a href="https://kangworld.tistory.com/37">참고1</a>
<a href="https://velog.io/@agugu95/%EB%B9%84%EC%88%9C%ED%99%98-%EB%B0%A9%ED%96%A5%EC%84%B1-%EA%B7%B8%EB%9E%98%ED%94%84DAG%EC%99%80-%EC%9C%84%EC%83%81%EC%A0%95%EB%A0%ACTopological-Sortingh">추가자료</a>
</div>
</details>
<hr>

## 10. 퀵 정렬(Quick Sort)에 대해 설명해주세요. 
<details>
<summary>10번 정답</summary>
<div markdown="1">      
퀵 정렬은 빠른 정렬 속도를 자랑하는 분할 정복 알고리즘 중 하나로 피봇을 설정하고 피봇보다 큰 값과 작은 값으로 분할하여 정렬합니다.<br>
시간 복잡도는 O(nlogn)이며 최악의 경우 O(n^2)입니다.<br>
<a href="https://dev-coco.tistory.com/160">참고1</a>
</div>
</details>
<hr>

## 11. 퀵 정렬(Quick Sort)과 병합 정렬(Merge Sort)의 공통점과 차이점에 대해 설명해주세요. 
<details>
<summary>11번 정답</summary>
<div markdown="1">      
공통점<br>
- 분할 정복 알고리즘<br>
- 속도가 빠름<br>
차이점<br>
- 퀵 정렬은 불안정 정렬, 병합 정렬은 안정 정렬<br>
- 퀵 정렬은 최악의 경우 O(n^2)의 시간 복잡도를 가지지만 병합 정렬은 O(nlogn)<br>
- 병합 정렬은 추가 메모리 공간이 필요(임시 배열 필요)<br>
<a href="https://velog.io/@bluejoyq/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%ED%80%B5-%EC%A0%95%EB%A0%ACquick-sort-vs-%EB%B3%91%ED%95%A9-%EC%A0%95%EB%A0%ACmerge-sort">참고1</a>
<a href="https://butter-shower.tistory.com/64">참고2</a>
<a href="https://github.com/VSFe/Tech-Interview/blob/main/01-DATA_STRUCTURE_ALGORITHM.md">참고3</a>
</div>
</details>
<hr>

## 12. 값이 거의 정렬되어 있거나, 아예 정렬되어 있다면 어떤 정렬 알고리즘을 사용하는 것이 좋나요? 
<details>
<summary>12번 정답</summary>
<div markdown="1">      
삽입 정렬<br>
- k번째 원소를 1~k-1번째의 숫자들과 비교해 적절한 위치에 끼워 넣고, 그 뒤의 자료를 한 칸씩 뒤로 밀어내는 방식으로 역순으로 정렬되어 있을 경우에는 시간이 매우 걸린다.<br>
- 반면에 이미 정렬되어 있는 자료구조에는 최고의 정렬 알고리즘이 된다.<br>
<a href="https://bba-dda.tistory.com/98">참고1</a>
<a href="https://github.com/VSFe/Tech-Interview/blob/main/01-DATA_STRUCTURE_ALGORITHM.md">참고2</a>
</div>
</details>
<hr>

## 13. 파이썬에서의 정렬 함수는 무슨 정렬 알고리즘인가요? 
<details>
<summary>13번 정답</summary>
<div markdown="1">      
팀 정렬<br>
- 데이터의 정렬된 정도에 따라 삽입정렬과 병합정렬 사이를 전환하는 적응형 알고리즘<br>
- 추가 메모리는 사용하지만 기존의 병합정렬에 비해 적은 추가 메모리를 사용하여 다른 정렬 알고리즘의 단점을 최대한 극복한 알고리즘<br>
<a href="https://ssungkang.tistory.com/entry/python-%ED%8C%8C%EC%9D%B4%EC%8D%AC%EC%9D%98-%EC%A0%95%EB%A0%AC-Tim-Sort">참고1</a>
<a href="https://d2.naver.com/helloworld/0315536">추가자료</a>
</div>
</details>
<hr>

## 공부할 때 참조하면 좋을 사이트
[정렬 알고리즘](https://roytravel.tistory.com/328)
<hr>

## B 트리 / RedBlackTree 관련 문제 추가 예정(아직 이해를 못함ㅜㅜ..)



