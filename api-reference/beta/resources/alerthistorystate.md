---
title: alertHistoryState リソースの種類
description: 通知に加えられた変更を格納します。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9467da6f5b088e9b1fadd3797a8b10f4b6e820db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974424"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知に加えられた変更を格納します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appId|String| 通知に更新プログラム (パッチ) を送信した、呼び出し元アプリケーションのアプリケーション ID。 AppId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。 |
|assignedTo|String| 通知が割り当てられたユーザーの UPN (注: 通知は、最新の値/UPN のみを保存します)。 |
|comments|String コレクション|サインインしているユーザーによって入力されたコメント。|
|feedback|String| この更新プログラムの通知に関するアナリストからのフィードバック。 使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。|
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