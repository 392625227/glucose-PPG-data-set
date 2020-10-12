# glouse-PPG-data-set-
This data set records the blood glucose and PPG data at the same time, trying to find the relationship between them with CNN, and try to detect blood glucose continuously and noninvasively with PPG! 
这个数据集同时记录了血糖值和PPG 数据， 试图用CNN找到他们之间的关联关系，尝试基于PPG的无创连续检测血糖！

The blood glucose reading is from a micro invasive dynamic blood glucose detector on the market. It has a sensor and a very small electrode inserted into the skin about 5mm. It works continuously for 14 days to read the blood glucose data and update the data every 2 minutes. It can read real-time blood glucose data with mobile app.
血糖读数来自于一款上市的微创动态血糖检测仪，他有一个传感器，有一个很细小的电极插入皮肤5mm左右，连续工作14天读取血糖数据，每隔2分钟更新一次数据。可以用手机APP读取实时的血糖数据。

The PPG (photo plethyamo graph) reading comes from the development board of a pulse oximeter based on PPG. PPG is widely used in pulse oximeter on the market to test blood oxygen content. Many watches and bracelets also use the PPG method to measure pulse rate and blood oxygen. This method is completely noninvasive, and can obtain ideal results in a few seconds, which is very convenient.At the same time, the price is very low. The simple pulse oximeter only needs 100-200 RMB (about 20-30 USD).
PPG（Photo Plethyamo Graphy）读数来自于一台基于PPG的脉搏血氧仪的开发板。市场上的脉搏血氧仪普遍使用PPG来实现血氧含量的测试。很多手表和手环测量脉率和血氧也是用PPG方法。这个方法完全无创，而且几秒内就能获得理想的结果，非常方便。同时价格非常低，单纯的脉搏血氧仪大约只要100-200RMB（约20-30USD）。

However, most people still use blood glucose meters with punctured fingers to test blood sugar. The Chinese idiom says that ten fingers are linked to one heart! If it is punctured several times a day, it is also a painful thing. There are very few manufacturers on the market, can prick a needle, continuous use of 14 days of probe, can continuously read blood glucose value, very convenient. But the price is relatively high, about 300-400RMB (40-60USD) for a probe, 8100-10800RMB (1080-1620USD) a year. Diabetes is a chronic disease for a long time, and many people can't afford such high expenses.
然而测试血糖目前大部分人还是使用扎破手指的血糖仪，中国的成语说十指连心啊！如果一天扎破好几次也是比较痛苦的事情。有非常少的几个厂商上市了可以扎一次针，连续使用14天的探头，可以连续的读取血糖值，十分方便了。但是价格是比较高的，大约一个探头300-400RMB(40-60USD), 一年要8100-10800RMB(1080-1620USD)。糖尿病是长期的慢性病，很多人是难以承受如此高的支出。

The goal of this paper is to use a fast and inexpensive PPG method to test blood glucose. There are some papers tried by some university research institutions on the Internet, but it is difficult to obtain a large number of valid data. This paper is an open data set, and its data format is described as follows: each data file contains about 30KB of sampling data, which is composed of n * 17 data packets. Each data packet starts with 11551155 and is followed by 16 numbers. Even number is IR light intensity, and odd number is led light intensity. In fact, the sampling of each data packet starts from the lowest point of heart rate waveform, and the light intensity is sampled every 2ms
本文的目标就是希望用快速并且廉价的PPG 方法测试血糖。网上有一些大学研究机构尝试的论文，但是很难获得大量的有效数据。本文是开放的数据集，其数据格式说明如下：每个数据文件大约包括30KB的采样数据，由N x 17个数据包组成，每个数据包以11551155开头后面有16个数字，偶数是IR光强，奇数是LED光强。其实每个数据包的采样是从心率的波形的最低谷开始，每2ms采样一次光强数字。



