Thunder本のmctsをscore4用に改変しました。  
selfplayでリーチの対処をするようにしただけでかなり強くなりました。  
現行のalpha beta法によるAIに対する勝率は50%を超えています。  
mctsはroot並列化してあります。  
tree並列化はまだできていません。  

Human_v_AI関数の`think_time`で思考時間を変更可能  
mctsActionBitWithTimeThresholdParallel関数の`THREAD_NUM`でmctsのselfplayの並列化数を指定可能  

```
g++ mcts2.cpp -o mcts
```
