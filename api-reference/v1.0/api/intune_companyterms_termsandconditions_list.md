# <a name="list-termsandconditionses"></a>termsAndConditionses のリスト

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトのプロパティとリレーションシップをリストします。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|Accept|アプリケーションまたは json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```








