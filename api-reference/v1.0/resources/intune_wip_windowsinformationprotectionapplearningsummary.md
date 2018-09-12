# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護アプリの学習概要エンティティ。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsInformationProtectionAppLearningSummaries の一覧表示](../api/intune_wip_windowsinformationprotectionapplearningsummary_list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) コレクション|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsInformationProtectionAppLearningSummary の取得](../api/intune_wip_windowsinformationprotectionapplearningsummary_get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsInformationProtectionAppLearningSummary の作成](../api/intune_wip_windowsinformationprotectionapplearningsummary_create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|新しい [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。|
|[windowsInformationProtectionAppLearningSummary の削除](../api/intune_wip_windowsinformationprotectionapplearningsummary_delete.md)|なし|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) を削除します。|
|[windowsInformationProtectionAppLearningSummary の更新](../api/intune_wip_windowsinformationprotectionapplearningsummary_update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|WindowsInformationProtectionAppLearningSummary の一意識別子。|
|applicationName|文字列|アプリケーション名|
|applicationType|[applicationType](../resources/intune_wip_applicationtype.md)|アプリケーションの種類。 使用可能な値は、`universal`、`desktop` です。|
|deviceCount|Int32|デバイス数|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```








