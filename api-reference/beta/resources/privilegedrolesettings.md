---
title: privilegedRoleSettings リソースの種類
description: 特権ロールの設定を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed87787ca8016f1dde7711304a1da1fc977c641b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965714"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権ロールの設定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedRoleSettings を取得する](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトのプロパティとリレーションシップを読み取ります。|
|[PrivilegedRoleSettings の更新](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトを更新します。|
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevationDuration|duration|役割がアクティブ化される期間。|
|id|string| ロール設定の一意の識別子。 読み取り専用です。|
|isMfaOnElevationConfigurable|ブール値|**true**の場合は、mfaOnElevation を構成できます。 mfaOnElevation を構成できない場合は**false** 。|
|lastGlobalAdmin|ブール値|内部でのみ使用されます。|
|maxElavationDuration|duration|アクティブ化されたロールの最大期間。|
|mfaOnElevation|ブール値|役割をアクティブ化するために MFA が必要な場合は**true** 。 役割をアクティブ化するために MFA が必要でない場合は**false** 。|
|minElevationDuration|duration|アクティブ化されたロールの期間を最小化します。|
|notificationToUserOnElevation|ブール値|**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。 **true**の場合は、役割がアクティブ化されたときに通知を送信しません。|
|ticketingInfoOnElevation|ブール値|役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。|
|approvalOnElevation|ブール値|ロールをアクティブ化するときに承認が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに承認が必要ありません。|
|承認の検証 Ds| string collection |ライセンス認証に承認が必要な場合は、承認 id のリスト。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
