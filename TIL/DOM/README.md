# DOM

Document Object Model

## 문서 객체 모델 (DOM) : <https://developer.mozilla.org/ko/docs/Web/API/Document_Object_Model>

* 메모리에 웹 페이지 문서 구조를 표현함으로써 스크립트 및 프로그래밍 언어와 페이지를 연결
* DOM은 문서를 논리 트리로 표현합니다. 트리의 각 브랜치는 노드에서 끝나며, 각 노드는 객체를 갖습니다. DOM 메서드를 사용하면 프로그래밍적으로 트리에 접근할 수 있습니다. 이를 통해 문서의 구조, 스타일, 콘텐츠를 변경할 수 있습니다.
* 노드는 이벤트 처리기도 포함할 수 있습니다. 이벤트가 발생한 순간, 해당 이벤트와 연결한 처리기가 발동합니다.

## <https://developer.mozilla.org/ko/docs/Web/API/Document_Object_Model/Introduction>

### DOM 이란

문서 객체 모델(The Document Object Model, 이하 DOM) 은 *HTML, XML 문서의 프로그래밍 interface* 이다. DOM은 문서의 구조화된 표현(structured representation)을 제공하며 프로그래밍 언어가 DOM 구조에 접근할 수 있는 방법을 제공하여 그들이 문서 구조, 스타일, 내용 등을 변경할 수 있게 돕는다. DOM 은 `nodes`와 `objects`로 문서를 표현한다. 이들은 웹 페이지를 스크립트 또는 프로그래밍 언어들에서 사용될 수 있게 연결시켜주는 역할을 담당한다.

웹 페이지는 일종의 문서(document)다.  이 문서는 웹 브라우저를 통해 그 내용이 해석되어 웹 브라우저 화면에 나타나거나 HTML 소스 자체로 나타나기도 한다. 동일한 문서를 사용하여 이처럼 다른 형태로 나타날 수 있다는 점에 주목할 필요가 있다. DOM 은 동일한 문서를 표현하고, 저장하고, 조작하는 방법을 제공한다. DOM 은 *웹 페이지의 객체 지향 표현*이며, *자바스크립트와 같은 스크립팅 언어를 이용해 DOM 을 수정할 수 있다.*

W3C DOM, WHATWG DOM 표준은 대부분의 브라우저에서 DOM 을 구현하는 기준이다. 많은 브라우저들이 표준 규약에서 제공하는 기능 외에도 추가적인 기능들을 제공하기 때문에 사용자가 작성한 문서들이 각기 다른 DOM 이 적용된 다양한 브라우저 환경에서 동작할 수 있다는 사실을 항상 인지하고 있어야 한다.

### DOM and JS

페이지 콘텐츠(the page content)는 DOM 에 저장되고 자바스크립트를 통해 접근하거나 조작할 수 있다.

API (web or XML page) = DOM + JS (scripting language)

DOM 은 프로그래밍 언어와 독립적으로 디자인되었다. 때문에 문서의 구조적인 표현은 단일 API 를 통해 이용가능하다.

## DOM 접근

스크립트를 작성할 때(인라인 `<script>` 요소를 사용하거나 웹 페이지 안에 있는 스크립트 로딩 명령을 사용하여), 문서 자체를 조작하거나 문서의 children 을 얻기 위해 `document` 또는 `window` elements 를 위한 API 를 즉시 사용할 수 있다.

### 중요한 데이터 타입들

<https://developer.mozilla.org/ko/docs/Web/API/Document_Object_Model/Introduction#important_data_types>

* document : <https://developer.mozilla.org/ko/docs/Web/API/Document>
* element
* nodeList
* attribute
* namedNodeMap
