# memo

- Spring Security 6.1.0부터는 메서드 체이닝의 사용을 지양하고 람다식을 통해 함수형으로 설정하게 지향
    http.formLogin((formLogin)-> formLogin.disable())
    ...
