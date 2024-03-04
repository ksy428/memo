
## Spring Security
- deprecated and marked for removal

  - Spring Security 6.1.0부터는 메서드 체이닝의 사용을 지양하고 람다식을 통해 함수형으로 설정하게 지향

- passwordEncoder.matches

  - 평문 비밀번호와 암호화된 비밀번호 비교함

-  Cors문제(Spring Security <-> React)


            public class WebSecurityConfig implements WebMvcConfigurer {
                public void addCorsMappings(CorsRegistry registry) {
                    registry.addMapping("/**")
                            .allowedOriginPatterns("*")
                            .allowedMethods("*")
                            .allowedHeaders("*")
                            .allowCredentials(true);
                }
            }
React

요청
            withCredentials = true;
