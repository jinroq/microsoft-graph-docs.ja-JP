---
title: skypeForBusinessPeerToPeerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503885"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a>skypeForBusinessPeerToPeerActivityUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| im                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| appSharing        | Int64  |
| filetransfer      | Int64  |
| reportrefreshdate | Date   |
| reportDate        | Date   |
| reportperiod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
