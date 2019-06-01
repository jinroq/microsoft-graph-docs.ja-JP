---
title: applicationSignInDetailedSummary リソースの種類
description: アプリケーションサインインの概要を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6ecd91bb29abc409a745e92b523948b78552ed4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657624"
---
# <a name="applicationsigninsummary-resource-type"></a>applicationSignInSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションサインインの概要を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [ApplicationSignInSummary を取得する](../api/applicationsigninsummary-get.md) | [applicationSignInSummary](applicationsigninsummary.md) | **ApplicationSignInSummary**オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appDisplayName|String|ユーザーがサインインしたアプリケーションの名前。|
|appId|String|  ユーザーがサインアウトしたアプリケーションの ID。|
|failedSignInCount|Int64|アプリケーションによって実行された、失敗したサインインの数。|
|successPercentage|Int32|アプリケーションによって行われたサインインの成功率。|
|successfulSignInCount|Int64|アプリケーションによって作成された成功したサインインの数。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
