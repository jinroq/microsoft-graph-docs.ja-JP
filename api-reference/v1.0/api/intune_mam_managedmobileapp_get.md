# <a name="get-managedmobileapp"></a>Get managedMobileApp

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|Accept|アプリケーションまたは json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```








