# <a name="managedappoperation-resource-type"></a>managedAppOperation リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリ登録に対して適用される操作を表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAppOperations のリスト](../api/intune_mam_managedappoperation_list.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション|[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAppOperation を取得する](../api/intune_mam_managedappoperation_get.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedAppOperation を作成する](../api/intune_mam_managedappoperation_create.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|新しい [managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトを作成します。|
|[managedAppOperation を削除する](../api/intune_mam_managedappoperation_delete.md)|なし|[managedAppOperation](../resources/intune_mam_managedappoperation.md) を削除します。|
|[managedAppOperation を更新する](../api/intune_mam_managedappoperation_update.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列|操作名。|
|lastModifiedDateTime|DateTimeOffset|アプリ操作が変更された最終時刻。|
|状態|文字列|操作の現在の状態。|
|ID|文字列|エンティティのキー。|
|バージョン|文字列|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



