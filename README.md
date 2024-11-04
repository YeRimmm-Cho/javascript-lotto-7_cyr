# javascript-lotto-precourse
## 로또
### 기능 목록

#### 1. 구입 금액 입력 및 검증
- 사용자가 입력한 금액을 검증하고, 1,000원 단위로만 입력이 가능하도록 예외 처리를 한다
- 1,000원 단위로 금액을 입력하지 않을 경우 "[ERROR]"로 시작하는 에러 메시지를 출력하고 재입력받는다

#### 2. 로또 번호 생성
- 사용자가 입력한 금액에 따라 구매 가능한 로또 개수를 계산하여 생성한다
- 각 로또는 1~45 사이의 중복되지 않는 숫자 6개로 구성되고, 번호는 오름차순으로 정렬한다
- 로또 번호는 `MissionUtils.Random.pickUniqueNumbersInRange(1, 45, 6)` 메서드를 이용하여 생성한다

#### 3. 발행된 로또 번호 출력
- 발행된 로또 수량과 각 로또 번호를 오름차순으로 출력한다

#### 4. 당첨 번호 및 보너스 번호 입력
- 사용자가 입력한 당첨 번호 6개와 보너스 번호 1개를 입력받아 저장한다
- 당첨 번호와 보너스 번호는 중복되지 않아야 하며, 1~45 범위 내에서 입력해야 한다
- 입력된 번호가 잘못된 값이면 "[ERROR]"로 시작하는 에러 메시지를 출력하고 재입력받는다

#### 5. 당첨 결과 계산
- 구매한 로또 번호와 당첨 번호를 비교하여 일치하는 개수를 확인한다
- 일치하는 개수와 보너스 번호 일치 여부에 따라 1등부터 5등까지의 당첨 결과를 계산한다

#### 6. 당첨 내역 및 수익률 계산
- 각 등수별로 당첨된 로또 개수를 출력한다
- 총 당첨금과 수익률을 계산하여 출력한다
- 수익률은 소수점 둘째 자리에서 반올림하여 출력한다

#### 7. 예외 상황 처리
- 입력 값이 잘못됐을 경우 "[ERROR]" 메시지를 출력하고 해당 지점부터 재입력받는다

