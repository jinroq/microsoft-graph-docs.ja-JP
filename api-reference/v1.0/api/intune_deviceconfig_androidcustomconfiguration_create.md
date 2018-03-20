# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="86c4d-101">androidCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="86c4d-101">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="86c4d-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86c4d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86c4d-103">新しい [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="86c4d-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86c4d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="86c4d-104">Prerequisites</span></span>
<span data-ttu-id="86c4d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86c4d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86c4d-107">Permission type</span></span>|<span data-ttu-id="86c4d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86c4d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c4d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86c4d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="86c4d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c4d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86c4d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86c4d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c4d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c4d-112">Not supported.</span></span>|
|<span data-ttu-id="86c4d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86c4d-113">Application</span></span>|<span data-ttu-id="86c4d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c4d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c4d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86c4d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86c4d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c4d-116">Request headers</span></span>
|<span data-ttu-id="86c4d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c4d-117">Header</span></span>|<span data-ttu-id="86c4d-118">値</span><span class="sxs-lookup"><span data-stu-id="86c4d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c4d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c4d-119">Authorization</span></span>|<span data-ttu-id="86c4d-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="86c4d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86c4d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="86c4d-121">Accept</span></span>|<span data-ttu-id="86c4d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="86c4d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c4d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="86c4d-123">Request body</span></span>
<span data-ttu-id="86c4d-124">要求本文で、androidCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="86c4d-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="86c4d-125">次の表に、androidCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="86c4d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="86c4d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86c4d-126">Property</span></span>|<span data-ttu-id="86c4d-127">型</span><span class="sxs-lookup"><span data-stu-id="86c4d-127">Type</span></span>|<span data-ttu-id="86c4d-128">説明</span><span class="sxs-lookup"><span data-stu-id="86c4d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c4d-129">id</span><span class="sxs-lookup"><span data-stu-id="86c4d-129">id</span></span>|<span data-ttu-id="86c4d-130">String</span><span class="sxs-lookup"><span data-stu-id="86c4d-130">String</span></span>|<span data-ttu-id="86c4d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="86c4d-131">Name of the entity.</span></span> <span data-ttu-id="86c4d-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86c4d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="86c4d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c4d-134">DateTimeOffset</span></span>|<span data-ttu-id="86c4d-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="86c4d-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="86c4d-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86c4d-137">createdDateTime</span></span>|<span data-ttu-id="86c4d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c4d-138">DateTimeOffset</span></span>|<span data-ttu-id="86c4d-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="86c4d-139">DateTime the object was created.</span></span> <span data-ttu-id="86c4d-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-141">description</span><span class="sxs-lookup"><span data-stu-id="86c4d-141">description</span></span>|<span data-ttu-id="86c4d-142">String</span><span class="sxs-lookup"><span data-stu-id="86c4d-142">String</span></span>|<span data-ttu-id="86c4d-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="86c4d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86c4d-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="86c4d-145">displayName</span></span>|<span data-ttu-id="86c4d-146">String</span><span class="sxs-lookup"><span data-stu-id="86c4d-146">String</span></span>|<span data-ttu-id="86c4d-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="86c4d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86c4d-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-149">version</span><span class="sxs-lookup"><span data-stu-id="86c4d-149">version</span></span>|<span data-ttu-id="86c4d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="86c4d-150">Int32</span></span>|<span data-ttu-id="86c4d-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="86c4d-151">Version of the device configuration.</span></span> <span data-ttu-id="86c4d-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86c4d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86c4d-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="86c4d-153">omaSettings</span></span>|<span data-ttu-id="86c4d-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="86c4d-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="86c4d-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="86c4d-155">OMA settings.</span></span> <span data-ttu-id="86c4d-156">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="86c4d-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="86c4d-157">応答</span><span class="sxs-lookup"><span data-stu-id="86c4d-157">Response</span></span>
<span data-ttu-id="86c4d-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="86c4d-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c4d-159">例</span><span class="sxs-lookup"><span data-stu-id="86c4d-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="86c4d-160">要求</span><span class="sxs-lookup"><span data-stu-id="86c4d-160">Request</span></span>
<span data-ttu-id="86c4d-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86c4d-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="86c4d-162">応答</span><span class="sxs-lookup"><span data-stu-id="86c4d-162">Response</span></span>
<span data-ttu-id="86c4d-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86c4d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



