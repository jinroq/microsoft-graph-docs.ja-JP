# <a name="vpplicensingtype-resource-type"></a>vppLicensingType リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|supportsUserLicensing|ブール型 (Boolean)|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportsDeviceLicensing|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



