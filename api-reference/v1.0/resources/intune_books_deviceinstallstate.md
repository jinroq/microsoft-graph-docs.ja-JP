# <a name="deviceinstallstate-resource-type"></a>deviceInstallState リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスのインストール状態のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceInstallStates のリスト](../api/intune_books_deviceinstallstate_list.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceInstallState の取得](../api/intune_books_deviceinstallstate_get.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceInstallState の作成](../api/intune_books_deviceinstallstate_create.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|新しい [deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトを作成します。|
|[deviceInstallState の削除](../api/intune_books_deviceinstallstate_delete.md)|なし|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) を削除します。|
|[deviceInstallState の更新](../api/intune_books_deviceinstallstate_update.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|deviceName|文字列|デバイス名。|
|deviceId|文字列|デバイス ID。|
|lastSyncDateTime|DateTimeOffset|最後の同期日時。|
|installState|[installState](../resources/intune_books_installstate.md)|電子ブックのインストールの状態。 指定できる値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。|
|errorCode|文字列|インストール失敗のエラー コード。|
|osVersion|文字列|OS バージョン。|
|osDescription|文字列|OS の説明。|
|userName|文字列|デバイスのユーザー名です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceInstallState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



