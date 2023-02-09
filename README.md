# GraphTheory

[그래프이론](https://datascienceschool.net/03%20machine%20learning/17.01%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EC%9D%B4%EB%A1%A0%20%EA%B8%B0%EC%B4%88.html)



<img src="img/networkX.png" height="200" width="400"> 


Centrality 
- 전체 연결망에서 중심에 위치하는 정도를 표현하는 지표.
    

중심성 지표:
* Degree Centrality
    텍스트에서 단른 단어와 동시 출현 빈도가 많은 특정 단어는 연결 중심이 높다
    연결 중심성 계산 수식
        $$ degree_{ik} = \sum_{i=1}^{N} Z_{ijk} = Z_{jk}$$
        $$ outdegree_{ik} = \sum_{j=1}^{N} Z_{ijk} = Z_{ik} $$
        $$ C_{i} = \sum_{j=1}^{n}(Z_{ij}+Z_{ji}) / \sum_{i=1}^{n}\sum_{j=1}^{n}(Z_{ij})\qquad단, 0\le C \le 1$$
* Eigenvector Centrality 
    연결된 상대 단어의 중요성에 가중치
    중요한 단어와 많이 연결됐다면 위세 중심성이 높아짐
    $$ P_i =\sum_{j=1}^{N-1}P_iZ_{ji},\qquad0 \le P_i \le 1$$                    
* Betweeness Centrality
    