---
title: alertHistoryState リソースの種類
description: 通知にパッチが適用されるたびに、変更は alertHistoryState の新しいオブジェクトに保存され、変更された通知の一部として返されます。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: a5dda54101264ee2ec4d01a283f96a93f1d6e5e3
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366967"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知にパッチが適用されるたびに、変更は alertHistoryState の新しいオブジェクトに保存され、変更された通知の一部として返されます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appId|String| 通知に更新プログラム (パッチ) を送信した、呼び出し元アプリケーションのアプリケーション ID。 appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。 |
|assignedTo|String| 通知が割り当てられたユーザーの UPN (注: 通知は、最新の値/UPN のみを保存します)。 |
|comments|String コレクション|サインインしているユーザーによって入力されたコメント。|
|feedback|String| この更新プログラムの通知に関するアナリストからのフィードバック。 使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。|
|status|文字列型 (String)| 警告の状態の値 (更新された場合)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed` です。|
|updatedDateTime|DateTimeOffset| 通知の更新日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|user|String| アラートを更新したサインインしているユーザーの UPN (ユーザー/委任された認証モードの場合は、ベアラートークンから取得)。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->