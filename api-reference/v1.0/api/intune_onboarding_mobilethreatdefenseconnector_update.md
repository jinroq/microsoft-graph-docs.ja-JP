# <a name="update-mobilethreatdefenseconnector"></a>mobileThreatDefenseConnector の更新

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt;が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトの JSON 表記を指定します。

次の表に、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|lastHeartbeatDateTime|DateTimeOffset|管理者が MTP への接続オプションを有効にした後の、最後のハートビートのタイムスタンプ|
|partnerState|String|このテナントのパートナーの状態。可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。|
|androidEnabled|Boolean|Android のオンまたはオフの切り替え|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Android の場合、準拠していると判断される前にデータ同期のパートナーからデータを受信する必要がある旨、管理者が構成できるようにします|
|iosDeviceBlockedOnMissingPartnerData|Boolean|iOS の場合、準拠していると判断される前にデータ同期のパートナーからデータを受信する必要がある旨、管理者が構成できるようにします|
|partnerUnsupportedOsVersionBlocked|Boolean|最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスを、管理者がブロックできるようにします|
|iosEnabled|Boolean|iOS のオンまたはオフの切り替え|
|partnerUnresponsivenessThresholdInDays|Int32|このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを応答本文で返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



