T-share
======
* we aim to minimize the increased travel distance for each individual query $Q$
* it does not guarantee that the total travel distance of all taxis for all queries is minimized.
* 将路网划分，使用pre-calculated最短路来节省计算时间，但是travel time的计算不是很严谨
* 利用anchor node 代表网格中的所有节点
* 从O和D进行双向选择，选择标准就是时间和空间的距离

