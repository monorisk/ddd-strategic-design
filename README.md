# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장식사 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장식사 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장식사 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장식사 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장식사 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장식사 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장식사 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

<br>
<br>
<br>

--------------------------

## 용어 사전
### 보편적 용어

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 손님 | Customer | `돈`을 지불하고 `메뉴`를 `구매`하는 주체이다. |
| 매장 | Shop | `손님`에게 `돈`을 받고 `메뉴`를 `판매`하고 이를 위한 운영을 수행하는 주체이다.  |
| 배달 | Delivery | `매장`이 아닌 곳에 위치한 `손님`에게 `메뉴`를 전달하는 행위이다. |
| 배달 기사 | Rider | `배달 주문 유형`의 `주문`을 `손님`에게 전달하는 주체이다. |
| 돈 | Money | `메뉴`처럼 `손님`에게 `판매` 되는 요소의 가격이나, `상품`처럼 운영에 필요한 요소들의 가격을 지불할 수 있는 요소를 의미한다. |
| 판매 | Sale | `매장`이 `손님`에게 `메뉴`들을 `돈`을 받고 제공하는 행위이다. |
| 조리 | Cooking | `매장`이 `손님`이 `주문`한 `메뉴`들을 만드는 행위이다.  |

### 상품 용어
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 상품 | Product | `메뉴`를 구성할 수 있는 요소이다. |
| 상품 가격 | Product Price | `상품`의 가격을 의미하며, 이것을 이용하여 `메뉴 원가`를 책정한다. |
| 상품 이름 | Product Name | `상품`의 이름을 의미한다. |

### 메뉴 용어
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 그룹 | Menu Group | `메뉴`의 종류를 구분하는 방법이다. 그룹을 이용하여 치킨/음료/사이드 등의 종류를 구별한다. |
| 메뉴 그룹 이름 | Menu Group Name | `메뉴 그룹`의 이름을 의미한다. 이것을 이용하여 종류의 특징을 나타낸다. |
| 메뉴 | Menu | `손님`에게 판매될 수 있는 요소이다. |
| 메뉴 가격 | Menu Price | `메뉴`의 가격을 의미하며, `손님`에게 지불 받는 금액이다. |
| 메뉴 이름 | Menu Name | `메뉴`의 이름을 의미한다. |
| 메뉴 상품 | Menu Product | `메뉴`를 구성하는 `상품`들에 대한 정보이다. |
| 메뉴 원가 | Menu Cost | `메뉴`를 구성하는 `메뉴 상품`들의 총 가격으로, `메뉴`를 만드는데 필요한 원가를 의미한다. |
| 메뉴 노출 여부 | Menu Displayed | `손님`이 `메뉴`를 `주문`할 수 있는지에 대한 여부이다. 미노출 `메뉴`는 `주문`할 수 없다. |

### 주문 용어
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | Order | `매장`이 `손님`에게 `메뉴`들을 `판매`하는 방법이다. `손님`들이 `메뉴`들을 주문 한다. |
| 주문 가격 | Order Price | `손님`이 `주문`을 통해 `메뉴`들을 구입하는 가격이다. `주문 메뉴 가격`들의 총합으로 구성된다. |
| 주문 시각 | Order Date Time | `손님`이 `주문`한 시각이다. |
| 주문 유형 | Order Type | `주문`의 특징과 처리 방법을 구분하는 요소이며, 다음의 유형들이 존재한다. (`매장식사`, `배달`, `포장`) |
| 배달 주문 유형 | Delivery Order Type | `주문`한 `메뉴`들을 `배달`을 통해 받는 `주문`이다. |
| 배달 주소 | Delivery Order Type | `손님`이 `배달 기사`를 통해 `배달 주문 유형`의 `주문`을 받을 주소이다. |
| 배달 기사 요청 | Rider Request | `배달 주문 유형`의 `주문`을 `배달`할 `배달 기사`를 요청하는 행위이다. |
| 매장식사 주문 유형 | Eat In Order Type | `손님`들이 `주문`한 `메뉴`들을 `매장`의 `테이블`에 앉아 먹는 `주문`이다.  |
| 포장 주문 유형 | Take Out Order Type | `손님`이 `주문`한 `메뉴`들을 가지고 돌아가는 `주문`이다. |
| 주문 상태 | Order Status | `주문`의 처리 상태/단계이며, 다음의 유형들이 존재하며 `주문 유형`에 따라 조금씩 다른 상태/단계를 가진다. |
| 주문 접수 대기 상태 | Waiting Order Status | `주문`이 들어온 직후의 상태로서, 아직 `주문`을 수락할지 결정 되지 않은 단계이다. |
| 주문 접수 상태 | Accepted Order Status | `주문 접수 대기 상태`의 `주문`을 수락하고 `주문`의 `메뉴`들을 `조리`하는 단계이다. |
| 주문 서빙 상태 | Served Order Status | `주문 접수 상태` `주문`의 `메뉴`들이 모두 `조리` 되면, 그것을 `손님`혹은 `배달기사`에게 제공하는 단계이다. |
| 주문 배달 시작 상태 | Delivering Order Status | `배달 기사`가 `주문 서빙 상태`의 `배달 주문 유형` 주문을 수령하여 `손님`에게 `배달`하기 시작한 단계이다. |
| 주문 배달 완료 상태 | Delivered Order Status | `배달 기사`가 `주문 배달 시작 상태`의 `배달 주문 유형` 주문을 `손님`에게 `배달` 완료한 단계이다. |
| 주문 완료 상태 | Completed Order Status | 모든 `주문 유형`의 `주문`에 대해서 제공이 모두 완료된 상태이다. |
| 주문 메뉴 | Order Line Item | `주문`을 구성하는 `메뉴`들이다. |
| 주문 메뉴 가격 | Order Line Item Price | `손님`이 `주문`을 통해 `메뉴`들을 구입할 때 지불해야 하는 각 `메뉴`의 가격이다. 이 가격은 실제 `메뉴 가격`과 다를 수 있다. |
| 주문 테이블 | Order Table | `매장식사 주문 유형`의 `주문`을한 `손님`이 앉아서 식사를 하는 `테이블`이다. |

### 기타 용어
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 테이블 | Table | `매장식사` `손님`이 식사를 할 수 있는 공간이다. 빈 테이블에는 `손님`들이 앉을 수 있다. |
| 테이블 이름 | Table Name | `테이블`의 이름이다. |

<br>
<br>
<br>

------------------------

## 모델링
### Product
* `Product`는 이름과 가격을 가진다
  * 이름으로 비속어를 쓸 수 없다.
  * 가격은 0원 이상이다.
  * 가격은 `Menu`의 원가를 구성하기 위해 사용된다.
* 새로운 `Product`를 추가할 수 있다.
* 기존 `Product`의 가격을 바꿀 수 있다.
  * `Product` 가격 변경으로 `Menu`원가가 `Menu`가격 보다 비싸지면 `Menu` 미노출 시켜 판매를 중지한다.

### Menu
* `Menu`는 이름, 가격, `MenuGroup`, `MenuProduct`들 그리고 노출여부를 가진다.
  * 이름으로 비속어를 쓸 수 없다.
  * 가격은 원가보다 낮을 수 없다.
  * 가격은 0원 이상이다.
  * 가격은 판매가로 사용된다.
* `Menu`의 이름 규칙과, 가격 규칙을 준수하는 `Menu`를 추가할 수 있다.
* `Menu`의 가격 규칙 내에서 가격을 변경할 수 있다.
* `Menu`를 미노출 시킬 수 있다.
* `Menu`의 가격 규칙을 만족하는 `Menu`만 노출 시킬 수 있다.

### MenuGroup
* `MenuGroup`은 이름을 가진다.
* `MenuGroup`은 `Menu`의 종류를 구별해준다.

### MenuProduct
* `MenuProduct`는 `Product`와 수량으로 구성 되어 있다.
  * 수량은 0개 이상이다.
* `MenuProduct`는 `Menu`의 구성 `Product` 및 수량 그리고 원가를 알기 위해 사용된다.

### Order
* `Order`는 유형, 상태, 일시, `OrderLineItem`을 가진다.
* 손님이 주문한 `OrderLineItem`가격과 `Menu`가격이 다르다면 주문을 받아선 안된다.
* 손님은 `DELIVERY`, `TAKEOUT`, `EAT_IN` 유형의 `Order`를 주문할 수 있다.
* 모든 유형의 `Order`가 들어오면 `WAITING` 상태가 되어 수락을 기다린다.
* 모든 유형의 `WAITING`상태 `Order`는 수락 되어 `ACCEPT` 상태가 된다.

#### DELIVERY
* `DELIVERY` 유형의 `Order`는 배달 주소가 있어야 한다.
* `DELIVERY` 유형의 `WAITING`상태 `Order`이 수락될 때, 배달기사를 요청한다.
* `DELIVERY` 유형의 `ACCEPT`상태 `Order`는 배달기사에게 전달 되고 `SERVED` 상태가 된다.
* 배달기사에게 전달된 `DELIVERY` 유형의 `SERVED`상태 `Order`는 배달이 시작되고 `DELIVERING` 상태가 된다.
* 배달이 시작된 `DELIVERY` 유형의 `DELIVERING`상태 `Order`는 손님에게 전달 되어 `DELIVERED` 상태가 된다.
* 손님에게 전달된 `DELIVERY` 유형의 `DELIVERING`상태 `Order`는 완료 되어 `COMPLETED` 상태가 된다. 

#### TAKEOUT
* `TAKEOUT` 유형의 `ACCEPT`상태 `Order`는 손님에게 전달 되고 `SERVED` 상태가 된다.
* 손님에게 전달된 `TAKEOUT` 유형의 `SERVED`상태 `Order`는 완료 되어 `COMPLETED` 상태가 된다. 

#### EAT_IN
* `EAT_IN` 유형의 `Order`는 빈 `OrderTable`이 있어야 한다.
* `EAT_IN` 유형의 `Order`을 주문하는 손님은 자신의 `OrderTable`에서 여러 `Order`를 주문할 수 있다.
* `EAT_IN` 유형의 `ACCEPT`상태 `Order`는 손님에게 전달 되고 `SERVED` 상태가 된다.
* 손님에게 전달된 `EAT_IN` 유형의 `SERVED`상태 `Order`는 완료 되어 `COMPLETED` 상태가 된다. 
* `EAT_IN` 유형의 `SERVED`상태 `Order`는 완료 되어 `COMPLETED` 상태가 된다. 

### OrderLineItem
* `OrderLineItem`은 주문한 `Menu`, 수량 그리고 주문 메뉴 가격을 가진다.
* 존재하지 않는 `Menu`는 주문할 수 없다.
* 미노출중인 `Menu`는 주문할 수 없다.
* `OrderLineItem`은 손님이 한 번에 주문(`Order`)한 여러 `Menu`들로 구성된다.
* `EAT_IN` `Order`가 아니면 주문 수량은 0개 이상이어야 한다. 

### OrderTable
* `OrderTable`은 이름, 손님의 수 그리고 비었는지 여부를 가진다.
* `OrderTable`을 추가할 수 있다.
* 손님들이 `OrderTable`에 앉을 수 있으며, 이후에도 손님이 더 오거나 떠날 수 있다.
* 손님들이 아직 `OrderTable`에 앉아있지 않더라도 비어있지 않은 테이블로 취급될 수 있다.
* 모든 `Order`가 `COMPLETED`된 `OrderTable`을 정리하여 빈 테이블로 만들 수 있다.

<br>
<br>

## 모델링 질문
### 1. 모델링과 용어집의 차이는 무엇일까요? 
* 모델링은 추상적이던 개념을 코드에서 사용할 이름으로 바꾸는 등의, 코드화에 가까운 개념인가요?
* 그렇다면 모델링의 원래 목적인 `사용자와 개발자가 동일한 언어로 이야기 하기`에 안맞는 것 같은데 맞을까요?
* 만약 코드화에 가깝게 다듬는 과정이 아니면 왜 코드에서 쓸 클래스 이름이 언급이 될까요?
* 이부분을 잘 알아야 모델링이 코드의 라인 바이 라인을 자연어로 서술한 것에 그치지 않을 수 있을 것 같습니다.
  (잘 만들어진 도메인 대로 코드가 구현 되는 것은 맞지만, 코드를 라인 바이 라인으로 자연어로 서술하는 것으론 잘 만들어진 도메인을 만들수 없을테니)

### 2. 모델링 서술과 관련한 질문
```
Product에 있는 내용
-> Product 가격 변경으로 Menu원가가 Menu가격 보다 비싸지면 Menu 미노출 시켜 판매를 중지한다.
```
```
Menu에 있는 내용
-> Menu는 이름, 가격, MenuGroup, MenuProduct들 그리고 노출여부를 가진다.
  가격은 원가보다 낮을 수 없다.
  가격은 0원 이상이다.
  가격은 판매가로 사용된다.
-> Menu의 가격 규칙을 만족하는 Menu만 노출 시킬 수 있다.
```
위의 두 내용을 살펴 보면 `원가보다 비싸게 안파는 메뉴를 노출 시키지 않는 것이 비지니스의 규칙`이고, 이를 유발하는 상황이 두 가지 있습니다.
1. 메뉴 가격을 낮추는 행위
2. 제품 가격을 올려서 원가를 올리는 행위

결과적으로 위의 두 행위가 하나의 비지니스 규칙을 어기게 되는데, 이 규칙이 이미 Menu 관련한 부분에 서술 되어 있다면 Product에서는 저 내용을 또 기술하지 않아도 될지 궁금합니다.

Product에 있는 메뉴 미노출에 대한 내용을 빼더라도 이미 Menu에 원가보다 판매가가 높지 않으면 못판다라고 되어 있으니, 이 모델링을 읽는 사람이 Product에서 일어나는 원가의 변경이 영향을 줄 것이라 생각하여 둘 간의 관계를 파악하지 않을까 라고 생각 합니다.
혹시 이와 관련하여 어떤 의견들을 가지고 계실까요?
