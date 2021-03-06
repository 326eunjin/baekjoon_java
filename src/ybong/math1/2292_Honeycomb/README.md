# 벌집
# Problem
![image](https://user-images.githubusercontent.com/75327385/139776561-476b3ae2-c29c-4d62-bbf1-6a31cfc2ffea.png)

위의 그림과 같이 육각형으로 이루어진 벌집이 있다. 그림에서 보는 바와 같이 중앙의 방 1부터 시작해서 이웃하는 방에 돌아가면서 1씩 증가하는 번호를 주소로 매길 수 있다. 숫자 N이 주어졌을 때, 벌집의 중앙 1에서 N번 방까지 최소 개수의 방을 지나서 갈 때 몇 개의 방을 지나가는지(시작과 끝을 포함하여)를 계산하는 프로그램을 작성하시오. 예를 들면, 13까지는 3개, 58까지는 5개를 지난다.

제한시간: 2초

## Input
첫째 줄에 N(1 ≤ N ≤ 1,000,000,000)이 주어진다.

## Output
입력으로 주어진 방까지 최소 개수의 방을 지나서 갈 때 몇 개의 방을 지나는지 출력한다.

---
# Example
|입력|출력|
|:-|:-|
|13|3|
|58|5|
  
# Tag
`mathematics`

---
# Solution
![image](https://user-images.githubusercontent.com/75327385/139777112-4a951e04-1f83-437e-8b72-35671026f805.png)
- 벌집 한 칸마다 멤버 갯수가 6의 배수로 늘어난다. 
- 해당 칸만큼이 1과의 거리가 된다. 
- 따라서 
  - 첫째줄은 7까지
  - 둘째줄은 19까지 (7 + (6*2))
  - 셋째줄은 37까지 (19 + (6*3))
    ...
- 입력 숫자가 몇번재 줄에 위치하는 지 알아내고, 번째 +1이 답이다. 
