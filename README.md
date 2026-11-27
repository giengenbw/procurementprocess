# SAP Procurement & Enterprise Process Knowledge Base

<p align="center">
  <strong>企业级 SAP 业务流程知识库</strong><br>
  <sub>Process Documentation · Transaction Index · Operational Reference</sub>
</p>

<p align="center">
  <img alt="Documentation" src="https://img.shields.io/badge/Docs-Markdown-0A66C2?style=flat-square">
  <img alt="Process-oriented" src="https://img.shields.io/badge/Structure-Process--oriented-167D5A?style=flat-square">
  <img alt="SAP" src="https://img.shields.io/badge/Platform-SAP-0FA3D9?style=flat-square">
  <img alt="Language" src="https://img.shields.io/badge/Language-Chinese%20%7C%20SAP%20Terms-6B7280?style=flat-square">
</p>

> **项目定位**
>
> 本知识库用于沉淀、检索和复用企业 SAP 操作流程，覆盖采购、销售、供应商与材料主数据、MRP、合同、工程变更、审批、报表及输出管理等业务领域。
>
> **重要提示：** 本文档基于现有 SAP 培训资料整理，属于内部操作参考。系统字段、组织结构、权限、配置值及状态流转可能因系统版本和企业配置而异，执行前必须以当前 SAP 系统及内部制度为准。

---

## 01 · Knowledge Base Overview

### 核心用途

- **标准化操作：** 将分散的培训知识整理为可检索、可复用的业务流程。
- **快速定位：** 通过业务领域或 Transaction Code 直接进入对应操作文档。
- **过程可视化：** 每个流程文档原则上包含操作步骤、Mermaid 流程图及关键字段说明。
- **知识持续维护：** 通过统一更新规范管理流程变更，降低知识过期风险。
- **跨流程关联：** 将业务操作与相关事务码、前置条件及后续步骤建立索引关系。

### 适用读者

| 角色 | 使用场景 |
|---|---|
| Procurement / Purchasing | 采购申请、询价、报价、采购订单、合同及供应商协同 |
| Master Data | 供应商、客户、材料及采购信息记录维护 |
| Planning / MRP | 物料需求计划、货源清单及计划订单处理 |
| Engineering / PDM | 材料、BOM、文档及工程变更管理 |
| Operations / Key Users | 日常操作查询、异常定位及流程交接 |
| Process Owners | 流程审核、知识维护及标准化管理 |

### 如何使用

1. **按业务场景查找：** 在下方「流程目录」中选择业务域。
2. **按事务码查找：** 在文末「Transaction Code 索引」中搜索 SAP 事务码。
3. **执行前核对：** 阅读流程中的前置条件、组织范围、关键字段和风险提示。
4. **执行后确认：** 根据流程要求检查凭证状态、审批状态、输出结果或后续单据。
5. **发现差异时：** 先确认系统配置和权限，再按知识库维护规范更新文档。

### 文档规范

- 每项业务流程独立保存为 Markdown 文件，避免将多个操作场景混写在同一文档中。
- 文件名采用 `序号-业务主题-事务码.md` 或现有目录约定，保持稳定、可读。
- 流程文档应尽可能包含：目的与适用范围、前置条件、操作步骤、关键字段、流程图、结果检查及注意事项。
- 事务码仅作为入口索引；具体操作以对应流程文档和当前系统界面为准。
- 更新规则与维护提示见 [`UPDATE_PROMPT.md`](UPDATE_PROMPT.md)。

---

## 02 · Process Catalogue

以下目录保留现有知识库中的流程条目与文件路径。点击条目即可打开对应操作说明。

## 流程目录
### 销售与售后
- [创建客户主数据](docs/sales/01-create-customer-vd01.md)

- [创建报价](docs/sales/02-create-quotation-va21.md)

- [创建客户订单](docs/sales/03-create-sales-order-va01.md)

- [从报价创建订单](docs/sales/04-order-from-quotation.md)

- [创建与放行贷项通知请求](docs/sales/05-credit-memo-request.md)

- [客户退货处理](docs/sales/06-return-process.md)

### 采购
- [冻结重复供应商并设置删除标识](docs/purchasing/01-block-duplicate-vendor.md)

- [维护供应商的替代订购地址](docs/purchasing/02-alternate-order-address.md)

- [维护供应商的替代开票方](docs/purchasing/03-alternate-invoicing-party.md)

- [创建采购询价](docs/purchasing/04-create-rfq-me41.md)

- [从已有询价复制并新增供应商](docs/purchasing/05-copy-rfq-template.md)

- [修改与显示采购询价](docs/purchasing/06-change-display-rfq.md)

- [录入与显示供应商报价](docs/purchasing/07-maintain-display-quotation.md)

- [执行供应商报价比较](docs/purchasing/08-quotation-comparison-me49.md)

- [创建标准采购申请 BANF](docs/purchasing/09-create-purchase-requisition-me51n.md)

- [修改与显示采购申请 BANF](docs/purchasing/10-change-display-purchase-requisition.md)

- [采购清单报表与开放订单分析](docs/purchasing/11-purchasing-list-reports.md)

- [ME80FN 期望交期与实际交期对比](docs/purchasing/12-me80fn-delivery-date-report.md)

- [供应商采购金额分析和偏差区间](docs/purchasing/13-vendor-purchasing-value-analysis.md)

- [采购订单确认监控 Bestellbestätigungsmonitor](docs/purchasing/14-monitor-purchase-order-confirmations.md)

- [按创建人查看 BANF 与放行状态](docs/purchasing/15-list-purchase-requisitions-by-creator.md)

- [使用 ME21N 手工创建采购订单](docs/purchasing/16-create-manual-purchase-order-me21n.md)

- [创建特殊采购订单与交货](docs/purchasing/17-create-special-purchase-orders.md)

- [使用 ME57 分配 BANF 并创建采购订单](docs/purchasing/18-convert-purchase-requisitions-me57.md)

- [委外加工供料与外部库存检查](docs/purchasing/19-subcontracting-component-delivery.md)

- [维护委外供料供应商主数据](docs/purchasing/20-maintain-subcontracting-vendor-master.md)

- [维护委外采购及供料组件材料主数据](docs/purchasing/21-maintain-subcontracting-material-master.md)

- [无材料号采购信息记录及参数化服务编码](docs/purchasing/22-info-records-without-material-number.md)

- [创建带开票的跨公司采购订单](docs/purchasing/23-create-intercompany-purchase-order.md)

- [创建采购信息记录](docs/purchasing/24-create-purchasing-info-record.md)

- [修改、显示及删除标识采购信息记录](docs/purchasing/25-change-display-delete-info-record.md)

- [创建已科目分配的采购申请](docs/purchasing/26-create-account-assigned-requisition.md)

- [将已科目分配 BANF 转为采购订单](docs/purchasing/27-convert-account-assigned-requisition.md)

- [手工创建成本中心或固定资产采购订单](docs/purchasing/28-create-manual-account-assigned-order.md)

- [批量导出及导入采购信息记录价格条件](docs/purchasing/29-mass-maintain-purchasing-conditions.md)

- [使用 MEKP 批量调整采购信息记录价格](docs/purchasing/30-change-info-record-prices-mekp.md)

### 物料计划 / MRP
- [在物料主数据中扩展 MRP 区域](docs/material-planning/01-extend-material-mrp-area.md)

- [检查并运行 MRP 区域计划](docs/material-planning/02-check-plan-mrp-area.md)

### Variant Configuration
- [软管变式配置主数据](docs/vc/01-hose-variant-configuration.md)

### PDM / 工程变更
- [创建变更号](docs/pdm/01-create-change-number-cc01.md)

- [创建材料](docs/pdm/02-create-material-mm01.md)

- [创建或修改 BOM](docs/pdm/03-maintain-bom-cs01-cs02.md)

- [修改文档与材料链接](docs/pdm/04-document-management-cv02n.md)

- [显示与搜索文档](docs/pdm/05-display-search-document.md)

- [显示与搜索材料](docs/pdm/06-material-display-search-mm03.md)

- [材料主数据工作流](docs/pdm/07-material-workflow.md)

### 采购催交与沟通
- [催交逾期或即将到期采购订单](docs/purchasing-communications/01-remind-overdue-purchase-orders.md)

- [催收缺失的订单确认](docs/purchasing-communications/02-remind-missing-order-confirmations.md)

- [催收合同与询价报价](docs/purchasing-communications/03-remind-contracts-and-rfqs.md)

### 材料主数据
- [将现有材料扩展至工厂采购、MRP 与会计视图](docs/material-master/01-extend-material-to-plant.md)

### 供应商主数据
- [将现有供应商扩展至公司代码和采购组织](docs/supplier-master/01-extend-vendor-to-company-and-purchasing-org.md)

- [维护供应商采购文本及语言版本](docs/supplier-master/02-maintain-vendor-purchasing-texts.md)

- [创建供应商并监控主数据工作流](docs/supplier-master/03-create-vendor-and-monitor-workflow.md)

### 供应商质量
- [年度供应商评价与历史数据归档](docs/supplier-quality/01-archive-annual-supplier-evaluation.md)

### 供应商退货
- [从质量工作项创建供应商退货](docs/supplier-returns/01-create-supplier-return-from-qm-workitem.md)

- [在退货订单中增加替代交货项目](docs/supplier-returns/02-add-replacement-delivery-to-return-order.md)

### 发运
- [手工创建无订单引用的发货单](docs/shipping/01-create-delivery-without-reference.md)

### 合同
- [准备中央采购合同的跨组织主数据](docs/contracts/01-prepare-central-contract-master-data.md)

- [创建中央数量合同](docs/contracts/02-create-central-quantity-contract.md)

- [重复输出中央合同](docs/contracts/03-repeat-central-contract-output.md)

- [创建工厂级数量合同](docs/contracts/04-create-plant-level-quantity-contract.md)

- [维护合同货源清单并监控合同调用量](docs/contracts/05-maintain-source-list-and-monitor-contract-usage.md)

- [维护框架协议监控阈值](docs/contracts/06-maintain-contract-monitoring-thresholds.md)

- [使用自定义报表监控框架协议](docs/contracts/07-monitor-framework-agreements.md)

- [保存并调用框架协议监控变式](docs/contracts/08-save-contract-monitor-variant.md)

- [维护框架协议状态自定义表](docs/contracts/09-maintain-framework-agreement-status.md)

### 物料计划 / MRP
- [手动启动项目 MRP 计划运行](docs/material-planning/03-run-project-mrp-md51.md)

- [在 MD04 中将计划订单转换为 BANF 或生产订单](docs/material-planning/04-convert-planned-order-in-md04.md)

- [运行单项多层 MRP 并使用 MD06 处理计划清单](docs/material-planning/05-run-net-change-and-worklist-md04-md06.md)

- [维护材料货源清单与固定供应源](docs/material-planning/06-maintain-source-list.md)

- [从信息记录或合同生成货源清单记录](docs/material-planning/07-generate-source-list-records.md)

### 库存与消耗分析
- [运行 XYZ 分析并更新材料分类](docs/analysis/01-run-xyz-analysis.md)

- [查询与分析 XYZ 分类结果](docs/analysis/02-evaluate-xyz-results.md)

- [维护 XYZ 分类阈值](docs/analysis/03-maintain-xyz-thresholds.md)

- [结合 ABC 与 XYZ 分析制定物料计划策略](docs/analysis/04-compare-abc-and-xyz-analysis.md)

### 工程变更与 BOM
- [维护委外供料 BOM 项目标识](docs/pdm/08-maintain-subcontracting-bom-flags.md)

- [使用变更号修改委外供料 BOM](docs/pdm/09-change-subcontracting-bom-with-ecn.md)

- [执行材料主数据工程变更工作流](docs/pdm/10-run-material-master-change-workflow.md)

### 审批策略
- [分析采购审批策略的特征与分类](docs/release-strategy/01-analyze-release-characteristics.md)

- [使用 CL20N 调整 BANF 与采购订单审批策略](docs/release-strategy/02-change-purchase-release-strategy-cl20n.md)

- [批量审批已科目分配的采购申请](docs/release-strategy/03-release-account-assigned-requisitions.md)

- [单笔审批、拒绝或撤销采购申请](docs/release-strategy/04-single-release-reject-requisition.md)

- [批量审批采购订单](docs/release-strategy/05-mass-release-purchase-orders.md)

- [单笔审批、拒绝或撤销采购订单](docs/release-strategy/06-single-release-reject-purchase-order.md)

### 报表与布局
- [调整、保存并选择 ALV 列表布局](docs/reporting/01-customize-save-select-alv-layout.md)

- [按材料、供应商、科目分配或提交号搜索采购凭证](docs/reporting/02-search-purchasing-documents.md)

- [采购与主数据 Transaction Code 参考](docs/reporting/03-transaction-code-reference.md)

### 输出管理 DOM
- [监控 DOM Trigger 处理状态](docs/output-management/01-monitor-dom-trigger.md)

- [处理和删除 DOM 工作列表消息](docs/output-management/02-edit-dom-worklist.md)

- [重复发送或手工创建 DOM 输出消息](docs/output-management/03-repeat-create-dom-output.md)

- [手工打印或生成 PDF 的 DOM 输出](docs/output-management/04-manual-dom-print-pdf.md)

- [DOM 功能范围、监控入口与状态判断](docs/output-management/05-dom-training-overview.md)

- [配置经典采购消息控制条件记录](docs/output-management/06-configure-classic-message-control-nace.md)

- [采购消息媒介与发送时点参考](docs/output-management/07-message-medium-and-dispatch-time-reference.md)

### 标准文本
- [创建及维护多语言标准文本](docs/text-management/01-create-maintain-standard-texts.md)

- [在采购凭证中插入标准文本](docs/text-management/02-insert-standard-text-into-purchasing-document.md)

### 个人设置
- [配置 SAP GUI 个人基本设置](docs/user-settings/01-configure-sap-user-settings.md)

- [设置 SAP 工作流代理人](docs/user-settings/02-set-workflow-substitute.md)

- [设置 DOM 输出签署权限标识](docs/user-settings/03-set-dom-signature-authority.md)

## Transaction Code 索引
| Transaction | 流程文件 |
|---|---|
| `/JA41/_BBEST` | [14-monitor-purchase-order-confirmations](docs/purchasing/14-monitor-purchase-order-confirmations.md) |

| `/JA41/_BC_IMG` | [14-monitor-purchase-order-confirmations](docs/purchasing/14-monitor-purchase-order-confirmations.md) |

| `CC01` | [01-create-change-number-cc01](docs/pdm/01-create-change-number-cc01.md) |

| `CC02` | [07-material-workflow](docs/pdm/07-material-workflow.md) |

| `CC07` | [07-material-workflow](docs/pdm/07-material-workflow.md) |

| `CH41` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CH42` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CH43` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CS01` | [03-maintain-bom-cs01-cs02](docs/pdm/03-maintain-bom-cs01-cs02.md)<br>[01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CS02` | [03-maintain-bom-cs01-cs02](docs/pdm/03-maintain-bom-cs01-cs02.md)<br>[01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CS03` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CT04` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CU01` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CU02` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CU03` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `CV02N` | [04-document-management-cv02n](docs/pdm/04-document-management-cv02n.md) |

| `CV03N` | [05-display-search-document](docs/pdm/05-display-search-document.md) |

| `CV04N` | [05-display-search-document](docs/pdm/05-display-search-document.md) |

| `M-04` | [03-alternate-invoicing-party](docs/purchasing/03-alternate-invoicing-party.md) |

| `M-06` | [02-alternate-order-address](docs/purchasing/02-alternate-order-address.md) |

| `MC$4` | [13-vendor-purchasing-value-analysis](docs/purchasing/13-vendor-purchasing-value-analysis.md) |

| `MD04` | [02-check-plan-mrp-area](docs/material-planning/02-check-plan-mrp-area.md) |

| `ME1M` | [11-purchasing-list-reports](docs/purchasing/11-purchasing-list-reports.md) |

| `ME21N` | [16-create-manual-purchase-order-me21n](docs/purchasing/16-create-manual-purchase-order-me21n.md)<br>[17-create-special-purchase-orders](docs/purchasing/17-create-special-purchase-orders.md) |

| `ME22N` | [16-create-manual-purchase-order-me21n](docs/purchasing/16-create-manual-purchase-order-me21n.md) |

| `ME23N` | [14-monitor-purchase-order-confirmations](docs/purchasing/14-monitor-purchase-order-confirmations.md)<br>[16-create-manual-purchase-order-me21n](docs/purchasing/16-create-manual-purchase-order-me21n.md) |

| `ME2L` | [11-purchasing-list-reports](docs/purchasing/11-purchasing-list-reports.md) |

| `ME2ON` | [19-subcontracting-component-delivery](docs/purchasing/19-subcontracting-component-delivery.md) |

| `ME3L` | [11-purchasing-list-reports](docs/purchasing/11-purchasing-list-reports.md) |

| `ME41` | [04-create-rfq-me41](docs/purchasing/04-create-rfq-me41.md)<br>[05-copy-rfq-template](docs/purchasing/05-copy-rfq-template.md) |

| `ME42` | [06-change-display-rfq](docs/purchasing/06-change-display-rfq.md) |

| `ME43` | [06-change-display-rfq](docs/purchasing/06-change-display-rfq.md) |

| `ME47` | [07-maintain-display-quotation](docs/purchasing/07-maintain-display-quotation.md) |

| `ME48` | [07-maintain-display-quotation](docs/purchasing/07-maintain-display-quotation.md) |

| `ME49` | [08-quotation-comparison-me49](docs/purchasing/08-quotation-comparison-me49.md) |

| `ME4S` | [11-purchasing-list-reports](docs/purchasing/11-purchasing-list-reports.md) |

| `ME51N` | [09-create-purchase-requisition-me51n](docs/purchasing/09-create-purchase-requisition-me51n.md) |

| `ME52N` | [10-change-display-purchase-requisition](docs/purchasing/10-change-display-purchase-requisition.md) |

| `ME53N` | [10-change-display-purchase-requisition](docs/purchasing/10-change-display-purchase-requisition.md) |

| `ME57` | [18-convert-purchase-requisitions-me57](docs/purchasing/18-convert-purchase-requisitions-me57.md) |

| `ME5A` | [15-list-purchase-requisitions-by-creator](docs/purchasing/15-list-purchase-requisitions-by-creator.md) |

| `ME80FN` | [12-me80fn-delivery-date-report](docs/purchasing/12-me80fn-delivery-date-report.md) |

| `MK02` | [01-block-duplicate-vendor](docs/purchasing/01-block-duplicate-vendor.md)<br>[02-alternate-order-address](docs/purchasing/02-alternate-order-address.md)<br>[03-alternate-invoicing-party](docs/purchasing/03-alternate-invoicing-party.md) |

| `MM01` | [01-extend-material-mrp-area](docs/material-planning/01-extend-material-mrp-area.md)<br>[02-create-material-mm01](docs/pdm/02-create-material-mm01.md) |

| `MM02` | [01-extend-material-mrp-area](docs/material-planning/01-extend-material-mrp-area.md) |

| `MM03` | [06-material-display-search-mm03](docs/pdm/06-material-display-search-mm03.md)<br>[01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `MMBE` | [19-subcontracting-component-delivery](docs/purchasing/19-subcontracting-component-delivery.md) |

| `PMEVC` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `VA01` | [03-create-sales-order-va01](docs/sales/03-create-sales-order-va01.md)<br>[04-order-from-quotation](docs/sales/04-order-from-quotation.md)<br>[05-credit-memo-request](docs/sales/05-credit-memo-request.md)<br>[06-return-process](docs/sales/06-return-process.md) |

| `VA02` | [03-create-sales-order-va01](docs/sales/03-create-sales-order-va01.md)<br>[05-credit-memo-request](docs/sales/05-credit-memo-request.md)<br>[06-return-process](docs/sales/06-return-process.md) |

| `VA03` | [03-create-sales-order-va01](docs/sales/03-create-sales-order-va01.md) |

| `VA05` | [03-create-sales-order-va01](docs/sales/03-create-sales-order-va01.md) |

| `VA05N` | [03-create-sales-order-va01](docs/sales/03-create-sales-order-va01.md) |

| `VA21` | [02-create-quotation-va21](docs/sales/02-create-quotation-va21.md) |

| `VA22` | [02-create-quotation-va21](docs/sales/02-create-quotation-va21.md) |

| `VA23` | [02-create-quotation-va21](docs/sales/02-create-quotation-va21.md) |

| `VA25N` | [02-create-quotation-va21](docs/sales/02-create-quotation-va21.md) |

| `VD01` | [01-create-customer-vd01](docs/sales/01-create-customer-vd01.md) |

| `VF01` | [05-credit-memo-request](docs/sales/05-credit-memo-request.md) |

| `VK11` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `VK12` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `VK13` | [01-hose-variant-configuration](docs/vc/01-hose-variant-configuration.md) |

| `VL01N` | [06-return-process](docs/sales/06-return-process.md) |

| `VL02N` | [19-subcontracting-component-delivery](docs/purchasing/19-subcontracting-component-delivery.md)<br>[06-return-process](docs/sales/06-return-process.md) |

| `VL10B` | [17-create-special-purchase-orders](docs/purchasing/17-create-special-purchase-orders.md) |

| `XK02` | [01-block-duplicate-vendor](docs/purchasing/01-block-duplicate-vendor.md) |

| `/JA41/M_DOM_MON_TRG` | [01-monitor-dom-trigger](docs/output-management/01-monitor-dom-trigger.md)<br>[05-dom-training-overview](docs/output-management/05-dom-training-overview.md) |

| `/JA41/M_DOM_WORKLIST` | [02-edit-dom-worklist](docs/output-management/02-edit-dom-worklist.md)<br>[05-dom-training-overview](docs/output-management/05-dom-training-overview.md) |

| `/JA41/M_REPKONTRAKT` | [07-monitor-framework-agreements](docs/contracts/07-monitor-framework-agreements.md)<br>[08-save-contract-monitor-variant](docs/contracts/08-save-contract-monitor-variant.md) |

| `/JA41/M_RVSTAT` | [09-maintain-framework-agreement-status](docs/contracts/09-maintain-framework-agreement-status.md) |

| `/JA41/XYZ_01` | [01-run-xyz-analysis](docs/analysis/01-run-xyz-analysis.md)<br>[04-compare-abc-and-xyz-analysis](docs/analysis/04-compare-abc-and-xyz-analysis.md) |

| `/JA41/XYZ_02` | [02-evaluate-xyz-results](docs/analysis/02-evaluate-xyz-results.md)<br>[04-compare-abc-and-xyz-analysis](docs/analysis/04-compare-abc-and-xyz-analysis.md) |

| `/JA41/XYZ_STAT` | [03-maintain-xyz-thresholds](docs/analysis/03-maintain-xyz-thresholds.md) |

| `CC01` | [09-change-subcontracting-bom-with-ecn](docs/pdm/09-change-subcontracting-bom-with-ecn.md) |

| `CC02` | [10-run-material-master-change-workflow](docs/pdm/10-run-material-master-change-workflow.md) |

| `CC07` | [10-run-material-master-change-workflow](docs/pdm/10-run-material-master-change-workflow.md) |

| `CL02` | [01-analyze-release-characteristics](docs/release-strategy/01-analyze-release-characteristics.md) |

| `CL20N` | [02-change-purchase-release-strategy-cl20n](docs/release-strategy/02-change-purchase-release-strategy-cl20n.md) |

| `CS02` | [08-maintain-subcontracting-bom-flags](docs/pdm/08-maintain-subcontracting-bom-flags.md)<br>[09-change-subcontracting-bom-with-ecn](docs/pdm/09-change-subcontracting-bom-with-ecn.md) |

| `CS03` | [08-maintain-subcontracting-bom-flags](docs/pdm/08-maintain-subcontracting-bom-flags.md) |

| `CT04` | [01-analyze-release-characteristics](docs/release-strategy/01-analyze-release-characteristics.md) |

| `MC40` | [04-compare-abc-and-xyz-analysis](docs/analysis/04-compare-abc-and-xyz-analysis.md) |

| `MC41` | [04-compare-abc-and-xyz-analysis](docs/analysis/04-compare-abc-and-xyz-analysis.md) |

| `MD04` | [04-convert-planned-order-in-md04](docs/material-planning/04-convert-planned-order-in-md04.md)<br>[05-run-net-change-and-worklist-md04-md06](docs/material-planning/05-run-net-change-and-worklist-md04-md06.md)<br>[05-mass-release-purchase-orders](docs/release-strategy/05-mass-release-purchase-orders.md)<br>[01-create-supplier-return-from-qm-workitem](docs/supplier-returns/01-create-supplier-return-from-qm-workitem.md)<br>[02-add-replacement-delivery-to-return-order](docs/supplier-returns/02-add-replacement-delivery-to-return-order.md)<br>[01-configure-sap-user-settings](docs/user-settings/01-configure-sap-user-settings.md) |

| `MD06` | [05-run-net-change-and-worklist-md04-md06](docs/material-planning/05-run-net-change-and-worklist-md04-md06.md) |

| `MD51` | [03-run-project-mrp-md51](docs/material-planning/03-run-project-mrp-md51.md) |

| `ME01` | [05-maintain-source-list-and-monitor-contract-usage](docs/contracts/05-maintain-source-list-and-monitor-contract-usage.md)<br>[06-maintain-source-list](docs/material-planning/06-maintain-source-list.md)<br>[07-generate-source-list-records](docs/material-planning/07-generate-source-list-records.md) |

| `ME03` | [06-maintain-source-list](docs/material-planning/06-maintain-source-list.md) |

| `ME04` | [06-maintain-source-list](docs/material-planning/06-maintain-source-list.md) |

| `ME11` | [22-info-records-without-material-number](docs/purchasing/22-info-records-without-material-number.md)<br>[24-create-purchasing-info-record](docs/purchasing/24-create-purchasing-info-record.md) |

| `ME12` | [22-info-records-without-material-number](docs/purchasing/22-info-records-without-material-number.md)<br>[25-change-display-delete-info-record](docs/purchasing/25-change-display-delete-info-record.md)<br>[30-change-info-record-prices-mekp](docs/purchasing/30-change-info-record-prices-mekp.md) |

| `ME13` | [22-info-records-without-material-number](docs/purchasing/22-info-records-without-material-number.md)<br>[25-change-display-delete-info-record](docs/purchasing/25-change-display-delete-info-record.md)<br>[30-change-info-record-prices-mekp](docs/purchasing/30-change-info-record-prices-mekp.md) |

| `ME1L` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME1M` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME21N` | [23-create-intercompany-purchase-order](docs/purchasing/23-create-intercompany-purchase-order.md)<br>[28-create-manual-account-assigned-order](docs/purchasing/28-create-manual-account-assigned-order.md)<br>[02-insert-standard-text-into-purchasing-document](docs/text-management/02-insert-standard-text-into-purchasing-document.md) |

| `ME22N` | [03-repeat-create-dom-output](docs/output-management/03-repeat-create-dom-output.md)<br>[04-manual-dom-print-pdf](docs/output-management/04-manual-dom-print-pdf.md)<br>[02-add-replacement-delivery-to-return-order](docs/supplier-returns/02-add-replacement-delivery-to-return-order.md)<br>[02-insert-standard-text-into-purchasing-document](docs/text-management/02-insert-standard-text-into-purchasing-document.md) |

| `ME28` | [05-mass-release-purchase-orders](docs/release-strategy/05-mass-release-purchase-orders.md) |

| `ME29N` | [06-single-release-reject-purchase-order](docs/release-strategy/06-single-release-reject-purchase-order.md) |

| `ME2K` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME2L` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME2M` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md)<br>[01-create-supplier-return-from-qm-workitem](docs/supplier-returns/01-create-supplier-return-from-qm-workitem.md)<br>[02-add-replacement-delivery-to-return-order](docs/supplier-returns/02-add-replacement-delivery-to-return-order.md) |

| `ME31K` | [02-create-central-quantity-contract](docs/contracts/02-create-central-quantity-contract.md)<br>[04-create-plant-level-quantity-contract](docs/contracts/04-create-plant-level-quantity-contract.md)<br>[06-maintain-contract-monitoring-thresholds](docs/contracts/06-maintain-contract-monitoring-thresholds.md)<br>[02-insert-standard-text-into-purchasing-document](docs/text-management/02-insert-standard-text-into-purchasing-document.md) |

| `ME32K` | [02-create-central-quantity-contract](docs/contracts/02-create-central-quantity-contract.md)<br>[04-create-plant-level-quantity-contract](docs/contracts/04-create-plant-level-quantity-contract.md)<br>[05-maintain-source-list-and-monitor-contract-usage](docs/contracts/05-maintain-source-list-and-monitor-contract-usage.md)<br>[06-maintain-contract-monitoring-thresholds](docs/contracts/06-maintain-contract-monitoring-thresholds.md) |

| `ME33K` | [02-create-central-quantity-contract](docs/contracts/02-create-central-quantity-contract.md)<br>[04-create-plant-level-quantity-contract](docs/contracts/04-create-plant-level-quantity-contract.md)<br>[05-maintain-source-list-and-monitor-contract-usage](docs/contracts/05-maintain-source-list-and-monitor-contract-usage.md)<br>[06-maintain-contract-monitoring-thresholds](docs/contracts/06-maintain-contract-monitoring-thresholds.md) |

| `ME3L` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME3M` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME41` | [02-insert-standard-text-into-purchasing-document](docs/text-management/02-insert-standard-text-into-purchasing-document.md) |

| `ME42` | [03-repeat-create-dom-output](docs/output-management/03-repeat-create-dom-output.md) |

| `ME4L` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME4M` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME4S` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME51N` | [26-create-account-assigned-requisition](docs/purchasing/26-create-account-assigned-requisition.md) |

| `ME54N` | [04-single-release-reject-requisition](docs/release-strategy/04-single-release-reject-requisition.md) |

| `ME55` | [03-release-account-assigned-requisitions](docs/release-strategy/03-release-account-assigned-requisitions.md) |

| `ME57` | [27-convert-account-assigned-requisition](docs/purchasing/27-convert-account-assigned-requisition.md)<br>[01-configure-sap-user-settings](docs/user-settings/01-configure-sap-user-settings.md) |

| `ME5A` | [02-search-purchasing-documents](docs/reporting/02-search-purchasing-documents.md) |

| `ME91A` | [03-remind-contracts-and-rfqs](docs/purchasing-communications/03-remind-contracts-and-rfqs.md) |

| `ME91F` | [01-remind-overdue-purchase-orders](docs/purchasing-communications/01-remind-overdue-purchase-orders.md) |

| `ME92F` | [02-remind-missing-order-confirmations](docs/purchasing-communications/02-remind-missing-order-confirmations.md) |

| `ME92K` | [03-remind-contracts-and-rfqs](docs/purchasing-communications/03-remind-contracts-and-rfqs.md) |

| `ME9K` | [03-repeat-central-contract-output](docs/contracts/03-repeat-central-contract-output.md) |

| `MEKP` | [30-change-info-record-prices-mekp](docs/purchasing/30-change-info-record-prices-mekp.md) |

| `MK01` | [03-create-vendor-and-monitor-workflow](docs/supplier-master/03-create-vendor-and-monitor-workflow.md) |

| `MK02` | [20-maintain-subcontracting-vendor-master](docs/purchasing/20-maintain-subcontracting-vendor-master.md)<br>[02-maintain-vendor-purchasing-texts](docs/supplier-master/02-maintain-vendor-purchasing-texts.md) |

| `MK03` | [06-maintain-source-list](docs/material-planning/06-maintain-source-list.md) |

| `MM01` | [01-prepare-central-contract-master-data](docs/contracts/01-prepare-central-contract-master-data.md)<br>[01-extend-material-to-plant](docs/material-master/01-extend-material-to-plant.md) |

| `MM02` | [21-maintain-subcontracting-material-master](docs/purchasing/21-maintain-subcontracting-material-master.md) |

| `NACE` | [06-configure-classic-message-control-nace](docs/output-management/06-configure-classic-message-control-nace.md) |

| `SBWP` | [10-run-material-master-change-workflow](docs/pdm/10-run-material-master-change-workflow.md)<br>[01-create-supplier-return-from-qm-workitem](docs/supplier-returns/01-create-supplier-return-from-qm-workitem.md)<br>[02-set-workflow-substitute](docs/user-settings/02-set-workflow-substitute.md) |

| `SO10` | [01-create-maintain-standard-texts](docs/text-management/01-create-maintain-standard-texts.md) |

| `SOST` | [03-create-vendor-and-monitor-workflow](docs/supplier-master/03-create-vendor-and-monitor-workflow.md) |

| `SU3` | [01-configure-sap-user-settings](docs/user-settings/01-configure-sap-user-settings.md)<br>[03-set-dom-signature-authority](docs/user-settings/03-set-dom-signature-authority.md) |

| `VL01NO` | [01-create-delivery-without-reference](docs/shipping/01-create-delivery-without-reference.md) |

| `VL02N` | [01-create-delivery-without-reference](docs/shipping/01-create-delivery-without-reference.md) |

| `VL03N` | [01-create-delivery-without-reference](docs/shipping/01-create-delivery-without-reference.md) |

| `XK01` | [01-prepare-central-contract-master-data](docs/contracts/01-prepare-central-contract-master-data.md)<br>[01-extend-vendor-to-company-and-purchasing-org](docs/supplier-master/01-extend-vendor-to-company-and-purchasing-org.md) |

| `ZMMKONDITIONEN` | [29-mass-maintain-purchasing-conditions](docs/purchasing/29-mass-maintain-purchasing-conditions.md)<br>[30-change-info-record-prices-mekp](docs/purchasing/30-change-info-record-prices-mekp.md) |

## 匿名化规则
- 公司名称统一替换为“公司”或“内部”。

- 人员姓名、品牌、邮箱、电话、本地路径、地点、历史供应商编号和可识别配置不写入流程。

- 原始附件不纳入 ZIP。

- 交付前执行全文扫描、链接检查及 ZIP 完整性检查。

---

## 03 · Documentation Governance

### 内容可信度与使用边界

- 本知识库是内部培训与操作经验的结构化整理，不替代 SAP 系统配置文档、正式工作指引或审批制度。
- 不应仅凭事务码推断用户拥有执行权限；权限以实际角色分配为准。
- 对于定制事务码、企业专用报表及自定义字段，应以本企业 SAP 环境为唯一执行依据。
- 当文档内容与系统实际行为不一致时，应暂停按旧文档操作，并由流程负责人或系统支持人员确认。

### 更新与审核原则

| 维护项目 | 要求 |
|---|---|
| 流程变更 | 同步更新步骤、流程图、字段说明及关联索引 |
| 事务码变更 | 检查事务码索引及所有受影响流程 |
| 组织或权限变化 | 明确标注适用范围，并由责任人验证 |
| 文档链接 | 确保目录链接指向真实存在的文件 |
| 版本维护 | 重要变更应记录日期、变更内容及维护责任人 |

### 建议的流程文档结构

```text
# 流程名称

## 目的与适用范围
## 前置条件
## 操作步骤
## 关键字段说明
## 流程图
## 结果检查
## 常见问题与注意事项
## 相关事务码与关联流程
```

### 数据保护与匿名化

- 公司名称统一使用“公司”或“内部”等中性表述。
- 不在流程文档中保留人员姓名、品牌、邮箱、电话、具体地点或本地路径等可识别信息。
- 对历史供应商编号、客户编号及其他可识别配置值进行匿名化处理。
- 原始附件不纳入对外分发的 ZIP 包。
- 发布或交付前执行全文敏感信息扫描、Markdown 链接检查及 ZIP 完整性检查。

---

## 04 · Repository Maintenance Checklist

- [ ] 新增流程已放入正确业务目录
- [ ] 文件命名符合仓库约定
- [ ] 流程步骤与当前 SAP 环境完成核对
- [ ] 关键字段、权限及组织范围已注明
- [ ] Mermaid 流程图与实际步骤一致
- [ ] 相关 Transaction Code 索引已更新
- [ ] README 内部链接检查通过
- [ ] 敏感信息与匿名化检查通过
- [ ] 更新内容已由相应流程负责人确认

---

<p align="center">
  <sub>内部知识管理资料 · SAP Process Reference · Verify in the target system before execution</sub>
</p>
