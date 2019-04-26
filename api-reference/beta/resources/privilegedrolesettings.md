---
title: privilegedRoleSettings リソースの種類
description: 特権ロールの設定を表します。
localization_priority: Normal
ms.openlocfilehash: 6500d5a51fcedce97d71c1c4022c7d941de27b83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344231"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権ロールの設定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedRoleSettings を取得する](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |privilegedRoleSettings オブジェクトのプロパティとリレーションシップを読み取ります。|
|[privilegedRoleSettings の更新](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |privilegedRoleSettings オブジェクトを更新します。|
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevationDuration|duration|役割がアクティブ化される期間。|
|id|string| ロール設定の一意の識別子。 読み取り専用です。|
|isMfaOnElevationConfigurable|boolean|**true**の場合は、mfaonelevation を構成できます。 mfaonelevation を構成できない場合は**false** 。|
|lastglobaladmin|boolean|内部でのみ使用されます。|
|maxelavationduration|duration|アクティブ化されたロールの最大期間。|
|mfaonelevation|boolean|役割をアクティブ化するために MFA が必要な場合は**true** 。 役割をアクティブ化するために MFA が必要でない場合は**false** 。|
|minElevationDuration|duration|アクティブ化されたロールの期間を最小化します。|
|notificationToUserOnElevation|boolean|**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。 **true**の場合は、役割がアクティブ化されたときに通知を送信しません。|
|ticketingInfoOnElevation|boolean|役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。|
|approvalonelevation|boolean|ロールをアクティブ化するときに承認が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに承認が必要ありません。|
|承認の検証 ds| string collection |ライセンス認証に承認が必要な場合は、承認 id のリスト。|

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
