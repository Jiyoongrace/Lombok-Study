# Lombok-Study

1. Lombok

- 자바 코드 다이어트 라이브러리
- VO 작성 시 반복적인 getter, setter, 생성자, toString 재정의 같은 작업을 수행하게 되는데 이 작업을 조금 더 쉽게 할 수 있도록 도와준다.
- 코드 상에서는 당연히 Lombok의 annotation을 이용해서 처리하고, 컴파일되면 class 내에 해당 getter나 setter 등이 포함되는 구조

2. Lombok Annotation

2.1 @Getter, @Setter

- getter, setter를 자동으로 만들어준다.

2.2 @NoArgsConstructor

- 인자를 가지지 않는 생성자를 자동으로 만들어준다.
        - default 생성자

2.3 @AllArgsConstructor

- 모든 private field를 인자로 가지는 생성자를 자동으로 만들어준다.

2.4 @RequiredArgsConstructor

- 생성자에 포함되는 인자를 내가 결정해서 생성자를 자동으로 만들어준다. @NonNull 이용

2.5 @ToString

- 객체의 내용을 문자열로 표현하기 위해 우리는 toString method를 overriding해서 사용하는데 이걸 자동으로 만들어준다.
- 이들 외에도 여러 가지 Annotation이 제공된다.

2.6 @Data

- @Setter, @Getter, @RequiredArgsConstructor, @ToString을 포함하고 있는 Annotation
- 사용하지 않는 여러 생성자나 toString이 같이 포함될 수 있기 때문에 자원의 낭비(class 크기가 상대적으로 커진다.)가 발생할 여지가 있다. 그래서 이를 꺼려 하는 사용자도 있다.
