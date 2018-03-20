# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="baa3e-101">androidForWorkAppConfigurationSchema の更新</span><span class="sxs-lookup"><span data-stu-id="baa3e-101">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="baa3e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="baa3e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baa3e-103">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="baa3e-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baa3e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="baa3e-104">Prerequisites</span></span>
<span data-ttu-id="baa3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baa3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="baa3e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baa3e-107">Permission type</span></span>|<span data-ttu-id="baa3e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="baa3e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baa3e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baa3e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="baa3e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa3e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="baa3e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baa3e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baa3e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baa3e-112">Not supported.</span></span>|
|<span data-ttu-id="baa3e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baa3e-113">Application</span></span>|<span data-ttu-id="baa3e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baa3e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baa3e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baa3e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="baa3e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baa3e-116">Request headers</span></span>
|<span data-ttu-id="baa3e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baa3e-117">Header</span></span>|<span data-ttu-id="baa3e-118">値</span><span class="sxs-lookup"><span data-stu-id="baa3e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baa3e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa3e-119">Authorization</span></span>|<span data-ttu-id="baa3e-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="baa3e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="baa3e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="baa3e-121">Accept</span></span>|<span data-ttu-id="baa3e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="baa3e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baa3e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="baa3e-123">Request body</span></span>
<span data-ttu-id="baa3e-124">要求本文で、[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="baa3e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="baa3e-125">次の表に、a[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="baa3e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="baa3e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baa3e-126">Property</span></span>|<span data-ttu-id="baa3e-127">型</span><span class="sxs-lookup"><span data-stu-id="baa3e-127">Type</span></span>|<span data-ttu-id="baa3e-128">説明</span><span class="sxs-lookup"><span data-stu-id="baa3e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa3e-129">id</span><span class="sxs-lookup"><span data-stu-id="baa3e-129">id</span></span>|<span data-ttu-id="baa3e-130">String</span><span class="sxs-lookup"><span data-stu-id="baa3e-130">String</span></span>|<span data-ttu-id="baa3e-131">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="baa3e-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="baa3e-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="baa3e-132">exampleJson</span></span>|<span data-ttu-id="baa3e-133">Binary</span><span class="sxs-lookup"><span data-stu-id="baa3e-133">Binary</span></span>|<span data-ttu-id="baa3e-134">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="baa3e-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="baa3e-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="baa3e-135">schemaItems</span></span>|<span data-ttu-id="baa3e-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="baa3e-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="baa3e-137">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="baa3e-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="baa3e-138">応答</span><span class="sxs-lookup"><span data-stu-id="baa3e-138">Response</span></span>
<span data-ttu-id="baa3e-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="baa3e-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baa3e-140">例</span><span class="sxs-lookup"><span data-stu-id="baa3e-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="baa3e-141">要求</span><span class="sxs-lookup"><span data-stu-id="baa3e-141">Request</span></span>
<span data-ttu-id="baa3e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="baa3e-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="baa3e-143">応答</span><span class="sxs-lookup"><span data-stu-id="baa3e-143">Response</span></span>
<span data-ttu-id="baa3e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="baa3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



