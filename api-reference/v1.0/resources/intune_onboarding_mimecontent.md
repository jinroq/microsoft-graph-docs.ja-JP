# <a name="mimecontent-resource-type"></a>mimeContent リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

汎用 MIME コンテンツのプロパティが含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|type|文字列|MIME タイプのコンテンツを示します。|
|値|バイナリ|実際のコンテンツを含むバイト配列です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



