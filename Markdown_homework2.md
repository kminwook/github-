# [공통] 마크다운 markdown 작성법 정보추가 2 (info2)

# 1. 마크다운에 관하여

## 1.1. 마크다운이란?

**마크다운**(markdown) 2004 년 John Gruber 가 만든 Markdown은 이제 세계에서 가장 인기있는 일반 텍스트 기반의 경량 마크업 언어다. 일반 텍스트로 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다. HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README 파일이나 온라인 게시물 등에 많이 사용된다.
마크다운이 최근 각광받기 시작한 이유는 깃헙([https://github.com](https://github.com)) 덕분이다. 깃헙의 저장소Repository에 관한 정보를 기록하는 README.md는 깃헙을 사용하는 사람이라면 누구나 가장 먼저 접하게 되는 마크다운 문서였다. 마크다운을 통해서 설치방법, 소스코드 설명, 이슈 등을 간단하게 기록하고 가독성을 높일 수 있다는 강점이 부각되면서 점점 여러 곳으로 퍼져가게 된다.

## 1.2. 왜 마크다운을 사용할까?

### 1.2.1. 장점

```markdown
1. 배우기가 정말 쉽고 직관적이다.
2. 별도의 도구없이 작성가능하다.
3. 다양한 형태로 변환이 가능하다.
4. 텍스트(Text)로 저장되기 때문에 용량이 적어 보관이 용이하다.
5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
6. 지원하는 프로그램과 플랫폼이 다양하다.
```

### 1.2.2. 단점

```markdown
1. 표준이 없어 도구에 따라서 변환방식이나 생성물이 다르다.
2. 모든 HTML 마크업을 대신하지 못한다.
```

****

# 2. 마크다운 사용법(문법)

## 2.1. 제목(Headings)
* 큰제목: 문서 제목
    ```
    This is an H1
    =============
    ```
    This is an H1
    =============

* 작은제목: 문서 부제목
    ```
    This is an H2
    -------------
    ```
    This is an H2
    -------------
- **주의!**
   - 반드시 # 은 띄어서 쓴다
     ``` 
     #this is an H1 (x) # this is an H1(o)
     ```


* 글머리: 1~6까지만 지원
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
####### This is a H7(지원하지 않음)



## 2.2. 단락
단락을 만들기 위해서는 빈 줄을 사용하해야한다. 
```
* 빈 줄이 없는경우
I really like using Markdown.
I think I'll use it to format all of my documents from now on.

* 빈 줄이 있는경우
I really like using Markdown.

I think I'll use it to format all of my documents from now on.
```
* 빈 줄이 없는경우
  
  I really like using Markdown.
  I think I'll use it to format all of my documents from now on.

* 빈 줄이 있는경우

  I really like using Markdown.

  I think I'll use it to format all of my documents from now on.

## 2.3. 줄 바꿈
3칸 이상 띄어쓰기(` `)를 하면 줄이 바뀐다.

```
* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. 
이렇게

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.___\\ 띄어쓰기
이렇게
```

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. 이렇게

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.    \
이렇게

## 2.4. 중요성(강조)
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```

* *single asterisks*
* _single underscores_
* **double asterisks**
* __double underscores__
* ~~cancelline~~

> ```문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.```   
> 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.


## 2.5. 인용구
사용하려는 단락앞에 >를 추가하면 인용구가 만들어진다.
```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> Dorothy followed her through many of the beautiful rooms in her castle.
``` 
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> Dorothy followed her through many of the beautiful rooms in her castle.

## 2.6. 목록(list)
### ● 순서있는 목록(번호)

  목록은 번호 1로 시작되어야 한다.

순서있는 목록은 숫자와 점을 사용한다.
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

**현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.**
```
1. 첫번째
3. 세번째
2. 두번째
```
1. 첫번째
3. 세번째
2. 두번째


### ● 순서없는 목록(글머리 기호: `*`, `+`, `-` 지원)
```
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
```
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

혼합해서 사용하는 것도 가능하다

```
* 1단계
  - 2단계
    + 3단계
      + 4단계
```

* 1단계
  - 2단계
    + 3단계
      + 4단계


## 2.7. code(')
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.

### 2.7.1. 들여쓰기
```
This is a normal paragraph:

    This is a code block.
    
end code block.
```

실제로 적용해보면,

적용예:

*****
This is a normal paragraph:

    This is a code block.

end code block.
*****

> 한줄 띄어쓰지 않으면 인식이 제대로 안되는 문제가 발생합니다.

```
This is a normal paragraph:
    This is a code block.
end code block.
```

적용예:

*****
This is a normal paragraph:
    This is a code block.
end code block.
*****

### 2.7.2. 코드블럭
코드블럭은 다음과 같이 2가지 방식을 사용할 수 있습니다:

* `<pre><code>{code}</code></pre>` 이용방식

```
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>
```

<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
</code>
</pre>

* 코드블럭코드("\```") 을 이용하는 방법

<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

**깃헙**에서는 코드블럭코드("\```") 시작점에 사용하는 언어를 선언하여 [문법강조(Syntax highlighting)](https://docs.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks#syntax-highlighting)이 가능하다.

<pre>
<code>
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```


## 2.8. Horizontal Rules
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 *페이지 나누기* 용도로 많이 사용한다.

```
* * *

***

*****

- - -

---------------------------------------
```

* 적용예
* * *

***

*****

- - -

---------------------------------------


## 2.9. Links
* 참조링크

```
[link keyword][id]

[id]: URL "Optional Title here"

// code
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
```

Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

* 외부링크
```
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
```
Link: [Google](https://google.com, "google link")

* 자동연결
```
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

## 2.10. 이미지
```
![Alt text](https://mblogthumb-phinf.pstatic.net/20141113_147/nsi_blog_1415805988740N8Y7e_PNG/%B7%AF%B9%F6%B4%F6.png?type=w2)
![Alt text](https://mblogthumb-phinf.pstatic.net/20141113_147/nsi_blog_1415805988740N8Y7e_PNG/%B7%AF%B9%F6%B4%F6.png?type=w2 "Optional title")
```
![석촌호수 러버덕](https://mblogthumb-phinf.pstatic.net/20141113_147/nsi_blog_1415805988740N8Y7e_PNG/%B7%AF%B9%F6%B4%F6.png?type=w2)
![석촌호수 러버덕](https://mblogthumb-phinf.pstatic.net/20141113_147/nsi_blog_1415805988740N8Y7e_PNG/%B7%AF%B9%F6%B4%F6.png?type=w2 "RubberDuck")

사이즈 조절 기능은 없기 때문에 ```<img width="" height=""></img>```를 이용한다.

## 2.11. Escaping Characters
문자 \앞에 백 슬래시를 추가하면 Escaping Characters로 표시된다.
```
\* Without the backslash, this would be a bullet in an unordered list.
```
\* Without the backslash, this would be a bullet in an unordered list.


## 2.12. HTML
많은 Markdown 응용 프로그램을 사용하면 Markdown 형식의 텍스트에서 HTML 태그를 사용할 수 있습니다. Markdown 구문보다 특정 HTML 태그를 선호하는 경우 유용합니다. 예를 들어 어떤 사람들은 이미지에 HTML 태그를 사용하는 것이 더 쉽다고 생각합니다. HTML을 사용하면 텍스트 색상 지정 또는 이미지 너비 변경과 같이 요소의 속성을 변경해야 할 때도 유용합니다.

HTML을 사용하려면 마크 다운 형식 파일의 텍스트에 태그를 배치하십시오.

```html
This **word** is bold. This <em>word</em> is italic.
```
This **word** is bold. This <em>word</em> is italic.


[github readme.md](https://github.com/kminwook/-)