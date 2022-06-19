# jpa_basic
jpabasic


좀 더 복잡한 쿼리가 있을때 JPQL OR QueryDSL 둘중 하나를 고민하게 된다.
## Query DSL?
  쿼리를 자바코드로 작성할 수 있도록 도와주는 기술(JAVA코드를 활용해서 작성)
  자바로 작성하기 때문에 컴파일 시점에 문법 오류를 확인
  
## JPQL(Java Persistence Query Language)
  JPA에서 엔티티 객체를 대상으로 쿼리하는 언어(String으로 입력해서 작성)
  SQL문과 비슷하지만 SQL은 데이터베이스 테이블을 대상으로, JPQL은 엔티티 객체를 대상으로 쿼리
  STRING으로 작성하기 때문에 문법 오류 파악이 어려움
  
## Query DSL VS JPQL
  결과적으로 Querydsl로 작성한 코드는 JPQL이 된다. 
  
 Join, 동적쿼리를 작성하려면 QueryDSL, 정말 단순한 쿼리 JPQL(@Query 애노테이션 활용?) 
