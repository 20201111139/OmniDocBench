项目4 综合应用

续表
<table>
<thead>
<tr>
<th>序号</th>
<th>监控内容</th>
<th>连接变量</th>
<th colspan="2">输入 值</th>
<th colspan="2">输出值</th>
</tr>
<tr>
<th></th>
<th></th>
<th></th>
<th>数值类型</th>
<th>数值范围</th>
<th>数值类型</th>
<th>整数位数</th>
<th>小数位数</th>
</tr>
</thead>
<tbody>
<tr>
<td>3</td>
<td>操作值</td>
<td>MV</td>
<td></td>
<td></td>
<td>模拟量输出</td>
<td>3位</td>
<td>2位</td>
</tr>
<tr>
<td>4</td>
<td>手动设定值</td>
<td>SP_man</td>
<td>模拟量输入</td>
<td>0~100</td>
<td>模拟量输出</td>
<td>3位</td>
<td>2位</td>
</tr>
<tr>
<td>5</td>
<td>PID 比例系数</td>
<td>PIDO_P</td>
<td>模拟量输入</td>
<td>0~100</td>
<td>模拟量输出</td>
<td>3位</td>
<td>2位</td>
</tr>
<tr>
<td>6</td>
<td>PID 积分时间</td>
<td>PIDO_I</td>
<td>模拟量输入</td>
<td>0~100</td>
<td>模拟量输出</td>
<td>3位</td>
<td>2位</td>
</tr>
<tr>
<td>7</td>
<td>PID 微分时间</td>
<td>PIDO_D</td>
<td>模拟量输入</td>
<td>0~100</td>
<td>模拟量输出</td>
<td>3位</td>
<td>2位</td>
</tr>
<tr>
<td>8</td>
<td>控制方式</td>
<td>MAN_on</td>
<td>离散值输入</td>
<td>0或1</td>
<td>离散值输出</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

实时趋势曲线

| 曲线定义 | 标识定义 |
|---|---|

标识轴——时间轴
标识Y轴——数值轴

<table>
<thead>
<tr>
<th>数值轴</th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td>标识数目</td>
<td>3</td>
<td>起始值</td>
<td>0</td>
<td>最大值</td>
<td>100</td>
</tr>
<tr>
<td>整数位位数</td>
<td>3</td>
<td>小数位位数</td>
<td>2</td>
<td>厂科学计数法</td>
<td>字体</td>
</tr>
<tr>
<td>数值格式</td>
<td>●工程百分比
○实际值</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th>时间轴</th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td>标识数目</td>
<td>3</td>
<td>格式:</td>
<td>年月日时分秒</td>
</tr>
<tr>
<td>更新频率:</td>
<td>1 秒 分</td>
<td>字体</td>
</tr>
<tr>
<td>时间长度:</td>
<td>30 秒 分 时</td>
<td></td>
</tr>
</tbody>
</table>

确定 取消

图4.75 实时趋势曲线标识定义——————设置坐标轴

液位PID控制

手动设定值######
设定值:######
测量值 ######
操作值: ######

比例系数 ######
积分时间:######
微分时间 ######
控制方式 ######

自动方式
手动方式
启动变频器
停变频器

图4.76 监控主界面

134
