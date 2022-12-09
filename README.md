파이썬으로 오목 구현
====================

1.설명
------
제가 구현한 것은 오목입니다.   
   
> 오목은 두 사람이 번갈아 돌을 놓아 가로나 세로, 대각선으로 다섯 개의 연속된 돌을 먼저 만들면 승리하는 게임입니다.
>
> 각 플레이어는 흑돌과 백돌 중 하나를 선택해서 게임을 수행합니다.
>
> 흑돌을 선택한 플레이어가 선공을 합니다.
>
> 여기서는 렌주룰을 적용합니다.
>>
>> ## 렌주룰
>>
>> 3 - 3 , 4 - 4 , 장목은 백돌만 허용합니다.
>>
>> ### 3 - 3
>> 
>> 3이 동시에 두 개가 발생하여 상대편이 한 쪽을 막아도 다른 쪽으로 열린 4를 만들 수 있는 경우에 해당한다.
>>  
>> ### 4 - 4
>>
>> 4가 동시에 발생하는 경우에 해당한다.
>>   
>> ### 장목
>> 6개 이상으로 연속된 돌을 둘 경우에 해당한다.
>
> 저는 파이참을 이용해서 파이썬을 사용해 오목을 구현하였습니다. 사용되는 이미지 중 일부는 아래에 표기한 출처에서 가져와 가공하였고 일부는 직접 제작했습니다. GUI 구현을 위해서 pygame 라이브러리를 사용했습니다.

2.게임 구현 설명
----------------

### 1.메인 메뉴

![image](/project/Images/markdown/main.PNG)

Main Menu는 

- `START`
- `EXPLAIN`
- `TURN OFF`

세 가지 버튼으로 구성되어 있습니다.

`START`를 누르면 1P, 2P 플레이어의 수를 선택하는 창으로 이동합니다.
`EXPLAIN`를 누르면 게임 설명으로 이동합니다.
`TURN OFF`를 누르면 프로젝트는 종료됩니다.

### 2. 게임설명

`EXPLAIN`를 누르면 다음 창이 뜹니다.

![image](/project/Images/markdown/explain.PNG)

`BACK`을 누르면 MainMenu 창으로 이동합니다.

### 3. 플레이어 수 , 선/후공 선택

`START`를 누르면 다음 창이 뜹니다.

![image](/project/Images/markdown/player.PNG)

- `1P`
- `2P`

`1P`를 누르면 선공(흑돌) , 후공(백돌)을 선택하는 창으로 이동합니다.

`2P`를 누르면 게임 창으로 바로 이동합니다.

`1P`를 누르면 다음 창이 뜹니다.

![image](/project/Images/markdown/select_color.PNG)

- `흑돌로플레이`
- `백돌로플레이`

`흑돌로플레이`버튼을 누르면 선공으로 게임을 시작합니다.

`백돌로플레이`버튼을 누르면 후공으로 게임을 시작합니다.

`2P`를 누르면 게임 화면 창이 뜹니다.

### 4. 게임화면

![image](/project/Images/markdown/play.PNG)

- `SKIP TURN`

`SKIP TURN`을 누르면 차례가 넘어갑니다.

해당 화면은 게임 시작 후 선공, 후공이 각각 한 번씩 둔 이후의 화면입니다. 

오른쪽 위는 현재 누구의 차례인지 표시해 줍니다.

마우스 커서를 판위에 올려놓으면 현재 차례의 플레이어의 돌이 표시됩니다.

렌주룰에 따라 흑돌은 3-3, 4-4, 장목을 판에 클릭하더라도 돌을 두지 못합니다.

룰을 따르고 두고자 하는 위치 위에 클릭을 하면 돌이 놓아지고, 차례가 바뀌어서 돌의 색이 바뀝니다.

플레이어의 경우 돌을 놓을 곳이 없으면 `SKIP TURN`버튼을 눌러 차례가 넘어가게 됩니다.

CPU의 경우 자동으로 턴이 넘어갑니다.

![image](/project/Images/markdown/victory.PNG)

플레이 후에 이겼을 경우 위의 화면처럼 이긴 플레이어의 돌을 보여줍니다.

시간이 지나면 자동으로 시작 화면으로 돌아갑니다.

-----------------------------------------

출처

code : https://github.com/kulord99/Othello

font : https://cooltext.com/Logo-Design-Fun
