---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921235"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>mailboxUsageQuotaStatusMailboxCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ              | 種類   |
| :-------------------- | :----- |
| reportRefreshDate     | 日付   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| 不確定         | Int64  |
| reportDate            | 日付   |
| reportPeriod          | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
