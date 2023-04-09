:kr:
웹이나 깃허브에서 문서를 읽기 쉽게 표현하기 위한 방법

출처: `https://guides.github.com/features/mastering-markdown/`

---
**표식하기 문서편집기** (앱, 프로그램)

| 상징 | 편집기 이름 | 단점, 장점 |  
| :---: | ---        | --- |  
| ![비스-코드](./images/ico_vs-code_50x50.png) | 코드(Code) | 완벽한 한글지원, 가볍다, 빠르다, 지금까지 가장 좋음(2019.02.16) |  
| | | `https://code.visualstudio.com` |  
| ![아톰](./images/ico_Atom_50x50.png) | 아톰(Atom)  | 한글지원 안됨, 사용법이 복잡함, 깃허브 보기와 가장 비슷함, 사용중 점점 둔해짐 |  
| | | `https://github.com/atom/atom.io` |  
| ![노트패드](./images/ic_-Notepad-pp_50x50.png) | Notepad++ |  삽입그림 표시안됨 |  
| | | `https://notepad-plus-plus.org` |  
| ![MarkdownPad2](./images/ico_markdownpad2_50x50.png) | MarkdownPad2 | 삽입그림 표시안됨 |  
| | | `https://markdownpad.com` |  

```text
덧글:
 - 마이크로소프트에서 깃허브를 2018년 10월에 인수함
```

---

# 표식하기 통달(Mastering-Markdown)

표식하기(Markdown)는 깃허브(GitHub) 플랫폼에서 모든 글쓰기 서식을 표현하기위한 가볍고 사용하기쉬운 문법이다.

**배우게 될 것:**  

- 공동으로 수정하기 쉬운 표현의 표식하기 양식을 만드는 방법  
- 일반적인 양식화 방법과 표식하기의 차이점  
- 문자를 양식화하기 위하여 표식하기를 사용하는 방법  
- 깃허브에 표식하기 표현을 자동으로 적용하는 방법  
- 깃허브에 표식하기의 고유한 확장을 적용하는 방법  

> ## 알맹이
>
> ### [1 표식하기(Markdown)는 무엇인가?](#표식하기)
>
> ### [2 본보기(Examples)](#본보기)
>
> [2-1 간략한 본보기(Examples)](#2-1)  
> [2-2 목록 형식](#2-2)  
> [2-3 이미지 연결](#2-3)  
> [2-4 글머리 & 따옴표](#2-4)  
> [2-5 코드 표현](#2-5)  
> [2-6 추가기능](#2-6)  
> 
> ### [3 문법 안내(Syntax guide)](#문법안내)
> 
> [3-1 기본문법](#3-1)  
> [3-2 글머리(Headers)](#3-2)  
> [3-3 강조(Emphasis)](#3-3)  
> [3-4 목록](#3-4)  
> [3-5 이미지](#3-5)  
> [3-6 연결](#3-6)  
>  [가. 웹주소 연결](#웹주소)  
>  [나. 문서내 연결](#문서내)  
> [3-7 인용문](#3-7)  
> [3-8 내장 코드](#3-8)  
> 
> ### [4. 깃허브풍의 표식하기](#깃허브풍)
> 
> [4-1 문법 강조](#4-1)  
> [4-2 작업 목록](#4-2)  
> [4-3 표](#4-3)  
> [4-4 SHA 참조](#4-4)
> [4-5 저장소 내에서 쟁점참조](#4-5)  
> [4-6 사용자명 @언급](#4-6)  
> [4-7 URL에 대한 자동 연결](#4-7)  
> [4-8 취소선](#4-8)  
> [4-9 감성기호(이모지, Emoji)](#4-9)  
> [4-10 유튜브 동영상 연결](#4-10)  
> [4-11 수학식 표현](#4-11)  

- codecogs에서 `gif` 파일을 만들어 내려받고, 연결로 표현  
- codecogs의 latex 로 직접 표현  

---

<a name="표식하기"></a>

## 1 표식하기(Markdown)는 무엇인가?

표식하기([Markdown](http://daringfireball.net/projects/markdown/))는 웹에서 문자 서식을 지정하는 방법이다. 문서의 표시를 제어한다; 단어를 강조 또는 기울임으로 양식화, 이미지 추가, 그리고 목록 만들기는 표식하기로 할 수 있는 단지 몇 가지 이다. 주로, 표식하기는 알파벳이 아닌 기호가 몇 개 있는 일 반 문자이다, `#` 또는 `*` 같은.

표식하기는 깃허브 대부분의 공간에서 사용할 수 있다:  

- [깃사용자들(기스트들, Gists)](https://gist.github.com/)  
- 쟁점(Issues)과 긁어오기요청(Pull requests)에서 주석달기  
- `.md` 또는 `.markdown` 확장자로 된 파일들  

더 자세한 정보는, 깃허브 도우미에서 "[깃허브에 기록(Writing on Github)](https://help.github.com/categories/writing-on-github/)"을 참조.

---

<a name="본보기"></a>

## 2 본보기(Examples)

<a name="2-1"></a>

### 2-1 간략한 본보기(Examples)

```bash
표식하기로 어떤 단어를 **강조** 그리고 다른 단어의 *기울임* 을 아주 쉽게 만들 수 있다.
심지어 [구글에 연결!](http://google.com)을 할 수 있다.
```

표식하기로 어떤 단어를 **강조** 그리고 다른 단어의 *기울임* 을 아주 쉽게 만들 수 있다.  
심지어 [구글에 연결!](http://google.com)을 할 수 있다.

<a name="2-2"></a>

### 2-2 목록 형식

```text
때로는 순번있는 목록이 필요하다:
1. 일
1. 이
1. 삼

때로는 중요한 것이 필요하다
* 별로 행을 시작한다
* 이점!

그 대신에,

- 음부호는 아주 잘 동작한다
- 그리고 종속목록이 있다면, 별 또는 음부호 앞에 공백 2개를 삽입한다:
  - 이것처름
  - 그리고 이것처럼
```

때로는 순번있는 목록이 필요하다:

1. 일
2. 이
3. 삼

때로는 중요한 것이 필요하다

* 별로 행을 시작한다
* 이점!

그 대신에,

- 음부호는 아주 잘 동작한다
- 그리고 종속목록이 있다면, 별 또는 음부호 앞에 공백 2개를 삽입한다:
  - 이것처름
  - 그리고 이것처럼

<a name="2-3"></a>

### 2-3 이미지 연결  

이미지 소박이가 필요하다면, 이것을 어떻게 하는가:

```html
<p align="left"><img width="10%" src="images/yaktocat.png" /></p>   <= 좌측정렬, 원본크기의 10%
<p align="center"><img width="10%" src="images/yaktocat.png" /></p> <= 중앙정렬, 원본크기의 10%
<p align="right"><img width="10%" src="images/yaktocat.png" /></p>  <= 우측정렬, 원본크기의 10%
<p align="center"><img width="50%" src="images/yaktocat.png" /></p> <= 중앙정렬, 원본크기의 50%

![문어고양이 이미지](https://octodex.github.com/images/yaktocat.png)     <= 원본크기의 100%
```

소박이한 이미지가 필요하다면, 이것을 어떻게 하는가:
<p align="left"><img width="10%" src="images/yaktocat.png" /></p>
<p align="center"><img width="10%" src="images/yaktocat.png" /></p>
<p align="right"><img width="10%" src="images/yaktocat.png" /></p>
<p align="center"><img width="50%" src="images/yaktocat.png" /></p>

![문어고양이 이미지](images/yaktocat.png)

<a name="2-4"></a>

### 2-4 글머리 & 따옴표

```text
# 짜임새있는 문서
때로는 문서를 짜임새있게 하기 위하여 글머리 수준이 다른것을 사용하는것이 유용하다.
글머리를 생성하기 위하여 '#'으로 행을 시작한다.
더작은 글머리 크기는 한행에 여러개의 '##'를 표시한다.

### 이것은 세번째-단계 글머리다
글머리 크기에 대해서 '#' 하나에서 '######' 6개까지 사용할 수 있다.

어떤것을 인용하고 싶다면, 행의 시작에 > 기호를 사용한다:
> 커피. 지금까지 고안된 최고급 유기물이다... 나는 이것으로 보르그를 이겼다.
> - 캡틴 제인웨이
```

> # 짜임새있는 문서
>
> 때로는 문서를 짜임새있게 하기 위하여 글머리 수준이 다른것을 사용하는것이 유용하다.
> 글머리를 생성하기 위하여 '#'으로 행을 시작한다.
> 더작은 글머리 크기는 한행에 여러개의 '##'를 표시한다.
>
> ### 이것은 세번째-단계 글머리다
>
> 글머리 크기에 대해서 '#' 하나에서 '######' 6개까지 사용할 수 있다.
> 어떤것을 인용하고 싶다면, 행의 시작에 > 기호를 사용한다:
>> 커피. 지금까지 고안된 최고급 유기물이다... 나는 이것으로 보르그를 이겼다.
>> -캡틴 제인웨이

<a name="2-5"></a>

### 2-5 코드 표현

```java
깃허브의 표식하기로 코드를 꾸미기 위한 다양한 방법이 있다.  
인라인 코드 덩이가 있다면, 역따옴표로 감싼다: `var example = true`.  
좀더 긴 코드덩이를 가지고 있다면, 4개의 공백으로 들여쓸 수 있다:  

    if (isAwesome)
    {
        return true
    }

깃허브는 또한 코드울타리 라는것을 지원한다,  
이것은 들여쓰기가 없는 여러 행을 허용한다:
  ` ` `
  if (isAwesome)
  {
    return true
  }
  ` ` `

그리고 문법 강조하기를 사용하고 싶다면, 언어를 포함한다:
  ` ` `javascript
  if (isAwesome)
  {
    return true
  }
  ` ` `

  ` ` `bash
  if (isAwesome)
  {
    return true
  }
  ` ` `
```

깃허브의 표식하기로 코드를 꾸미기 위한 다양한 방법이 있다.  
인라인 코드 덩이가 있다면, 역따옴표로 감싼다: `var example = true`.  
좀더 긴 코드덩이를 가지고 있다면, 4개의 공백으로 들여쓸 수 있다:  

    if (isAwesome)  
    {  
        return true  
    }  

깃허브는 또한 코드울타리 라는것을 지원한다,  
이것은 들여쓰기가 없는 여러 행을 허용한다:  

  ```
  if (isAwesome)
  {
    return true
  }
  ```

그리고 문법 강조하기를 사용하고 싶다면, 언어를 포함한다:

  ```javascript
  if (isAwesome)
  {
    return true
  }
  ```

  ```bash
  if (isAwesome)
  {
    return true
  }
  ```

<a name="2-6"></a>

### 2-6 추가기능

```t
깃허브는 표식하기에서 사람에게 문의및 연결등의 많은 추가기능을 지원한다.
만약 누군가에게 의견을 직접 보내기를 원한다면,
이름에 @ 기호 접두사를 붙일 수 있다:
안녕 @효진 - 스웨터 이쁘다!  

하지만 나는 인정한다, 작업목록이 내 마음에 든다:
- [x] 이것은 완료된 항목이다
- [ ] 이것은 미완료 항목이다

쟁점의 첫번째 의견에 작업목록을 포함시키면,
너의 쟁점목록에서 도움이되는 진도막대를 볼 수 있다.
또한, 이것은 요청당겨오기에서도 작동한다!  

그리고, 당연히 이모티콘도! :kr: :sparkles: :camel: :boom:
```

깃허브는 표식하기에서 사람에게 문의및 연결등의 많은 추가기능을 지원한다.
만약 누군가에게 의견을 직접 보내기를 원한다면,
이름에 @ 기호 접두사를 붙일 수 있다:
안녕 @효진 - 스웨터 이쁘다!  

하지만 나는 인정한다, 작업목록이 내 마음에 든다:

- [x] 이것은 완료된 항목이다
- [ ] 이것은 미완료 항목이다

쟁점의 첫번째 의견에 작업목록을 포함시키면,
너의 쟁점목록에서 도움이되는 진도막대를 볼 수 있다.
또한, 이것은 요청당겨오기에서도 작동한다!  

그리고, 당연히 그림상징(이모티콘)도! :kr: :sparkles: :camel: :boom:

> 참조: [그림상징(이모티콘) 보기](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

---

<a name="문법안내"></a>

## 3 문법 안내(Syntax guide)

다음은 표식하기 문법의 요약이다 이것은 GitHub.com의 어디에서나 또는 자신의 문자 파일에서 사용할 수 있다.

<a name="3-1"></a>

### 3-1 기본문법

```t
구분선     ==> ---
기울임     ==> * * 또는 _ _
강조       ==> ** ** 또는 __ __
배경       ==> ` ` (불꽃)
취소       ==> ~~ ~~ (물결)
강제줄바꿈  ==> 문장끝에 공백 2개를 연속으로 삽입한다
```

<a name="3-2"></a>

### 3-2 글머리(Headers)

```t
# 이것은 글머리1인 <h1>의 식별자 이다
## 이것은 글머리2인 <h2>의 식별자 이다
###### 이것은 글머리6인 <h6>의 식별자 이다
```

> # 이것은 글머리1인 \<h1>의 식별자 이다
> ## 이것은 글머리2인 \<h2>의 식별자 이다
> ###### 이것은 글머리6인 \<h6>의 식별자 이다

<a name="3-3"></a>

### 3-3 강조(Emphasis)

```t
*이 문자는 기울어진다* _이것 또한 기울어진다_
**이 문자는 강조된다** __이것 또한 강조된다__
_이것을 **조합**할 수 있다_
그리고
`이것은 배경이있다`
~~이것은 글자에 가로선을 추가한다~~
```

> *이 문자는 기울어진다* _이것 또한 기울어진다_  
> **이 문자는 강조된다** __이것 또한 강조된다__  
> _이것을 **조합**할 수 있다_  
> 그리고  
> `이것은 배경이있다`  
> ~~이것은 글자에 가로선을 추가한다~~  

<a name="3-4"></a>

### 3-4 목록

#### 3-4-1 순번없는

```t
* 항목 1
* 항목 2
  * 항목 2)
  * 항목 2)
```

* 항목 1
* 항목 2
  * 항목 2)
  * 항목 2)

#### 3-4-2순번있는

```t
1. 항목 1
1. 항목 2
1. 항목 3
    3.1 항목 1)
    3.2 항목 2)
1. 항목 4
```

1. 항목 1
1. 항목 2
1. 항목 3  
    3.1 항목 1)  
    3.2 항목 2)  
1. 항목 4

<a name="3-5"></a>

### 3-5 이미지

```t
![깃허브 감성기호](/images/GitHub-Mark.png)

양식: ![깃허브 상징](https://github.com/zeuseyera/Mastering-Markdown-kr/blob/master/images/GitHub-Logo.png)
```

> ![깃허브 감성기호](/images/GitHub-Mark.png)  

> 양식: ![깃허브 상징](https://github.com/zeuseyera/Mastering-Markdown-kr/blob/master/images/GitHub-Logo.png)

<a name="3-6"></a>

### 3-6 연결

<a name="웹주소"></a>

가. 웹주소 연결

```t
http://github.com - 자동!
[깃허브](http://github.com)
```

http://github.com - 자동!  
[깃허브](http://github.com)

<a name="문서내"></a>

나. 문서내 연결

```t  
<!-- MarkdownTOC depth=4 -->  
`마우스 클릭으로 문서내에서 이동할 위치의 연결을 정의한다`  
- [문서내에서 어디로 갈까?](#여기로-이동)

`"#여기로-이동"으로 정의된 "문서내에서 어디로 갈까?" 연결을 마우스로 클릭하면 이동할 위치를 지정한다`
<a name="여기로-이동"></a>
- 여기로 이동 - "문서내에서 어디로 갈까?"를 마우스로 클릭하면 화면이 여기로 이동한다  
```

<!-- MarkdownTOC depth=4 -->  
`마우스 클릭으로 문서내에서 이동할 위치의 연결을 정의한다`  

- [문서내에서 어디로 갈까?](#여기로-이동)  

`"#여기로-이동"으로 정의된 "문서내에서 어디로 갈까?" 연결을 마우스로 클릭하면 이동할 위치를 지정한다`

<a name="여기로-이동"></a>  

- 여기로 이동 - "문서내에서 어디로 갈까?"를 마우스로 클릭하면 화면이 여기로 이동한다  

<a name="3-7"></a>

### 3-7 인용문

```t
칸예 웨스트 말에 의하면:
> 우리는 미래를 살아 간다  그러므로
> 현재는 과거이다.
```

칸예 웨스트 말에 의하면:
> 우리는 미래를 살아 간다  그러므로  
> 현재는 과거이다.

<a name="3-8"></a>

### 3-8 내장 코드

```t
내장코드를 사용해야 한다면  
대신에 <addr> 요소를 사용한다.  
```

내장코드를 사용해야 한다면  
대신에 <addr> 요소를 사용한다.  

---

<a name="깃허브풍"></a>

## 4. 깃허브풍의 표식하기

GitHub.com은 유용한 특징집합을 추가적으로 제공하고 표식하기 문법 자체를 사용한다, 많은 것들을 GitHub.com의 내용으로 작업하기 쉽다.
깃허브풍의 표식하기의 일부 특징은 쟁점과 요청당겨오기의 설명과 주석에 대한 사용할 쉬 있다는 것을 알린다. 이것들은 SHA-1에 대한 언급, 쟁점, 그리고 요청 당겨오기의 언급 뿐만아니라 참조도 포함한다. 작업목록은 또한 요지주석에서도 가능하다 그리고 요지주석 파일에서도.

<a name="4-1"></a>

### 4-1 문법 강조

여기에 [깃허브풍의 표식하기](https://help.github.com/articles/basic-writing-and-formatting-syntax/)로 문법을 강조하는 방법의 본보기가 있다:

```javascript
function fancyAlert( arg )
{
    if( arg )
    {
        $.facebox( { div:'#foo' } )
    }
}
```

또한 공백 4개로 간단하게 코드 들여쓰기를 할 수 있다:  

```js
    function fancyAlert( arg )  
    {  
        if( arg )  
        {  
            $.facebox( { div:'#foo' } )  
        }  
    }  
```

여기는 문법강조가 없는 파이썬 코드의 본보기다:  

```js
def foo():  
    if not bar:  
        return True  
```

<a name="4-2"></a>

### 4-2 작업 목록

```t
- [x] @언급, #참조, [연결](), **양식설정**, 그리고 <del>취소</del> 를 지원한다
- [x] 목록문법 필요 (순번없는 또는 순번있는 모든 목록 지원)
- [x] 이것은 완료된 항목이다
- [ ] 이것은 미완료 항목이다
```

> - [x] @언급, #참조, [연결](), **양식설정**, 그리고 <del>취소</del> 를 지원한다
> - [x] 목록문법 필요 (순번없는 또는 순번있는 모든 목록 지원)
> - [x] 이것은 완료된 항목이다
> - [ ] 이것은 미완료 항목이다

<a name="4-3"></a>

### 4-3 표

단어목록을 조합하여 표를 만들 수 있다 그리고 가로기호(하이픈)'-'으로 나눈다 (첫번째 행을 위하여)나눈다, 그리고 그런다음 세로기호(파이프)'|'로 각 열을 분리한다:
그리고 **:** 는 정렬기호다

```t
| 첫번째 글머리 | 두번째 글머리 | 세번째 글머리 | 네번째 글머리 |  
| ---          | ---          | :---:        | ---:         |  
| 첫번째 열의 내용 | 두번째열의 내용 | :가운데정렬: | 오른쪽정렬: |  
```

아래처럼 표시될 것이다:  

| 첫번째 글머리 | 두번째 글머리 | 세번째 글머리 | 네번째 글머리 |  
| ---          | ---          | :---:        | ---:         |  
| 첫번째 열의 내용 | 두번째열의 내용 | :가운데정렬: | 오른쪽정렬: |  

<a name="4-4"></a>

### 4-4 SHA 참조

지르기(커밋)위한 [:kr:SHA-1 뭇칼질](./SHA-1_안전한뭇칼질알고리즘/SHA-1.md)[(영문)](http://en.wikipedia.org/wiki/SHA-1)의 모든 참조는 깃허브에서 지르기(커밋)에 대한 연결로 자동으로 변환된다.

```t
16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac
```

> 16c999e8c71134401a78d4d46435517b2271d6ac  
> mojombo@16c999e8c71134401a78d4d46435517b2271d6ac  
> mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac  

<a name="4-5"></a>

### 4-5 저장소 내에서 쟁점참조

쟁점 또는 요청 끌어오기를 나타내는 모든 숫자는 연결로 자동적으로 변환된다

```t
#1
mojombo#1
mojombo/github-flavored-markdown#1
```

> #1  
> mojombo#1  
> mojombo/github-flavored-markdown#1

<a name="4-6"></a>

### 4-6 사용자명 @언급

골뱅이('@') 기호를 입력하면, 사용자명 다음에, 그 사람에게 오라고 알리 것이다 그리고 주석을 본다. 이것은 "@언급(mention)"이라고 한다, 당신이 개인적으로 언급하기 때문이다. 또한 조직내의 팀을 @언급 할 수 있다.

<a name="4-7"></a>

### 4-7 URL에 대한 자동 연결

모든 URL(`http://www.github.com/` 처럼)은 클릭할 수 연결로 자동적으로 변환된다.

<a name="4-8"></a>

### 4-8 취소선

두개의 물결기호(tilde)로 감싼(~~이것~~ 처럼) 모든 단어는 횡단되어 나타난다.

<a name="4-9"></a>

### 4-9 감성기호(이모지, Emoji)

깃허브는 감성기호를 지원한다! :kr: :sparkles: :camel: :boom:  
우리가 지원하는 모든 이미지의 목록을 보려면, [감성기호 요약 쪽지](http://www.emoji-cheat-sheet.com/)를 확인해라.

<a name="4-10"></a>

### 4-10 유튜브 동영상 연결

참조: `https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet`  

유튜브 동영상은 직접 추가할 수 없다 하지만 다음과 같이 동영상에 대한 연결이 포함된 이미지를 추가할 수 있다:  

```html
<a href="https://www.youtube.com/watch?feature=player_embedded&v=유튜브동영상 고유명칭은 여기에"
target="_blank"><img src="https://img.youtube.com/vi/유튜브동영상 고유명칭은 여기에/0.jpg"
alt="이미지 대체문자는 여기에" width="240" height="180" border="10" /></a>

[![이미지 대체문자는 여기에](https://img.youtube.com/vi/유튜브동영상 고유명칭 여기에/0.jpg)](https://www.youtube.com/watch?v=유튜브동영상 고유명칭은 여기에)
```

> <a href="https://www.youtube.com/watch?feature=player_embedded&v=VOC3huqHrss" target="_blank"><img src="https://img.youtube.com/vi/VOC3huqHrss/0.jpg" alt="욜로v2" width="240" height="180" border="10" /></a>

> [![이미지 대체문자는 여기에](https://img.youtube.com/vi/VOC3huqHrss/0.jpg)](https://www.youtube.com/watch?v=VOC3huqHrss)

<a name="4-11"></a>

### 4-11 수학식 표현

- mathjax 방식 사용  

- [표식하기 수학식 문자 위키피디아 참조](https://ko.wikipedia.org/wiki/위키백과:TeX_문법)

#### 가. 문장내 표현

- 표현할 수식의 시작과 끝에 '$'를 하나씩 추가한다.

> ```math
> 문장을 작성중에 $수식: x = a_1 * x^2$ 처럼 표현하면 문장내에 표현할 수 있음.
> ```
> 
> 문장을 작성중에 $수식: x = a_1 * x^2$ 처럼 표현하면 문장내에 표현할 수 있음.

#### 나. 한줄에 표현(수식만)

- 표현할 수식의 시작과 끝에 '$'를 두개씩 추가한다.

> 본보기 1
> 
> ```math
> $$Pr(Class_i|Object) ∗ Pr(Object) ∗ IOU^{truth}_{pred} = Pr(Class_i) ∗ IOU^{truth}_{pred} \qquad (1)$$
> ```
> 
> $$Pr(Class_i|Object) ∗ Pr(Object) ∗ IOU^{truth}_{pred} = Pr(Class_i) ∗ IOU^{truth}_{pred} \qquad (1)$$

> 본보기 2
> 
> ```math
> $$\phi(x) = \begin{cases} x, & x > 0 \mathsf{\mbox{ 이면}} \\
>  0.1x, & \mathsf{\mbox{아니면}} \end{cases} \qquad (2)$$
> ```
> 
> $$\phi(x) = \begin{cases} x, & x > 0 \mathsf{\mbox{ 이면}} \\
>  0.1x, & \mathsf{\mbox{아니면}} \end{cases} \qquad (2)$$

> 본보기 3
>
> ```math
> $$ \lambda_{ \mathsf{coord} } \sum^{S^2}_{i=0}\ \sum^{B}_{j=0}\ \mathbb{1}^{ \mathsf{obj} }_{ij} \left[ (x_i - \hat{x}_i)^2 + (y_i - \hat{y}_i)^2 \right] \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \lambda_{ \mathsf{coord} } \sum^{S^2}_{i=0} \sum^{B}_{j=0} \mathbb{1}^{ \mathsf{obj} }_{ij} \left[ (\sqrt{w_i} - \sqrt{\hat{w}_i})^2 + (\sqrt{h_i} - \sqrt{\hat{h}_i})^2 \right] $$  
> 
> $$ \qquad +\ \sum^{S^2}_{i=0} \sum^{B}_{j=0} \mathbb{1}^{\mathsf{obj}}_{ij} \left( C_i - \hat{C}_i \right)^2 \qquad \qquad \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \lambda_{ \mathsf{noobj} }\ \sum^{S^2}_{i=0}\ \sum^{B}_{j=0} \mathbb{1}^{ \mathsf{noobj} }_{ij} \left( C_i - \hat{C}_i \right)^2 \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \sum^{S^2}_{i=0}\ \mathbb{1}^{ \mathsf{obj} }_{i}\ \sum_{ c \in \mathsf{classes} } \left( p_i(c) - \hat{p}_i(c) \right)^2 \qquad \qquad \qquad (3) $$  
> ```
> 
> $$ \lambda_{ \mathsf{coord} } \sum^{S^2}_{i=0}\ \sum^{B}_{j=0}\ \mathbb{1}^{ \mathsf{obj} }_{ij} \left[ (x_i - \hat{x}_i)^2 + (y_i - \hat{y}_i)^2 \right] \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \lambda_{ \mathsf{coord} } \sum^{S^2}_{i=0} \sum^{B}_{j=0} \mathbb{1}^{ \mathsf{obj} }_{ij} \left[ (\sqrt{w_i} - \sqrt{\hat{w}_i})^2 + (\sqrt{h_i} - \sqrt{\hat{h}_i})^2 \right] $$  
> 
> $$ \qquad +\ \sum^{S^2}_{i=0} \sum^{B}_{j=0} \mathbb{1}^{\mathsf{obj}}_{ij} \left( C_i - \hat{C}_i \right)^2 \qquad \qquad \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \lambda_{ \mathsf{noobj} }\ \sum^{S^2}_{i=0}\ \sum^{B}_{j=0} \mathbb{1}^{ \mathsf{noobj} }_{ij} \left( C_i - \hat{C}_i \right)^2 \qquad \qquad \qquad \qquad $$  
> 
> $$ \qquad +\ \sum^{S^2}_{i=0}\ \mathbb{1}^{ \mathsf{obj} }_{i}\ \sum_{ c \in \mathsf{classes} } \left( p_i(c) - \hat{p}_i(c) \right)^2 \qquad \qquad \qquad (3) $$  

---

#### 그리스 문자 및 기호 표현

출처:
  - http://www.htmlhelp.com/reference/html40/entities/symbols.html

| 명령 | 기호 | 설명 | - |  
| --- | :---: | --- | --- |  
| `&ap;` | &ap; | 비슷하다 | almost equal, asymptotic |  
| `&fnof;` | &fnof; | 함수 | function, florin |  
| `&radic;` | &radic; | 루트 | square root, radical sign |  
| `&infin;` | &infin; | 무한대 | infinity | |  
| `&alpha;, &Alpha;` | &alpha;, &Alpha; | 알파 | |  
| `&beta;, &Beta;` | &beta;, &Beta; | 베타 | |  
| `&delta;, &Delta;` | &delta;, &Delta; | 델타 | |  
| `&epsilon;, &Epsilon;` | &epsilon;, &Epsilon; | 입실론 | |  
| `&gamma;, &Gamma;` | &gamma;, &Gamma; | 감마 | |  
| `&sigma;, &Sigma;` | &sigma;, &Sigma; | 시그마 | |  
| `&omega;, &Omega;` | &omega;, &Omega; | 오메가 | |  
| `&lambda;, &Lambda;` | &lambda;, &Lambda; | 람다 | |  
| `&rho;, &Rho;` | &rho;, &Rho; | 로우 | |  
| `&sum;, &Sum;` | &sum;, &Sum; | 합계 | |  
| `&int;, &Int;` | &int;, &Int; | 인티그랄 | |  
| `&eta;, &Eta;` | &eta;, &Eta; | 에타 | |  
| `&zeta;, &Zeta;` | &zeta;, &Zeta; | 제타 | |  
| `&theta;, &Theta;` | &theta;, &Theta; | 세타 | |  
| `&phi;, &Phi;` | &phi;, &Phi; | | |  
| `&psi;, &Psi;` | &psi;, &Psi; | | |  


| 명령 | 실제 표현 | 설명 | - |
| --- | --- | --- | --- |
| `<sup></sup>` | 앞<sup>중간</sup>뒤 | 위첨자 |
| `<sub></sub>` | 앞<sub>중간</sub>뒤 | 아래첨자 |
| `<ul></ul>` | 앞<ul>중간</ul>뒤 |
| `<dl></dl>` | 앞<dl>중간</dl>뒤 |
| `<s></s>`  | 앞<s>중간</s>뒤 |
