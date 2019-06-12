## <Html, css 실습>

## <06.form 요소, 07.main main-content 스타일링, 08. main side-content, 09. main side-content 스타일링>

# 06. form 요소

form은 로그인할 때, 게시판 글 작성, 여러개 항목 중에서 선택, 검색할 때 등의 입력해서 사용하던 요소들이 form
사용자와 웹사이트가 서로 상호작용하는 중요한 기술 중 하나
웹사이트에서 서버 쪽으로 제출하거나 브라우저에서 사용하기 위해 이용됨

입력된 정보를 어디에 보낼지에 대해 관련된 action 속성, 이 정보를 어떻게 처리할 것인지와 관련된 method 속성
http 배울 때 데이터 관련된 method가 값으로 들어가게 되고, post는 정보를 보낼 때, delete는 정보를 삭제할 때
put, patch는 정보를 수정할 때 사용되는 method
action에 들어가는 값에는 데이터를 보내는 url이 들어가게 됨
지금 당장은 서버와 통신하는 웹사이트를 만드는 게 아니기 때문에 나중에 추가적으로 배울 예정

input 요소는 빈 요소이며 type을 속성으로 가짐
type에 들어오는 값에 따라서 모양이나 입력받는 정보의 유효성이 달라지게 됨
ex) text 라고 type이 입력되면 숫자든 문자든 자유롭게 입력 가능
ex) checkbox -
ex) search, number, email, password,

label 요소같은 경우에는 input 요소와 꼭 한 쌍으로 지정을 해줘야하기 때문에 label에 for라고 되어있는 속성에 들어가는 값이 input의 id로 들어가는 값과 동일해야 하고,
이것은 여러번 사용될 수 없음

input 태그가 여러개 있을 때 이 요소가 어떤 요소인지 설명해주기 위한 캡션이 필요한데, label 요소가 그 역할을 해준다

<실습>
action 같은 경우 당장 사용할 것이 아니기 때문에 "#"
label 요소에 input 요소 설명하는 부분을 적어줄 것
placeholder: 칸 안에 회색 글씨로 어떤 정보를 입력해야하는지 안내해주는 문구 설정
name은 입력받은 이메일을 나중에 어떤 식으로 서버에 전송할지 이럴 때 input에 적힌 데이터를 가지고 오기 위해서 사용하는 경우 있음

'''<label for="">에 들어가는 속성=<input id="">'''

button type

# 07.main main-content 스타일링

:: 점 두개하면 가상 요소
: 콜론 하나면 가상 클래스

보이지 않게 하려면
display: none or visibility: hidden'

해당 크기에 넘치는 내용들은 숨겨지게 됨
overflow: hidden
배경색을 줘서 확인해보니 거의 없어지긴 했지만 쪼금 남아있음 --> margin: -1px,
clip: rect(0, 0, 0, 0)-- 웹 접근성을 향상시키는 데에 가장 권장되는 방법
회색 영역 없어짐
-----> label 요소는 안 보이게 하면서도 screenreader는 인식할 수 있게

border-radius: 4px
height: 5rem 픽셀 값을 50px으로 줘도 됨
botton 속성 같은 경우 input 속성 안에 위치해야되기 때문에 position: absolute를 사용
position absolute 가 어디를 기준으로 잡을 것인지 mailing form 에서 position relative 설정
background: transparent

botton에서 커서의 값에 point를 줘서 손모양
cursor: pointer

자간에 대한 속성: letter-spacing: 음수값 - 좁아짐, 양수값 - 넓어짐

# 08. main side-content

독립적이고 그 자체로 완결된 컨텐츠를 가지는 것을 article 태그로 마크업할 수 있음
time datetime="2019-06-11"

dt, dd요소 사용하게 되면 두 개의 요소가 연관이 있음을 알려줄 수 ㅇ

# 09. main side-content 스타일링

버튼 모양, 색깔 바뀌는 부분, get involved 마진 조절, 화살표? 넣어보는

cta

두 개의 버튼에 공통적으로 뽑아내서 cta 스타일에 적용하고, 나머지는 각자의 class에 적용하는 방식으로 스타일 정해보기

.side-cta:hover
selector specificity (id100점 ,class10점 ,tag1점 )

nth-child에 대해 더 알아보고 싶다면 nth master라는 사이트 참고

p {

}

.classname {
  
}
