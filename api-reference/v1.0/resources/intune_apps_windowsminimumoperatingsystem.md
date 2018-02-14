# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows モバイル アプリに必要な最小オペレーティング システム。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v8_0|ブール型 (Boolean)|Windows バージョン 8.0 以降。|
|v8_1|ブール型 (Boolean)|Windows バージョン 8.1 以降。|
|v10_0|ブール型 (Boolean)|Windows バージョン 10.0 以降。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



