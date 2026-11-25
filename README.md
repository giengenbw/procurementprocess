# SAP Process Knowledge Base

> 基于 SAP 培训资料整理。当前字段、权限、组织值和状态流转必须在 SAP 中验证。

## 使用方法

- 按业务域或 Transaction Code 索引进入流程。
- 每个流程独立为 Markdown，包含 Mermaid 流程图和字段表。
- 更新规则见 [`UPDATE_PROMPT.md`](UPDATE_PROMPT.md)。

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

## 来源文件

- `sources/20180417 Anleitung Kreditor sperren.docx`
- `sources/2018_09_13_PDM_Handbuch_gesamt.pdf`
- `sources/2018_11_07-SAL_Handbuch.docx`
- `sources/2018_12_18_Handbuch_VC-Schlauch.docx`
- `sources/AZG Dispobereiche im Materialstamm.docx`
- `sources/Abweichende Kreditorenrollen.docx`
- `sources/Anfrage anlegen, pflegen, Angebotsvergleich FERTIG.docx`
- `sources/Auswertungen und Reporting.docx`
- `sources/BANF erstellen.PDF`
- `sources/Banf (Standard) anlegen, ändern & anzeigen.docx`
- `sources/Banfen pro Sachbearbeiter anzeigen.docx`
- `sources/Bestellbestätigungsmonitor FERTIG.docx`
- `sources/Bestellung (inkl. Sonder-) anlegen me21n FERTIG.docx`
- `sources/Bestellung anlegen me57 FERTIG.docx`
- `sources/Bestellung mit Beistellung Lieferung anlegen FERTIG.docx`
