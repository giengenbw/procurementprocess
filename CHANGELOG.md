# Changelog

## 2026-11-23 - Round 5

### Added
- ME21N 手工订单、BANF/合同引用、估价和项目级预付款。
- 退货、计划交付、带交货的库存调拨和 Intercompany 判断。
- ME57 供应源分配、BANF 合并转订单和 DOM 输出。
- ME2ON 委外供料、MMBE 外部库存检查和 VL02N 发货。

## 2026-11-23 - Round 4

### Added / Updated
- 用 BANF PDF 增强 ME51N：Kontierungstyp K/Q、Kostenstelle、PSP-Element、负责人、特殊底盘备件与供应商可见文本。
- 新增 Bestellbestätigungsmonitor：首次 AB、后续改期、统计交期、批量复制、分批交货拆分和 ME23N 验证。
- 新增 ME5A 按创建人查询 BANF 及 Freigabekennzeichen。

### Pending verification
- `/JA41/_BBEST` 是否为当前可直接执行的自定义事务代码。
- 开放收货量复选框与“排除部分交货项目”描述的矛盾。
- 历史特殊材料 1091346、1091347、MB-02 的当前有效性。

## 2026-11-23 - Round 3

### Added
- ME51N 创建 BANF；ME52N/ME53N 修改和显示 BANF。
- ME*x* 采购清单、ME2L/WE101 开放订单、ME80FN 交期对比。
- MC$4 供应商采购金额、数量偏差和交期偏差分析。
- MM01/MM02 扩展 MRP 区域，MD04 区域库存需求和 MRP 检查。

### Pending verification
- Stat.Lieferdatum 与真实 MIGO 收货日期的口径。
- Sonderbeschaffung 45 和 MRP 运行参数的当前 Customizing。
- WE101/WE103 历史重复选择参数在当前系统的区别。

## 2026-11-23 - Round 2

### Added
- 冻结重复供应商并设置删除标识。
- 替代订购地址 BA 与替代开票方 RS。
- ME41 创建/复制询价，ME42/ME43 修改与显示。
- ME47/ME48 录入与显示报价，ME49 报价比较。

### Pending verification
- 重复供应商资料未提供明确事务码和具体截图字段，XK02/MK02 需在当前系统确认。
- M-06/M-04 的伙伴角色与 6xxx/4xxx 编号范围在原期资料中尚未激活，需确认当前配置。
- 未知交期使用 31.12.2099 的历史做法需与当前报表和自动化规则核对。

## 2026-11-23

### Added
- 建立销售、VC、PDM 三个业务域的流程知识库。
- 新增流程级 Markdown、Mermaid 流程图、字段表、检查清单。
- 新增可复用更新提示词。

### Notes
- 来源资料为 2017-2019 年历史培训文件，当前 SAP 字段、组织值和权限需验证。
- 原始资料中的空白、未完成段落和疑似笔误没有被当作已确认事实补齐。
