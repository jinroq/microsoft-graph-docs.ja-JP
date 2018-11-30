---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073072"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 型   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | コンテンツの最新の日付。          |
| productType              | String | 「Office 365 用リソース"、「プロジェクト クライアント」などの製品の種類または"Office 365"の Visio Pro です。 |
| 割り当てられています。                 | Int64  | ユーザーの数は、製品のライセンスの割り当てられています。 |
| アクティブ化                | Int64  | 製品をアクティブにしているユーザーの数です。 |
| sharedComputerActivation | Int64  | 共有のコンピューターで製品を使用したユーザーの数です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
