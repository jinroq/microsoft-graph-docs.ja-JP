---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577152"
---
# <a name="privilegedrolesettings-resource-type"></a>privilegedRoleSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権を持つロールの設定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleSettings を取得します。](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。|
|[PrivilegedRoleSettings を更新します。](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |PrivilegedRoleSettings オブジェクトを更新します。|
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevationDuration| 文字列 (タイムスタンプ) |ロールが有効な場合の期間です。|
|id| 文字列 (識別子)| ロールの設定の一意の識別子です。 読み取り専用です。|
|isMfaOnElevationConfigurable|boolean|**真**mfaOnElevation は、構成可能な場合です。 場合は**false を指定**mfaOnElevation は構成できません。|
|lastGlobalAdmin|boolean|内部エラーのみを使用します。|
|maxElavationDuration| 文字列 (識別子)| |アクティブ化されたロールの最大の期間です。|
|mfaOnElevation|boolean|**true** MFA は、ロールをアクティブにするために必要な場合です。 **false**場合は、MFA は、ロールをアクティブにする必要はありません。|
|minElevationDuration|文字列 (識別子)||アクティブ化されたロールの最低限の期間です。|
|notificationToUserOnElevation|boolean|**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。 **false**場合は、ロールがアクティブになったときに通知を送信できません。|
|ticketingInfoOnElevation|boolean|**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。 **false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。|
|approvalOnElevation|boolean|**true の**場合は、承認が必要な場合は、ロールをアクティブにします。 **false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。|
|approverIds| String コレクション |承認 id、ライセンス認証の必要な場合は承認の一覧です。|

## <a name="relationships"></a>関係
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
  "approverIds": [ "String (identifier)" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
