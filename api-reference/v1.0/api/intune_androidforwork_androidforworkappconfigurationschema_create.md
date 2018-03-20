# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="69709-101">androidForWorkAppConfigurationSchema の作成</span><span class="sxs-lookup"><span data-stu-id="69709-101">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="69709-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="69709-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69709-103">新しい [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="69709-103">Create a new [plannerBucket](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69709-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="69709-104">Prerequisites</span></span>
<span data-ttu-id="69709-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69709-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69709-107">Permission type</span></span>|<span data-ttu-id="69709-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69709-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69709-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69709-109">Delegated (work or school account)</span></span>|<span data-ttu-id="69709-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69709-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69709-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69709-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69709-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69709-112">Not supported.</span></span>|
|<span data-ttu-id="69709-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69709-113">Application</span></span>|<span data-ttu-id="69709-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69709-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69709-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69709-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="69709-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69709-116">Request headers</span></span>
|<span data-ttu-id="69709-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69709-117">Header</span></span>|<span data-ttu-id="69709-118">値</span><span class="sxs-lookup"><span data-stu-id="69709-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69709-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="69709-119">Authorization</span></span>|<span data-ttu-id="69709-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="69709-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69709-121">Accept</span><span class="sxs-lookup"><span data-stu-id="69709-121">Accept</span></span>|<span data-ttu-id="69709-122">application/json</span><span class="sxs-lookup"><span data-stu-id="69709-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69709-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="69709-123">Request body</span></span>
<span data-ttu-id="69709-124">要求本文で、androidForWorkAppConfigurationSchema オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69709-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="69709-125">次の表に、androidForWorkAppConfigurationSchema の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69709-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="69709-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69709-126">Property</span></span>|<span data-ttu-id="69709-127">型</span><span class="sxs-lookup"><span data-stu-id="69709-127">Type</span></span>|<span data-ttu-id="69709-128">説明</span><span class="sxs-lookup"><span data-stu-id="69709-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69709-129">id</span><span class="sxs-lookup"><span data-stu-id="69709-129">id</span></span>|<span data-ttu-id="69709-130">String</span><span class="sxs-lookup"><span data-stu-id="69709-130">String</span></span>|<span data-ttu-id="69709-131">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="69709-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="69709-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="69709-132">exampleJson</span></span>|<span data-ttu-id="69709-133">Binary</span><span class="sxs-lookup"><span data-stu-id="69709-133">Binary</span></span>|<span data-ttu-id="69709-134">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="69709-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="69709-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="69709-135">schemaItems</span></span>|<span data-ttu-id="69709-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="69709-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="69709-137">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="69709-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="69709-138">応答</span><span class="sxs-lookup"><span data-stu-id="69709-138">Response</span></span>
<span data-ttu-id="69709-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69709-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69709-140">例</span><span class="sxs-lookup"><span data-stu-id="69709-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="69709-141">要求</span><span class="sxs-lookup"><span data-stu-id="69709-141">Request</span></span>
<span data-ttu-id="69709-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69709-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
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

### <a name="response"></a><span data-ttu-id="69709-143">応答</span><span class="sxs-lookup"><span data-stu-id="69709-143">Response</span></span>
<span data-ttu-id="69709-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69709-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



