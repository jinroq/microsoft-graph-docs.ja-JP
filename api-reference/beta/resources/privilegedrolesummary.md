---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の概要統計情報です。
localization_priority: Normal
ms.openlocfilehash: b74b562a992f7795f3ae8e317608f1e370bc2a4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858619"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定の役割の概要統計情報です。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleSummary を取得します。](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |PrivilegedRoleSummary オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|elevatedCount|int32|割り当てられているロールおよびロールを持つユーザーの数がアクティブになります。|
|ID|文字列| ロールの一意の識別子です。 読み取り専用です。|
|managedCount|int32|役割が割り当てられているユーザーが、ロールの数が無効になります。|
|mfaEnabled|ブール|**真**の役割のアクティブ化には、MFA が必要な場合です。 **false**の役割のアクティブ化は、MFA を必要としない場合。|
|status|文字列| 使用可能な値は、`ok`、`bad` です。 値の比率によって異なります (managedCount/usersCount)。 割合は、定義済みのしきい値より小さい場合は、`ok`が返されます。 それ以外の場合、`bad`が返されます。|
|usersCount|int32|ロールに割り当てられているユーザーの数です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
