---
title: securityActionState リソースの種類
description: SecurityAction 状態の変更履歴を表します。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e3efd29e156b6e0346574c74fad2a30a39ec7131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008510"
---
# <a name="securityactionstate-resource-type"></a>securityActionState リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

SecurityAction 状態の変更履歴を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appId|String|アクションに更新プログラム (PATCH) を送信した、呼び出し元アプリケーションのアプリケーション ID。 は`appId` 、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|status|String| この更新プログラムの securityAction の状態。 使用可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。|
|updatedDateTime|DateTimeOffset| ActionState が更新されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|user|String|更新 (PATCH) をアクションに送信した、サインインしているユーザーのユーザープリンシパル名。 は`user` 、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
