# <a name="create-mobilethreatdefenseconnector"></a>Create mobileThreatDefenseConnector

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校アカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。

次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|lastHeartbeatDateTime|DateTimeOffset|管理者が MTP へのオプション接続を有効にした後の、最後のハートビートのタイムスタンプ|
|partnerState|String|このテナントのパートナーの状態です。可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。|
|androidEnabled|Boolean|Android 切り替えのオンまたはオフ|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Android において、管理者がデータ同期パートナーの準拠を判断する前に、データ同期パートナーからの受信必須データを設定できるようにします|
|iosDeviceBlockedOnMissingPartnerData|Boolean|iOS の場合、管理者がデータ同期パートナーの準拠を判断する前に、データ同期パートナーからの受信必須データを設定できるようにします|
|partnerUnsupportedOsVersionBlocked|Boolean|有効にされたプラットフォーム上にあっても最低バージョン要件を満たさないデバイスを管理者がブロックできるようにします|
|iosEnabled|Boolean|iOS 切り替えのオンまたはオフ|
|partnerUnresponsivenessThresholdInDays|Int32|このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
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
HTTP/1.1 201 Created
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



