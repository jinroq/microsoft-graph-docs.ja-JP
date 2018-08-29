# <a name="ioshomescreenapp-resource-type"></a>iosHomeScreenApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ホーム画面上のアプリのアイコンを表します

[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|アプリの名前。[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) から継承|
|bundleID|文字列型 (String)|アプリの BundleID|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.iosHomeScreenItem",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



