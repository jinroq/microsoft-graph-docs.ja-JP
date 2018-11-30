---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
ms.openlocfilehash: 1846677ea72dda836f92e0d45d76ea0df0ae74f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073026"
---
# <a name="auditevent-resource-type"></a>auditEvent リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

監査イベントのプロパティが含まれるクラス。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List auditEvents](../api/intune-auditing-auditevent-list.md)|[auditEvent](../resources/intune-auditing-auditevent.md) コレクション|[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。|
|[Delete auditEvent](../api/intune-auditing-auditevent-delete.md)|なし|[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。|
|[Update auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。|
|[getAuditCategories function](../api/intune-auditing-auditevent-getauditcategories.md)|String コレクション|まだ文書化されていません|
|[getAuditActivityTypes function](../api/intune-auditing-auditevent-getauditactivitytypes.md)|String コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|displayName|String|イベントの表示名。|
|componentName|String|コンポーネント名。|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|監査イベントに関連付けられている AAD ユーザーとアプリケーション。|
|activity|String|わかりやすいアクティビティの名前。|
|activityDateTime|DateTimeOffset|アクティビティが実行された日時 (UTC)。|
|activityType|String|実行されたアクティビティの種類。|
|activityOperationType|String|アクティビティの HTTP 操作の種類。|
|activityResult|String|アクティビティの結果。|
|correlationId|Guid|システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。|
|resources|[auditResource](../resources/intune-auditing-auditresource.md) コレクション|変更中のリソースです。|
|category|String|監査のカテゴリです。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```





