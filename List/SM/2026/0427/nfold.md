---
layout: post
---
# n-Fold Way

만약 표현이 서로 달라도 동일한 물리를 기술한다면 다 같은 해석으로 묶을 수 있으니 편할 테니 보통 그런 기대를 품고 duality를 찾는데, 물리에서 duality나 correspondence라는 이름이 붙은 것들이 꽤 여러가지 있고 그중 하나가 state-observable duality이다. 애초부터 measure를 선택하고 확률의 의미를 해석하고 typical한 상태를 가정하고.. 이딴 걸 굳이 머리아프게 하지 말고 그냥 그 measure를 주는 구조 자체만 딱 정의하고 싶다는 데서 시작한다.

시스템에 대해 아는 정보가 하나도 없는 상태를 기준으로 해서 여기에 연산을 작용하면 특정한 mixed state들을 얻고(e.g. Bloch sphere) 그런 상태들을 다루는 density matrix를 만드는데, 그 state가 observable에 확률을 부여해주는 linear functional인 것이고, 거기서 state space와 observable space를 '식별'하는 방법이 (trace와 inner product를 도입해서 만들어지는) 관계식으로 주어지고 그런다.

그렇게 했을 때 가능한 algebra를 분류하면 물리적으로 유효한 observable의 체계가 실수, 복소수, 사원수, 3차원 팔원수, spin factor밖에 없다. Stone's theorem은 시간 병진 대칭성을 양자 상태에 적용했을 때 (계의 에너지에 대응하는) 해밀토니안 연산자와 unitary one-parameter group의 bijection이 있다는 정리인데 이게 성립하려면 generator가 self-adjoint obsevable이 돼야 해서 허수가 필요하기 때문에 실수 체계에서는 구성이 불가능하고, 사원수 체계에서는 anticommutativity 때문에 linearity가 깨진다. 그런데 이걸 복소수 힐베르트 공간 위의 대칭군으로 옮기면 그 위에서 작용하는 군의 irreducible representation H가 딱 세 개로 나뉘는데, H가 자기 자신의 dual space와 동형이 아니면 complex고 unitary다. 동형이면서 unitary operator가 있는데 그 operator의 제곱이 1이면 real이고 orthogonal이다. 그 제곱이 -1이면 quaternion이고 symplectic이다. 이걸 Dyson의 3-fold way라고 부른다.

[Gaussian ensemble](https://en.wikipedia.org/wiki/Gaussian_ensemble)

: Dyson은 이걸 이용해서 해밀토니안의 대칭성을 모델링하는데, random matrix들을 모은 앙상블을 저 unitary, orthogonal, symplectic 세 가지로 나눴다. 이 앙상블이 주로 large N limit을 다룰 때 계산하는 데 활용된다.
파인만 다이어그램에서 1/N의 거듭제곱 급수로 asymptotic expansion 하는데 여기서 전개되는 모델이 SO(N), SU(N), Sp(2N) 이고 그게 저 세 가지 gaussian ensemble과 연결된다.

​
시간 병진 대칭에 대해서만 하던 걸 CPT 대칭성으로 확장한 게 10-fold way인데 그게 끈이론의 worldsheet에 fermion mode 추가한 초끈이론이나 위상 절연체 쪽 다루는 응집물리에서 쓰인단 말이 써있다. 아직은 topological K-theory를 건드리기엔 아직 때가 한참 아닌 거 같다.

-----
[Ten-Fold Way](https://ncatlab.org/nlab/show/ten-fold+way)
[The Three-Fold Way Part I](https://golem.ph.utexas.edu/category/2010/12/division_algebras_and_quantum.html)
[The Three-Fold Way Part II](https://golem.ph.utexas.edu/category/2010/12/the_threefold_way_part_2.html)


<div class="pagination">
  <a href="{{ '/List/SM/sm.html' | relative_url }}" class="prev-button" data-turbo="true">목록</a>
</div>