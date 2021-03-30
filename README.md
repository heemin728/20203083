
------
# Markdown Syntax
### 컴퓨터학부 20203083 강희민
------


## CONTENTS

1. <a href="#Heading">Headings </a>
2. <a href="#Paragraph"> Paragraph </a>
3. <a href="#LineBreaks"> Line Breaks </a>
4. <a href="#Emphasis"> Emphasis </a>
5. <a href="#Blockquotes"> Blockquotes </a>
6. <a href="#Lists"> Lists </a>
7. <a href="#Code"> Code </a>
8. <a href="#HorizontalRules">Horizontal Rules </a>
9. <a href="#Links"> Links </a>
10. <a href="#Images"> Images </a>
11. <a href="#EscapingCharacters"> Escaping Characters </a>
12. <a href="#HTML"> HTML </a>  

 <a href="#Github"> Github Link </a>



----

<h2 id = "Heading">

# Headings  

</h2>

- 단어나 구문 앞에 number signs(#) 추가  
- #의 개수가 제목의 레벨과 같음
- **한 칸 공백** 필요
- 또는 문장 아래 "===="(level 1), "----"(level 2) 추가

        # LEVEL 1
        ## LEVEL 2
        ### LEVEL 3
        #### LEVEL 4

    
    # LEVEL 1
    ## LEVEL 2
    ### LEVEL 3
    #### LEVEL 4

<br>

---


<h2 id = "Paragraph">  

# Paragraphs

</h2>

- **blank line**을 사용하여 문단을 생성
- 리스트 내부의 문단이 아니라면, 스페이스 혹은 탭은 사용하지 않음

<br>


---

<h2 id = "LineBreaks">  

# Line breaks

</h2>

- 스페이스를 두번 이상 치고 엔터

    > 에디터에서 trailing whitespace를 찾기 어려우며, 많은 사람들이 우연히 또는 의도적으로 모든 문장 끝에 두번씩 스페이스를 치는 경우가 있다는 문제점
- 따라서, html tag와 같은 < b r > 을 이용해 줄바꿈을 하는 것을 권장 

 <br>

---

<h2 id = "Emphasis">  

# Emphasis

</h2>

<br>

### Bold 
- 구문 앞 뒤로 asterisks(*) 또는 underscores(_)를 두 개씩 **공백 없이** 붙여준다.
- 호환성을 위해 단어 중간에는 __보다는 **를 쓰는 것이 좋음. 
<br>

        learning **markdown** language

    learning **markdown** language

<br>

### Italic
- 구문 앞뒤로 asterisks(*), 또는 underscores(_)를 한 개씩 *공백 없이* 붙여준다.
- 호환성을 위해 단어 중간에는 _보다 *를 쓰는 것이 좋음
<br>

        learning *markdown* language
    learning *markdown* language
   
<br>

### Bold와 Italic 동시에 쓰기
- 구문 앞뒤로 asterisks(*), 또는 underscores(_)를 세 개씩 ***공백 없이*** 붙여준다.
- 호환성을 위해 단어 중간에는 __보다는 ***를 쓰는 것이 좋음. 
<br>

        Learning ***Markdown*** using VS Code
    Learning ***Markdown*** using VS Code

<br>



---



<h2 id = "Blockquotes">  

# Blockquotes

</h2>

- paragraph 앞에 > 추가
<br>

        > Creating Blockquote

    > Creating Blockquote

<br>

### Blockquotes with muliple paragraphs
- paragraphs 사이의 빈 라인에 > 추가
<br>

        >multiple paragraphs
        >
        >using markdown language!

    
    >multiple paragraphs
    >
    >using markdown language!

<br>

### Nested blockquotes
- nest 하고 싶은 paragraph 앞에 ' >> ' 
<br>

        >Nested blockquotes
        >>in markdown language!


    >nested blockquotes
    >>in markdown language!

<br> 

### 다른 요소 추가
- 다른 마크다운 형식을 사용할 수 있음

        > #### blockquotes with other elements 
        > - lists
        > - lists
        >
        > *italic*.. **bold**

    > #### Blockquotes with other elements
    >
    > - lists 1
    > - lists 2
    >
    > *italic*..  **bold**
<br>


---


<h2 id = "Lists"> 

# Lists

</h2>
<br>

### Ordered Lists
- 숫자 + 온점 (1.)
- 숫자의 순서를 지킬 필요는 없으나, 무조건 '1.'로 시작해야 함
- 공백 필요

        1. 하나<br>
        1. 둘<br>
        5. 셋<br>
        2. 넷<br>
    
    1. 하나<br>
    1. 둘<br>
    5. 셋<br>
    2. 넷<br>
<br>

- tab을 사용해 indented item을 추가할 수 있음

        1. 하나<br>
        2. 둘<br>
            1. 하나<br>
            4. 둘<br>
    
    1. 하나<br>
    2. 둘<br>
        1. 하나<br>
        4. 둘<br>
<br>

- 호환성 측면에서 ***'1)'*** 는 사용하지 말 것 : 모든 markdown applications이 지원하는게 아님.  

<br>

### Unordered Lists

- 라인 앞에 dashes(-), asterisks(*), plus signs(+) 모두 가능

- +, *, -, 모두 사용 가능하지만, ***이 세개를 한 개의 리스트에 중복하여 사용할 수 없음.*** 

- tab 또는 space 4번을 이용해 nested list를 만들 수 있음.
- elements 추가 가능


        - unodered lists
        - first item
        - second item
            - indented item

   - unodered lists
   - first item
   - second item
       - indented item

<br>

### 리스트에 요소 더하기 
* 4번의 스페이스 혹은 1번의 탭 

#### Paragraphs

        * first list item
        * second list item

            another paragraph

        * third list item 

   * first list item
   * second list item
          another paragraph

   * third list item. 


#### Blockquotes


        * first list item
        * second list item
            > A blockquote in second list item.
        * third list item 


*   first list item.
*   second list item.

    > A blockquote in second list item.

*   third list item

#### Code Block
* 코드가 리스트 안에 있을때는 **스페이스 8번 또는 탭 두번**

        1. Open the file.
        2. Find the following code block on line 21:

                <html>
                    <head>
                        <title>Test</title>
                        </head>

        3. Update the title to match the name of your website. 

    1. Open the file.
    2. Find the following code block on line 21:

            <html>
                <head>
                    <title>Test</title>
                    </head>

    3. Update the title to match the name of your website. 


#### Images
- 이미지 

        1. The logo of soongil university.

            ![soongsil.jpg](/soongsil.jpg)
        
        2. close the file.


 1. The logo of soongil university.


  ![soongsil.jpg](/soongsil.jpg)
    
 2. close the file.



#### Lists

- ordered list 안에 unordered list를 넣을 수도 있음. 반대도 가능

        1. first item.
        2. second item.
        3. thrid item.
            - indented item
            - also
        4. fouth item.

    1. first item.
    2. second item.
    3. thrid item.
        - indented item
        - also
    4. fouth item.
<br>


---


<h2 id = "Code">  

# Code

</h2>

- 단어나 구문을 코드로 쓰기- 앞뒤로 backticks 사용<br>
            `` at the command prompt, type `nano` ``
            at the command prompt, type `nano` 
    
<br>

### Escaping backticks
- double backticks 사용
            ``use `code` in our markdown file. ``
           `` ``use `code` in our markdown file. `` ``

<br>

### Code blocks 
- 모든 코드 라인을 4번의 스페이스 또는 한번의 탭으로 들여쓰기
<br>


---



<h2 id = "HorizontalRules">  

# Horizontal Rules

</h2>

- 3개 이상의 asterisks(*), dashes(-), underscores(_) 사용 

                ****
                ____

                ----


    ****
    ____

    ----

- 호환성을 위해 **앞뒤로 한줄씩 blank line 포함**

---

<h2 id = "Links">  

# Links 

</h2>

- [링크할 글자] (URL 입력)

        숭실대학교 홈페이지: [Soongsil University]( http://www.ssu.ac.kr/)


    숭실대학교 홈페이지:  [Soongsil University]( http://www.ssu.ac.kr/)

<br>

### Adding title
- 링크에 제목을 추가할 수 있음
- tooltip:  URL 옆에 " tooltip 문장 " 추가

            [Soongsil University]( http://www.ssu.ac.kr/ "MY School")

    [Soongsil University]( http://www.ssu.ac.kr/ "MY School")

<br>

### URLs and Email addresses
- angle brackets ( < > ) 에 URL 또는 이메일 주소 입력

            <http://www.ssu.ac.kr/> 
            <fake@example.com>

    <http://www.ssu.ac.kr/> 
    <fake@example.com>
<br>

- 강조를 위해 [ ] 앞 뒤에 * , 링크를 코드로 표현하기 위해 ' 를 [ ] 안에 사용 가능 (Formatting Links)

        I love supporting the **[EFF](https://eff.org)**.
        This is *[Soongsil University](https://www.ssu.ac.kr/)*.

    I love supporting the **[EFF](https://eff.org)**.
    This is *[Soongsil University](https://www.ssu.ac.kr/)*.


<br>

### Reference Style Links

- 마크다운에서 URL을 보고 읽기 쉽도록 만든 Links

- 두가지 파트로 구성
    - First Part : 글 속에 나타날 링크의 제목 
    - Second Part : 글을 읽기 쉽도록 하기 위하여 다른 부분에 저장한 주소

<br>

#### First Part of the link

    [링크로 나타날 글자][다른 곳에 저장된 주소를 가리키기 위한 label] 

- 첫 번째 `[ ]` 와 두 번째 `[ ]`사이는 붙여쓰거나 한 칸 띄어 쓸 수 있음
- label은 문자, 숫자, 스페이스, 구두점 모두 올 수 있음

        [Soongsil][1]
        [Soongil] [1]

<br>

#### Second Part of the link

    [label]: URL for Link "Optional Title"

- [label]과 colon(`:`) 사이는 공백 없음
- colon(:)과 URL 사이에는 적어도 하나의 공백이 필요
- URL을 angle brackets 사이에 둘 수도 있음
- Optional Title은 double quotes( " " ), single quotes(' '), or parentheses( ( ) )의 사이에 둘 수 있음

- 다음 7가지의 예는 모두 같음

        [1]: http://www.ssu.ac.kr/
        [1]: http://www.ssu.ac.kr/ "Soongsil University"
        [1]: http://www.ssu.ac.kr/ 'Soongsil University'
        [1]: http://www.ssu.ac.kr/ (Soongsil University)
        [1]: <http://www.ssu.ac.kr/> "Soongsil University"
        [1]: <http://www.ssu.ac.kr/> 'Soongsil University'
        [1]: <http://www.ssu.ac.kr/> (Soongsil University)

<br>

- Stadard URL Link를 이용

        Soongil University address is : [soongsil](http://www.ssu.ac.kr/)
    Soongil University address is : [soongsil](http://www.ssu.ac.kr/)


<br>

- Reference Style Link를 이용

        Soongil University address is : [soongsil][1]

        [1]: http://www.ssu.ac.kr/ "Soongsil University"

     Soongil University address is : [soongsil][1]

 [1]: http://www.ssu.ac.kr/ "Soongsil University"


<br>


---


<h2 id = "Images">  

# Image 삽입

</h2>

- exclamation mark(!) + [ alt text ] (URL or Path)

- URL 옆에 제목을 추가할 수 있음

        ![markdown](/markdown.jpg)

    ![markdown](/markdown.jpg)

<br>

### Linking image

- 사진에 링크 추가

-  [!\[alt text](url or path)](link)

           [![campus](/campus.jpg)](http://www.ssu.ac.kr/)

    [![campus](/campus.jpg)](http://www.ssu.ac.kr/)
<br><br>



---



<h2 id = "EscapingCharacters">  

# Escaping Characters

</h2>

- 마크다운 문서에서 format text로 사용될 수 있는 문자를 나타내기 위하여 쓰임
- 문자 앞에 ' \ ' 추가  

        \* with escaping character-not bolding

 \* with escaping character-not bolding

<br>

### backlash(\\)를 통해  Escape 할 수 있는 문자

| Character | Name |
| ----------- | ----------- |
| Header | backslash |
| Paragraph | backtick |
|  *  | asterisk|
|_|underscore|
|{ }|curly braces|
|[ ]|brackets|
|< >|angle brackets|
|( )|parentheses|
|#|	pound sign|
|+|plus sign|
|-|minus sign (hyphen)|
|.|dot|
|!|exclamation mark|
|\||pipe|
<br>


---


<h2 id = "HTML">  

# HTML 

</h2>

- html 태그 사용 가능
- 특정한 html 태그를 선호할 때 유용

        We can make this word in <em> italic type </em> using <em> HTML tag</em>.

  We can make this word in <em> italic type </em> using <em> HTML tag</em>. 


  ---

 <h2 id="Github">

[====20203083 강희민 Github Repository URL====](https://github.com/heemin728/_20203083)

</h2>
