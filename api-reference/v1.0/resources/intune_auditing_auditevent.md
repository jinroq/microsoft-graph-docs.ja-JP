# <a name="auditevent-resource-type"></a>auditEvent リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

監査イベントのプロパティが含まれるクラス。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List auditEvents](../api/intune_auditing_auditevent_list.md)|[auditEvent](../resources/intune_auditing_auditevent.md) コレクション|[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get auditEvent](../api/intune_auditing_auditevent_get.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create auditEvent](../api/intune_auditing_auditevent_create.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|新しい [auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトを作成します。|
|[Delete auditEvent](../api/intune_auditing_auditevent_delete.md)|なし|[auditEvent](../resources/intune_auditing_auditevent.md) を削除します。|
|[Update auditEvent](../api/intune_auditing_auditevent_update.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティを更新します。|
|[getAuditCategories function](../api/intune_auditing_auditevent_getauditcategories.md)|String コレクション|まだ文書化されていません|
|[getAuditActivityTypes function](../api/intune_auditing_auditevent_getauditactivitytypes.md)|String コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|displayName|String|イベントの表示名。|
|componentName|String|コンポーネント名。|
|actor|[auditActor](../resources/intune_auditing_auditactor.md)|監査イベントに関連付けられている AAD ユーザーとアプリケーション。|
|activity|String|わかりやすいアクティビティの名前。|
|activityDateTime|DateTimeOffset|アクティビティが実行された日時 (UTC)。|
|activityType|String|実行されたアクティビティの種類。|
|activityOperationType|String|アクティビティの HTTP 操作の種類。|
|activityResult|String|アクティビティの結果。|
|correlationId|Guid|システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。|
|resources|[auditResource](../resources/intune_auditing_auditresource.md) コレクション|変更中のリソースです。|
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
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
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



