# <a name="applistitem-resource-type"></a>appListItem リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象アプリケーションの一覧にあるアプリを表します
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|文字列型 (String)|アプリケーション名|
|発行元|文字列型 (String)|アプリケーションの発行元|
|appStoreUrl|文字列型 (String)|アプリケーションのストア URL|
|appId|文字列型 (String)|アプリケーションのアプリケーションまたはバンドルの識別子|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



