# 자바8 새로운 기술 써보기

1. Objects.equals(obj,obj)
이 메소드를 사용하면 null일지도 모르는 두 오브젝트의 값을 비교 할 수 있다.

사용계기: 
2개의 HashMap 값 비교
HashMap안에는 null 가능성 있음
get메소드를 사용하면 null exception

선언시 메소드 에러나는 경우는
파일 가장 위에 util.Objects 추가 후 메소드 작성

2. Stream().filter사용해보기
List<HashMap<String,Object>> lines
List<HashMap<String,Object>> colors

List<HashMap<String,Object>> results = lines.streams(). filter(i -> (String)i.get("shhn_cd").equals(colors.get(0).get("shhn_cd")))

