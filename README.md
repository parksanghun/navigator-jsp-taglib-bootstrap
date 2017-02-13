# 페이징 테그 라이브러리 부트스트랩 적용

부트스트랩을 적용해서 페이징 테크라이브러리를 만듬

```html

<%@ taglib prefix="navi" uri="http://github.com/sejoung/navigator-jsp-taglib-bootstrap" %>

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">

<navi:navigator currentPage="1" countPerPage="2" pagePerBlock="10" totalRecordCount="3" />

```
maven pom.xml에 추가

```xml
	    <!-- 페이징 라이브러리 추가 -->
	  <dependency>
			<groupId>com.github.sejoung</groupId>
			<artifactId>navigator</artifactId>
			<version>1.0</version>
		</dependency>
```

currentPage : 현재페이지 번호 (0부터 시작)

countPerPage : 페이지에 보이는 리스트 갯수

pagePerBlock : 페이징에서 보이는 갯수

totalRecordCount : 전체 카운트

