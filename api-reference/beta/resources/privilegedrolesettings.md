---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2018
ms.locfileid: "27074559"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特権を持つロールの設定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleSettings を取得します。](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。|
|[PrivilegedRoleSettings を更新します。](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトを更新します。|
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevationDuration|duration|ロールが有効な場合の期間です。|
|ID|文字列| ロールの設定の一意の識別子です。 読み取り専用。|
|isMfaOnElevationConfigurable|ブール|**真**mfaOnElevation は、構成可能な場合です。 場合は**false を指定**mfaOnElevation は構成できません。|
|lastGlobalAdmin|ブール|内部エラーのみを使用します。|
|maxElavationDuration|duration|アクティブ化されたロールの最大の期間です。|
|mfaOnElevation|ブール|**true** MFA は、ロールをアクティブにするために必要な場合です。 **false**場合は、MFA は、ロールをアクティブにする必要はありません。|
|minElevationDuration|duration|アクティブ化されたロールの最低限の期間です。|
|notificationToUserOnElevation|ブール|**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。 **false**場合は、ロールがアクティブになったときに通知を送信できません。|
|ticketingInfoOnElevation|ブール|**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。 **false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。|
|approvalOnElevation|ブール|**true の**場合は、承認が必要な場合は、ロールをアクティブにします。 **false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。|
|approverIds|配列|承認 id、ライセンス認証の必要な場合は承認の一覧です。|

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
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->