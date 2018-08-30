# <a name="auditactor-resource-type"></a>auditActor リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

監査アクターのプロパティが含まれるクラス。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|型|文字列型 (String)|アクターの種類。|
|userPermissions|String コレクション|監査の実行時におけるユーザーのアクセス許可の一覧。|
|applicationId|文字列型 (String)|AAD アプリケーション ID。|
|applicationDisplayName|文字列型 (String)|アプリケーションの名前。|
|userPrincipalName|文字列型 (String)|ユーザー プリンシパル名 (UPN)。|
|servicePrincipalName|文字列型 (String)|サービス プリンシパル名 (SPN)。|
|ipAddress|文字列型 (String)|IPAddress。|
|userId|文字列型 (String)|ユーザー ID。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
}
```



