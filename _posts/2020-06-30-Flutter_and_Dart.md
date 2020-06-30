---
title: "Git 정리"
date: 2020-06-29
categories: jekyll update
---

**Flutter 기본 명령어**
-Scaffold: 배경을 하얗게 만들 때 사용
-AppBar: 상단에 앱 바 생성
-StatelessWidget: 화면이 변하지 않는 경우에 적용
-StatefulWidget: 상태를 가지는 위젯(화면이 변하는)
-그 외 column, row, padding 등 있는데 직접 홈페이지에서 design 찾아보면서 하는게 좋을 듯.


**Dart 문법 정리**
-기본 문법은 자바, c와 매우 비슷함
-변수 선언시 기존 int, double, string 등 사용 가능하지만 통합시켜 var로도 선언이 가능
-마찬가지로 dynamic으로도 선언이 가능하다
 ->주로 함수에서 parameter로 사용하며 이 경우 어떤 변수든 사용 가능하다
 ->자바에서 object와 매우 유사
-마찬가지로 숫자의 경우 num으로 int와 double 모두 사용 가능하다
-final, const는 자바와 마찬가지로 따로 선언하지 않아도 사용 가능
-모든 변수는 선언시 public, 변수 이름 앞에 언더바(_)를 붙이면 private

-List<변수타입> 이름 = []: 자바와 비슷하게 리스트, 즉 array도 가능
-마찬가지로 List<변수타입> 부분을 var로 변경하면 어떤 변수든 사용 가능
-리스트 내에 ...리스트이름을 추가하면 이어서 사용할 수 있다
 ->예) var items = [1, 2, 3];
       var items2 = [...items, 4, 5];
   items2 출력 => 1, 2, 3, 4, 5

-함수 파라미터 안 변수에 중괄호를 씌우면 옵션 처리한다(13:50)
 ->여러개의 변수를 파라미터로 지정해도 함수 call시 모두 부르지 않아도 된다는 말

-타입 비교: == 대신 is 사용
 ->예) if(a is int) / if(a is! int)
-a가 정수, b가 실수일 때 자바에서처럼 타입 캐스팅(b = a)가 안됨. as를 사용할 것 
 ->b = a as double;
-if 대신 ??도 사용 가능
 ->예) var name;
       print(name ?? ‘널’);    ---> null일 때 ‘널’을 프린트한다


-클래스: 사용 방법은 자바와 동일. 다만 new는 옵션.
-getter, setter 없이 사용 가능(generate 메뉴에 있음)
-interface 문법 없음

-Stream: StreamController (var로도 대체 가능) (36:00)
