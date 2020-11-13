注意到当只保留了 $i$ 个食物 $i$ 个老鼠的时候，答案显然就是每个子树的食物 - 老鼠之差的绝对值之和。那么我们维护每个节点的这个差，以及在子树里给某个可行节点进行 $+1$ 能引发的最优贡献，就只需要递归到子树进行更新了。复杂度 $\Theta(m\log n)$。