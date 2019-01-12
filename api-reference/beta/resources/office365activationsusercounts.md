---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917721"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 種類   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日付   | コンテンツの最新の日付。          |
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
