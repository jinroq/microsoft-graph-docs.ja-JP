# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

組織アプリの保護と構成についての型指定されていない進捗レポートを表します。

[managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAppStatusRaws のリスト](../api/intune_mam_managedappstatusraw_list.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) コレクション|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAppStatusRaw の取得](../api/intune_mam_managedappstatusraw_get.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|進捗レポートのフレンドリ名。 [managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します|
|id|String|エンティティのキー。 [managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します|
|content|[Json](../resources/intune_mam_json.md)|進捗レポートの内容。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



