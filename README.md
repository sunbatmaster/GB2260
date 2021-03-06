# 中华人民共和国行政区划代码（GB/T 2260)
> 英文名为 Codes for the administrative divisions of the People's Republic of China

仅收录县级以上部分，即 6 位代码。按照标准，6 位数字代码，包含三级地理信息。
> 代码从左至右的含义是：<br>
> 第一、二位表示省（自治区、直辖市、特别行政区）。<br>
> 第三、四位表示市（地区、自治州、盟及国家直辖市所属市辖区和县的汇总码）。<br>
> 第五、六位表示县（市辖区、县级市、旗）。<br>

数据来源：[中华人民共和国民政部->民政数据->行政区划代码](http://www.mca.gov.cn/article/sj/xzqh/2019/)

## 本库特点：含逐年变更历史
该来源提供了1980年来每年的版本。由于历年的更新，会有部分代码在后续版本中不再出现。而这部分代码在当年颁发的证件中已被编码使用，所以还有查询的需要。
当前 (201908) 在 github 上找到的几个开源库，均不支持不同年份的代码。特别整理这两个文件。截止到2019年6月的数据均已采集。

## 使用说明
`code_year_region.csv` 分三列：`code`,`year`,`region`

`code_year_region.json` 结构为：`{"code":{"year":"region", ...}, ...}`

可通过取前 2, 4, 6 位，余位补 0 的形式 (xx0000, xxxx00, xxxxxx) 查询各级地理信息。
