# <a name="user-resource-type"></a>user リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List users](../api/intune_onboarding_user_list.md)|[user](../resources/intune_onboarding_user.md) コレクション|[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get user](../api/intune_onboarding_user_get.md)|[user](../resources/intune_onboarding_user.md)|[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create user](../api/intune_onboarding_user_create.md)|[user](../resources/intune_onboarding_user.md)|新しい [user](../resources/intune_onboarding_user.md) オブジェクトを作成します。|
|[Delete user](../api/intune_onboarding_user_delete.md)|なし|[user](../resources/intune_onboarding_user.md) を削除します。|
|[Update user](../api/intune_onboarding_user_update.md)|[user](../resources/intune_onboarding_user.md)|[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|ユーザーの一意識別子。|
|deviceEnrollmentLimit|Int32|ユーザーが登録を許可されているデバイスの最大数。 使用できる値は 5 または 1000 です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```



