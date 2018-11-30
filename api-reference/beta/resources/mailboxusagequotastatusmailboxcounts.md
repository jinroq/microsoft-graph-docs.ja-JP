---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069374"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>mailboxUsageQuotaStatusMailboxCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ              | 型   |
| :-------------------- | :----- |
| reportRefreshDate     | Date   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| 不確定         | Int64  |
| reportDate            | Date   |
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
