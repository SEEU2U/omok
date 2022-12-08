파이썬으로 오목 구현
====================

1.설명
------
제가 구현한 것은 오목입니다.   
   
> 오목은 두 사람이 번갈아 돌을 놓아 가로나 세로, 대각선으로 다섯 개의 연속된 돌을 먼저 만들면 승리하는 게임입니다.
>
> 각 플레이어는 흑돌과 백돌중 하나를 선택해서 게임을 수행합니다.
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
>> 3이 동시에 두 개가 발생하여 상대편이 한 쪽을 막아도 다른 쪽으로 열린 4를 만들수 있는 경우에 해당한다.
>>  
>> ### 4 - 4
>>
>> 4가 동시에 발생하는 경우에 해당한다.
>>   
>> ### 장목
>> 6개 이상으로 연속된 돌을 둘 경우에 해당한다.
>
> 저는 파이참을 이용해서 파이썬을 사용해 오목을 구현하였습니다. 사용되는 이미지중 일부는 아래에 표기한 출처에서 가져와 가공하였고 일부는 직접 제작했습니다. GUI구현을 위해서 pygame 라이브러리를 사용했습니다.

2.게임 구현 설명
----------------

## 1.메인 메뉴

![image](/project/Images/markdown/main.PNG)

## 2. 게임설명

![image](/project/Images/markdown/explain.PNG)

## 3. 플레이어 수 , 선/후공 선택

![image](/project/Images/markdown/player.PNG)

![image](/project/Images/markdown/select_color.PNG)

## 4. 게임화면


![image](/project/Images/markdown/play.PNG)

![image](/project/Images/markdown/victory.PNG)




-----------------------------------------

출처

code : https://github.com/kulord99/Othello

font : https://cooltext.com/Logo-Design-Fun
