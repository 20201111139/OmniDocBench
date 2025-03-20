续表
<table border=1><tr>
<td>序号</td>
<td>药名</td>
<td>频次</td>
<td>序号</td>
<td>药名</td>
<td>频次</td>
</tr>


<tr>
<td>8</td>
<td>山药</td>
<td>40</td>
<td>18</td>
<td>柴胡</td>
<td>20</td>
</tr>
<tr>
<td>9</td>
<td>海螵蛸</td>
<td>40</td>
<td>19</td>
<td>生白芍</td>
<td>20</td>
</tr>
<tr>
<td>10</td>
<td>丹参</td>
<td>37</td>
<td></td>
<td></td>
<td></td>
</tr>
</table>另外, 处方药物按类别区分, 频次前 4 位的是: 补虚药 302 频次 (24.65\%), 消食药 163 频次 (13.31\%), 利水祛湿药 118 频次 (9.63\%),理气药 106 频次 \((8.65 \%)\) 。
\section*{2.2 处方中药物组合关联规则 见表 2 。对药物组合出现关联规则进行分析, 支持度个数 23 (在所有药物中同时出现次数)、置信度为 0.95 (若 \(X \rightarrow Y\), 置信度为 \(Y\) 在含 \(X\) 的事物中出现的频繁度)。}
表 2 处方中药物组合关联规则 (置信度 \(>0.95\) )
<table border=1><tr>
<td>序号</td>
<td>规则</td>
<td>置信度</td>
</tr>


<tr>
<td>1</td>
<td>炒白术 $\rightarrow$ 党参</td>
<td>0.97222</td>
</tr>
<tr>
<td>2</td>
<td>甘草, 茯苓 $\rightarrow$ 党参</td>
<td>0.95238</td>
</tr>
<tr>
<td>3</td>
<td>甘草, 炒白术 $\rightarrow$ 党参</td>
<td>0.96666</td>
</tr>
<tr>
<td>4</td>
<td>茯苓, 炒白术 $\rightarrow$ 党参</td>
<td>0.96774</td>
</tr>
<tr>
<td>5</td>
<td>陈皮, 炒白术 $\rightarrow$ 党参</td>
<td>0.96969</td>
</tr>
<tr>
<td>6</td>
<td>甘草, 茯苓, 炒白术 $\rightarrow$ 党参</td>
<td>1.96153</td>
</tr>
<tr>
<td>7</td>
<td>甘草, 陈皮, 炒白术 $\rightarrow$ 党参</td>
<td>096428</td>
</tr>
<tr>
<td>8</td>
<td>陈皮, 茯苓, 炒白术 $\rightarrow$ 党参</td>
<td></td>
</tr>
<tr>
<td>9</td>
<td>甘草, 陈皮, 茯苓, 炒白术 $\rightarrow$ 克参</td>
<td></td>
</tr>
</table>\section*{2.3 基于摘聚类的方剂组方规律分析}
2.3.1 基于改进的互信息法的药物间关联度分析 见表 3 。依据方剂数量, 结合经验判断和不同参数提取数据的预读, 设置相关度为 8 , 惩罚度为 5 , 进行聚类分析, 得到方剂中两两药物间的关联度。