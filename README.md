# java-racingcar-precourse

## 세부 구현
### Model
- Car 와 RaceCourse, GameManger를 가진다.
- Car은 canMove 메서드를 통해 현재 이동이 가능한지, 가능하지 않은지 판단한다.
- RaceCourse는 Map<Car,Integer> 타입의 트랙을 가지고 있다.
- GameManger는 Course를 생성하고, 차량을 등록하며, 매 라운드 차량의 위치를 파악할 수 있다.
### View
- Enum인 OutMessage를 통해 문자열을 관리한다.
- 입력 및 출력을 담당하며, 의존성을 가지지 않는다.
- 사용자 입력에 대한 유효성 검사는 Validator 클래스를 통해 Controller에서 이루어진다. View 와 Controller 사이 새로운 로직을 구현하여 분리하는 것도 고려할 수 있다.
### Controller
- View와 GameManager에 의존성을 가진다.
- gameManger가 생성한 결과를 View 에 전달한다.


