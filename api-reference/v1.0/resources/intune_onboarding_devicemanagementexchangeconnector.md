# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Exchange 環境との接続を表すエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagementExchangeConnectors をリストする](../api/intune_onboarding_devicemanagementexchangeconnector_list.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) コレクション|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceManagementExchangeConnector を取得する](../api/intune_onboarding_devicemanagementexchangeconnector_get.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagementExchangeConnector を作成する](../api/intune_onboarding_devicemanagementexchangeconnector_create.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|新しい [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトを作成します。|
|[deviceManagementExchangeConnector を削除する](../api/intune_onboarding_devicemanagementexchangeconnector_delete.md)|なし|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) を削除します。|
|[deviceManagementExchangeConnector を更新する](../api/intune_onboarding_devicemanagementexchangeconnector_update.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。|
|[同期アクション](../api/intune_onboarding_devicemanagementexchangeconnector_sync.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|まだ文書化されていません|
|lastSyncDateTime|DateTimeOffset|Exchange Connector の最終同期日時|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|Exchange コネクタの状態。 指定できる値は、`none`、`connectionPending`、`connected`、`disconnected` です。|
|primarySmtpAddress|文字列|サービス間の Exchange Connector を構成するときに使用するメール アドレス。|
|serverName|文字列|Exchange サーバーの名前。|
|connectorServerName|文字列|Exchange Connector をホストするサーバーの名前。|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|構成されている Exchange Connector の種類。 指定できる値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。|
|version|文字列|ExchangeConnectorAgent のバージョン|
|exchangeAlias|文字列|Exchange Server に割り当てられているエイリアス。|
|exchangeOrganization|文字列|Exchange Server に対する Exchange 組織|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```



