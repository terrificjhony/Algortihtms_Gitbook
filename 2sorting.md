### 排序的复杂度分析
排序是算法的一个类型，我们设计算法，寻找它的最好最坏情况。在忙着寻找更合适的算法之前，我们也需要去思考一类算法会存在什么样的界限。对于排序算法来说，可以证明，排序的复杂度总是在lg(N!) ~ NlgN之间。

### Computational complexity
对此，我们要引入另一个话题：Computational Complexity.
它主要分析的几个方面是:
1. 分析的主题：如在排序方面，我们可以分析的，是排序算法中使用了多少次比较
2. 分析的方式：在Mergesort这一章节中，我们使用的是二叉树这样的模型来去分析，最终证明，实际上我们最少需要近似与NlgN的时间复杂度，来完成算法的排序
3. 已知的上界：这便是我们之前遇到的问题。
4. 理论的下届：如果它存在，那么我们就可以避免去白费力气。比如，既然我们已经知道排序的霞姐是NlgN,我们就不会再去奢望1/2 NlgN的算法，因为它根本不存在。
5.最优算法。这便是我们在已有的条件中，求考虑，到底存不存在这样的算法，它的时间复杂度与下界的复杂度是相同的。mergesort在排序这一主题下，满足这样的条件。