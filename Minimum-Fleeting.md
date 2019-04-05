Quantifying
======
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
- the shareability parameter $k$: the maximum number of trips that can be shared
- the maximum time delay the passenger can tolerate in a shared trip $\Delta$
- can be shared - the travel time between intersections - ad hoc heuristic
- tractable for $k=2$, heuristically feasible for $k=3$
- $k=2$: equivalent to the maximum amtching problem 
- $\Delta = 10min $, 150 million nodes and 100 billion links
- Oravle model, an artificial scenario, an upper bound
- 但是现在这样都是在你已经知道所有时间点的请求之后得出的结果，在实际中这是不可能做到的，我们不可能知道未来的结果
- $\delta$: 在寻求实时的基础上给予一定的放松，允许我们可以知道未来$\delta$时间内的请求，这样增添了灵活性，但是$\dekta$自然不能太大
- In dynamic approaches to taxi sharing however, in which taxis are allowed to re-route and to pick up new passengers on the fly, the concrete operational issues of the detailed spatial query setup and the communication protocol design between taxis and dispatch system becomes potentially intricate. This set of problems has been satisfactorily solved by a recently published service model called T-share。 the study has pointed out the impressive potential of a heuristic, dynamic approach, and has provided efficient and scalable algorithms to solve the taxi searching and scheduling sub-problems which occur when taxis are allowed to change their routes on the fly.
- 将od投影到intersection
- Traavel time estimation
    - 先将具有相同OD的放到同一集合，用一个代表元代表集合，用平均travel time 代表
    - 对于一个trip中的od利用Dijlstra算法计算travel time
    - 
