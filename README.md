# [프리코스 2주차] 자동차 경주 게임

프로젝트 설명
---
- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.

- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.

- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.

- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.

- 전진하는 조건은 0에서 9사이에서 random값을 구한 후 random값이 4이상일 경우 전진하고, 3이
하의 값이면 멈춘다.

- 자동차 경주게임을 완료한 후 누가 우승했는지를 알려준다.우승자는 한 명 이상일 수 있다.


프로그래밍 요구사항
---
- Car 기본 생성자를 추가할 수 없다.
- name, position 변수의 접근 제어자인 private을 변경할 수 없다.
- setPosition(int position) 메소드를 추가하지 않고 구현한다. 
- 자바 코드 컨벤션을 지키면서 프로그래밍 한다.
- indent depth를 3이 넘지 않도록 구현한다.
- 함수(메소드)의 길이가 15라인을 넘지 않도록 구현한다.
- else 예약어를 사용하지 않는다.
- 축약하지 않고 이름을 통해 의도를 드러내라.
- space와 tab을 혼용하지 않는다.
- 값을 하드 코딩하지 않는다.
- 의미없는 주석을 작성하지 않는다.

기능 구현 목록
---

### 1. Car 클래스 구현
- Position 변수의 setter 메서드를 제외한 기능 구현
- Position 변수 제어 메서드 구현

### 2. 자동차 이름 입력 받기
**입력 받기**
- inputPlayerName() : 자동차 이름 입력 받기
- setPlayerName() : 자동차 이름을 입력 받아 유효값 검사를 마치고 리스트에 담긴 값을 최종값을 리턴 

**유효값인지 검사**
- convertStringNameToArrayList() : 입력 받은 이름을 ,기준으로 나누어 리스트에 담기
- checkPlayerNameLength() : 입력 받은 이름이 5자 이하인지 확인하기

### 3. 자동차 객체 생성하기
- makePlayers() : 입력받은 이름으로 자동차 객체 생성하기

### 4. 게임 횟수 입력 받기
**입력 받기**
- inputMoveCount() : 게임 횟수 입력 받기

**유효값인지 검사**
- checkNumberOrNot() : 숫자가 입력되었는지 확인하기
- checkMoveCountInputOrNot() : 값이 입력되었는지, 입력 값이 0인지 확인하기

### 5. 우승자 파악하기
- judgeWinner() : 우승자 파악하기

### 6. 게임 시작하기
- startRace()

### 7. 우승자 출력하기
- printWinner()
