# <a name="edgesearchengine-resource-type"></a>edgeSearchEngine リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。

[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune_deviceconfig_edgesearchenginetype.md)|MDM 管理対象デバイス用の定義済みの既定の検索エンジンを設定するのには、IT 管理者を使用できます。使用可能な値: `default`、 `bing`。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```








