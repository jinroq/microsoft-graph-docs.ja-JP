# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List remoteAssistancePartners](../api/intune_remoteassistance_remoteassistancepartner_list.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) コレクション|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|新しい [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトを作成します。|
|[Delete remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|なし|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) を削除します。|
|[Update remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティを更新します。|
|[beginOnboarding アクション](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|なし|まだ文書化されていません|
|[disconnect アクション](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|String|パートナーの一意識別子。|
|displayName|String|パートナーの表示名。|
|onboardingUrl|String|パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|未定 可能な値は、 `notOnboarded`、`onboarding`、`onboarded` です。|
|lastConnectionDateTime|DateTimeOffset|TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```



