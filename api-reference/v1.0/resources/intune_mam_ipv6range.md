# <a name="ipv6range-resource-type"></a>iPv6Range リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

IP V6 の範囲

[ipRange](../resources/intune_mam_iprange.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lowerAddress|文字列|低い番号の IP アドレス|
|upperAddress|文字列|高い番号の IP アドレス|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```








