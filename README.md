# 오픈소스 SW 5주차 과제

### 아웃풋을 파일로 다운받기
보통 결과는 스크린으로 나오지만 파일로 다운 받을 수 있다.<br>
**>** : 파일로 저장할 수 있게 해줌 <br>
**>>** : 파일에 다른 내용을 추가할 수 있게 해줌

### 인풋을 파일로 받기
**<** 커맨드를 이용하면 파일에 있는 내용을 인풋 받을 수 있음

### 파이프라인 |
**|** 이 기호는 한줄로 여러 명령어를 처리하고 싶을 때 사용한다
ex) "첫번째 명령 | 두번째 명령" 첫번째 명령에서 나온 아웃풋이 두번째 명령의 인풋으로 들어가게 된다.

### expansion
echo 명령어는 뒤에 나오는 텍스트를 모두 출력해준다 <br>
echo뒤에 와일드카드인 *를 쓰면 현재 작업하고있는 파일들을 출력해준다. <br>
echo는 뒤에 오는 텍스트를 그래도 출력하지 않고 특수기능을 하는 텍스트를 반영하는데 이를 expansion이라고 한다.

### permissions
리눅스는 여러 사람들이 쓰는 시스템이다. 그래서 오류들이 발생할 수 있는데 이를 방지하기위해서 권한을 부여한다.<br>
**-** rwx rwx rwx<br>
owner/group/others<br>
**-** :일반파일을 칭함<br>
d:디렉토리 파일을 칭함<br>
r:Read<br>
w:Write<br>
e:Execution<br>

chmod를 이용하여 권한을 바꿀 수 있음<br>
10진수를 2진수를 변환하여 권환 여부를 따짐
##### ex: chmod 600 -> 110 000 000 owner는 read랑 write를 할 수 있지만 execute는 불가능함 나머지는 다 불가
Superuser: 관리자 모든권한을 가지고 있음<br>
sudo를 이용하여 사용 password를 입력해야됨

### Text Editors
- vi,vim : 처음에 사용하기 어렵지면 익숙해지면 활용성이 높음
- nano : 초보자가 사용하기 적합함
- gedit,kwrite: gui기반하여 cli를 이용할 수 있음

### Shell Script
명령어를 저장하고 한번해 이용할 수 있는 스크립트<br>

### History
내가 이전에 사용했던 커맨드들을 보여줌

### 인터넷에서 사용하는 커맨드
- wget: 인터넷에서 파일을 다운 받을 수 있음
- curl: 내가 원하는 이름으로 인터넷에 있는 파일을 다운 받을 수 있음
- grep: 파일에 있는 택스트를 검색할 수 있음
