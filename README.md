# 책임주도개발 연습 단계
1. 사용자에게 제공해야하는 기능인 시스템 책임을 파악한다.
2. 더 작은 책임으로 분할한다.
3. 분할된 책임을 수행할 수 있는 적절한 객체 또는 역할을 찾아 책임을 할당한다.
4. 다른 객체의 도움이 필요한 경우 이를 책임질 적절한 객체 또는 역할을 찾는다.
5. 해당 객체 또는 역할에게 책임을 할당함으로써 두 객체가 협력하게 한다.
---
# 문자열 사칙 연산 계산기
1. 사용자에게 제공해야하는 기능인 시스템 책임을 파악한다.
- 입력받은 문자열 계산식을 수행하여 결과값을 알려준다.

2. 더 작은 책임으로 분할한다.
- 입력받은 문자열 계산식을 숫자와 연산자로 분리한다.
    - 입력받은 문자열 계산식이 정상인지 판단한다.
- 계산한다.
    - 연산자 우선순위가 아닌 입력받은 순서대로 계산한다.
- 결과를 반환한다.
    - 문자열 값으로 결과를 반환한다.

3. 분할된 책임을 수행할 수 있는 적절한 객체 또는 역할을 찾아 책임을 할당한다.
- StringCalculator : 입력받은 문자열 계산식을 계산한다.
 
---
# 자동차 경주 게임
## 진행 방법
* 자동차 경주 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## 기능 요구사항
* 주어진 횟수동안 n대의 차동차는 전진/멈춤을 반복한다.
    * 사용자가 횟수와 자동차 수를 입력한다.
* 전진조건 : 0~9 사이 랜덤값을 구한 뒤 4보다 크거나 같은 경우 (number >= 4 전진.  number < 4 멈춤.)
* 자동차 상태를 화면에 출력. 출력시점의 제약 없음

## 책임정리
1. 사용자에게 제공해야하는 기능인 시스템 책임을 파악한다.
* 자동차 레이싱 게임을 진행하여 결과를 보여준다.

2. 더 작은 책임으로 분할한다.
* 입력 = 자동차 수, 반복횟수
* 출력 = 횟수별 자동차 위치결과

* 레이싱 게임을 진행한다.
    * 전진 / 멈춤을 정한다.

* 횟수별 결과를 저장한다. 

3. 분할된 책임을 수행할 수 있는 적절한 객체 또는 역할을 찾아 책임을 할당한다.
4. 다른 객체의 도움이 필요한 경우 이를 책임질 적절한 객체 또는 역할을 찾는다.
5. 해당 객체 또는 역할에게 책임을 할당함으로써 두 객체가 협력하게 한다.