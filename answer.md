1. 관계형 데이터베이스(RDBMS)와 비관계형 데이터베이스(NoSQL)의 장단점 비교

- 관계형 데이터베이스는 2차원 표를 통해 나타낼 수 있어 이해하기 쉽다.
- 관계형 데이터베이스는 정규화를 통해 중복을 감소시킬 수 있다.
- 관계형 데이터베이스는 데이터 무결성 적용을 통해 데이터의 정확성과 안정성을 보장하여, 대규모 데이터 관리에 용이하다.
- 관계형 데이터베이스는 사전에 스키마를 정의해야 하기 때문에 변경이 잦은 데이터에는 부적합하다.
- 관계형 데이터베이스는 스케일 업을 통해 성능을 개선하기 때문에 비용이 많이 소모된다.

- 비관계형 데이터베이스는 유연한 스키마를 제공하여 상대적으로 빠른 개발을 가능하게 하며, 다양한 형식의 데이터를 처리할 수 있다.
- 비관계형 데이터베이스는 스케일 아웃이 가능하여 비용을 낮추면서 확장이 가능하다.
- 비관계형 데이터베이스는 'join'이 없기 때문에 상대적으로 쿼리의 속도가 빠르다.
- 비관계형 데이터베이스는 ACID가 아닌 BASE를 기반으로 하기 때문에 상대적으로 유효성이 떨어진다.

2. 트랜잭션(transaction)이란 무엇인가요?

- 트랜잭션이란 데이터베이스와 관련하여 수행되는 작업 단위로서 하나 이상의 쿼리문을 말한다.
- 트랜잭션은 안정성 보장을 위해 트랜잭션이 모두 성공하거나, 모두 실패하는 원자성을 갖는다.
- 트랜잭션은 데이터베이스의 제약을 만족시켜야 하기 때문에, 트랜잭션 이전/이후의 상태가 모두 유효하게 되는 일관성을 갖는다.
- 트랜잭션은 둘 이상의 트랜잭션이 수행될 때 각 트랜잭션이 독립적으로 처리되는 독립성을 갖는다.
- 트랜잭션은 트랜잭션 완료 후에 변경사항을 영구적으로 갖는 지속성을 갖는다.

3. MySQL에서 조인(join)의 역할은 무엇인가요? 다양한 join의 방식에 대해 설명해주세요.

- 조인이란 두 개 이상의 테이블에서 연관된 열을 이용하여, 레코드를 합치는 것을 말한다.
- Inner join은 기준 테이블과 합치려는 테이블 모두에 결합조건이 매칭되는 열만 검색하는 방법이다.
- Left join은 기준 테이블의 모든 열과 합치려는 테이블 중 조건이 매칭되는 열만 검색 후 매칭되지 않는 열에는 null 값을 표시하는 방법이다.
- Right join은 합치려는 테이블의 모든 열과 기준 테이블에서 매칭되는 열만 검색하고 매칭되지 않는 열에는 null 값을 표시하는 방법이다.
- UNION을 사용하여 left, right join을 합쳐서 테이블 두 개를 통째로 합칠 수도 있다.

4. MySQL에서 인덱스(index)란 무엇인가요?

- 인덱스란 주어진 쿼리에서 테이블의 모든 열을 검색하지 않고도 데이터의 위치를 찾는데 사용되는 자료구조이다.
- 인덱스는 쿼리의 성능을 향상시키며, 만약 인덱스가 없다면 데이터를 찾기 위해 테이블 전체를 검색해야 할 것이다.
