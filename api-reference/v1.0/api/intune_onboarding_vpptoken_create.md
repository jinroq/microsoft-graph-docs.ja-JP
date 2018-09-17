# <a name="create-vpptoken"></a>vppToken の作成

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新規に[vppToken](../resources/intune_onboarding_vpptoken.md)オブジェクトを作成します。
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
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|承諾|アプリケーションまたは json|

## <a name="request-body"></a>要求本文
要求本文で、vppToken オブジェクトの JSON 表記を指定します。

次の表に、vppToken 作成時に必要なプロパティを示します。

|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|appleVolumePurchaseProgramToken 作成時に自動的に生成されます。 エンティティのキーになります。|
|organizationName|文字列|Apple Volume Purchase Program のトークンに関連付けられている組織|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune_shared_vpptokenaccounttype.md)|特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類です。指定できる値は、`business`、`education` です。指定できる値は、`business`、`education` です。|
|appleId|文字列|特定の Apple Volume Purchase Program のトークンに関連付けられている Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンの有効期限。|
|lastSyncDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。|
|token|文字列|Apple Volume Purchase Program からダウンロードした Apple ボリューム購入プログラムのトークン文字列。|
|lastModifiedDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンに関連付けられている最終変更日時。|
|都道府県|[vppTokenState](../resources/intune_onboarding_vpptokenstate.md)|Apple ボリューム購入プログラム トークンの現在の状態。指定できる値は`unknown`、 `valid`、 `expired`、 `invalid`、 `assignedToExternalMDM`。指定できる値は`unknown`、 `valid`、 `expired`、 `invalid`、 `assignedToExternalMDM`。|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune_onboarding_vpptokensyncstatus.md)|Apple ボリューム購入プログラム トークンを使用して発生した最後のアプリケーションの同期の現在の同期の状態です。指定できる値は`none`、 `inProgress`、 `completed`、 `failed`。指定できる値は`none`、 `inProgress`、 `completed`、 `failed`。|
|automaticallyUpdateApps|ブール型|VPP トークンのアプリを自動で更新するかどうか。|
|countryOrRegion|文字列|VPP トークンのアプリを自動で更新するかどうか。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [vppToken](../resources/intune_onboarding_vpptoken.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```








