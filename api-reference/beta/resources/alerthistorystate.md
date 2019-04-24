---
title: alertHistoryState リソースの種類
description: 通知に加えられた変更を格納します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461048"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知に加えられた変更を格納します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appId|String| 通知に更新プログラム (パッチ) を送信した、呼び出し元アプリケーションのアプリケーション ID。 appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。 |
|assignedTo|String| 通知が割り当てられたユーザーの UPN (注: 通知は、最新の値/UPN のみを保存します)。 |
|コメント|String collection|サインインしているユーザーによって入力されたコメント。|
|feedback|String| この更新プログラムの通知に関するアナリストからのフィードバック。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。|
|status|文字列型 (String)| 警告の状態の値 (更新された場合)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed` です。|
|updatedDateTime|DateTimeOffset| 通知の更新日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
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