# javascript-racingcar-precourse

## 요구사항

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 "[ERROR]"로 시작하는 메시지와 함께 Error를 발생시킨 후 애플리케이션은 종료되어야 한다.

## 구현할 기능 목록

- 입력 폼을 구현
  - 쉽표를 기준으로 구분하여 자동차 입력받기
    - 해쉬맵으로 구현한다.
  - 시도할 횟수를 입력
- 경주게임 구현
  - 0-9의 무작위 숫자 얻기
  - 진행상황 출력
    - 입력된 자동차 순서대로 출력
  - 우승자 출력
    - 공동우승자는 입력 순서대로 출력
      - ,로 구분
    - 만약 우승자가 없다면, 우승자가 없다고 출력
- 예외, 오류
  - 자동차 이름
    - 6글자이상이거나 빈글자는 오류
    - 대소문자를 구분한다.
    - 중복된 이름은 오류 처리
    - 영어로된 이름이어야 한다.
  - 시도횟수
    - 1이상의 숫자만 가능
    - 0또는 빈숫자, 숫자 이외의 입력은 오류처리
