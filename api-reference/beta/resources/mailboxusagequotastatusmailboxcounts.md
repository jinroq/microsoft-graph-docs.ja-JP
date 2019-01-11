---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835224"
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
