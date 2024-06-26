# 일반적인 컬렉션

러스트의 표준 라이브러리에는 *컬렉션 (collection)* 이라 불리는 매우 유용한 데이터
구조들이 여러 개 포함되어 있습니다. 대부분의 다른 데이터 타입은 단일한 특정 값을
나타내지만, 컬렉션은 다수의 값을 담을 수 있습니다. 내장된 배열 (build-in array) 이나
튜플 타입과는 달리, 이 컬렉션들이 가리키고 있는 데이터들은 힙에 저장되는데, 이는
즉 데이터의 양이 컴파일 타임에 결정되지 않아도 되며 프로그램 실행 중에 늘어나거나
줄어들 수 있다는 의미입니다. 각 컬렉션 종류는 서로 다른 크기와 비용을 가지고
있으며, 현재의 상황에 따라 적절한 컬렉션을 선택하는 것은 장시간에 걸쳐
발전시켜야 하는 기술입니다. 이번 장에서는 러스트 프로그램에서 굉장히 자주
사용되는 세 가지 컬렉션에 대해 다뤄보겠습니다:

* *벡터 (vector)* 는 여러 개의 값을 서로 붙어 있게 저장할 수 있도록 해줍니다.
* *문자열 (string)* 은 문자 (character) 의 모음입니다. `String` 타입은 전에도
  다루었지만, 이번 장에서 더 깊이 있게 이야기해 보겠습니다.
* *해시맵 (hash map)* 은 어떤 값을 특정한 키와 연관지어 주도록 해줍니다. 이는
  *맵 (map)* 이라 일컫는 좀 더 일반적인 데이터 구조의 특정한 구현 형태입니다.

표준 라이브러리가 제공하는 다른 컬렉션에 대해 알고 싶으시면,
[문서][collections]를 봐주세요.

이제부터 벡터, 문자열, 해시맵을 만들고 업데이트하는 방법 뿐만 아니라 
무엇이 각 컬렉션을 특별하게 해주는 지에 대해 논의해 보겠습니다.

[collections]: https://doc.rust-lang.org/std/collections/index.html
