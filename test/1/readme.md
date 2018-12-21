소장님과 함께하는 즐거운 연구 



12/21 금요일

Things to do : 

1. 수렴되는 그래프 뽑기 (뽑아지기를 기대하기)
   1.1 안될경우 혹은 기존 DQN보다 낮은 경우 -> Resolution을 줄여주는 것을 고려할것



현재 모델 : 



<img src="https://www.dropbox.com/s/zyqzozfabh9wnow/Screenshot%202018-12-21%2019.10.33.png?raw=1">







5일 학습 후 :



1. <img src="https://www.dropbox.com/s/bzyv92x6jcvwahm/Screenshot%202018-12-21%2018.43.59.png?raw=1">

1. 동영상 

[![](http://img.youtube.com/vi/HVIlETiJ8a0/0.jpg)](http://www.youtube.com/watch?v=HVIlETiJ8a0 "")



문제점 : 

1. 5000000 time step 정도즘 성능이 매우 좋아진 뒤
2. 학습을 더 하게 되면 성능이 떨어진다. 
3. 학습을 잘 하지 못한다. 



생각 : 



사람을 배우면 배울수록 세밀하게 컨트롤 하며 decision making을 하는데, 마리오도 그렇지 않을까? 

결국은 매 time step마다 action을 선택하게 하는것이 좋은 방법이 아닐까? 



<img src="https://www.dropbox.com/s/oh2mad82mzsrgxf/Screenshot%202018-12-21%2019.09.03.png?raw=1">





다음주 바꿔볼 부분 : 

1. 처음에는 omega network를 통하여 같은 action을 선택하는 작업을 많이 한다.

2. 학습을 계속 하면 할수록 그 횟수가 줄어들게 한다 ( decay 와 같이 )




<img src="https://www.dropbox.com/s/50ldive3m1pa6t4/Screenshot%202018-12-21%2019.10.59.png?raw=1">







회의 끝 



<img src="https://www.dropbox.com/s/2kwh8wvicjlm3od/Screenshot%202018-12-21%2020.56.06.png?raw=1">





원석 Things to do :

1. 고민할것 : 왜 갑자기 reward가 떨어지지? 
2. 그 전에: 
   일단 초반에 생각하였던 resolution exploration decay  하는 방법 
   2.1일반 DQN에서 action 반복하는 횟수만 decay시키기
   2.2 예를 들어 action 반복이 1~10에서 선택된다고 할때 
   2.3  처음에는 1~10부터
   1~9,1~8,1~7.... 1 까지 학습이 되면 될수록 그 반복 acrtion space가 줄어들게 한다. 
   2.4 마리오 말고 다른 아타리에다가 적용해볼것 


혜령 Things to do: 

1. 논문 마저 읽어오기 
2. 다음주면 다 까먹을 원석이에게 다시 설명해주기 

