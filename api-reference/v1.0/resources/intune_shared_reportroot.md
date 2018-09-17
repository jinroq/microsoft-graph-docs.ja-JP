# <a name="reportroot-resource-type"></a>reportRoot リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

履歴レポートのインスタンスを表すリソースです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ReportRoot の取得](../api/intune_shared_reportroot_get.md)|[reportRoot](../resources/intune_shared_reportroot.md)|[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[reportRoot の更新](../api/intune_shared_reportroot_update.md)|[reportRoot](../resources/intune_shared_reportroot.md)|[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトのプロパティを更新します。|
|**デバイス構成**|
|[deviceConfigurationDeviceActivity 関数](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[レポート](../resources/intune_shared_report.md)|デバイス構成のデバイス アクティビティ レポートのメタデータ|
|[deviceConfigurationUserActivity 関数](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[レポート](../resources/intune_shared_report.md)|デバイス構成のユーザー アクティビティ レポートのメタデータ|
|**トラブルシューティング**|
|[managedDeviceEnrollmentFailureDetails 関数](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[レポート](../resources/intune_shared_report.md)|まだ文書化されていません。|
|[managedDeviceEnrollmentTopFailures 関数](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[レポート](../resources/intune_shared_report.md)|まだ文書化されていません。|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|このエンティティの一意識別子です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```