---
title: securityactionstate リソースの種類
description: securityAction 状態の変更履歴を表します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522021"
---
# <a name="securityactionstate-resource-type"></a>securityactionstate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

securityAction 状態の変更履歴を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|appId|String|アクションに更新プログラム (PATCH) を送信した、呼び出し元アプリケーションのアプリケーション ID。 は`appId` 、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|status|String| この更新プログラムの securityAction の状態。 可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。|
|updatedDateTime|DateTimeOffset| actionstate が更新されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
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
