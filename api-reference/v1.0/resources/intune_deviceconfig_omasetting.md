# <a name="omasetting-resource-type"></a>omaSetting リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

OMA 設定の定義。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列|表示名。|
|説明|文字列|説明。|
|omaUri|文字列|OMA。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```








