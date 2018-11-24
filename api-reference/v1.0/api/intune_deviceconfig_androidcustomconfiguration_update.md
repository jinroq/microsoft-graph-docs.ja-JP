# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="e3bac-101">androidCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e3bac-101">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="e3bac-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3bac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3bac-103">[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3bac-103">Update the properties of a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3bac-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3bac-104">Prerequisites</span></span>
<span data-ttu-id="e3bac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3bac-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3bac-107">Permission type</span></span>|<span data-ttu-id="e3bac-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3bac-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3bac-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3bac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e3bac-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3bac-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3bac-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3bac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3bac-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3bac-112">Not supported.</span></span>|
|<span data-ttu-id="e3bac-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3bac-113">Application</span></span>|<span data-ttu-id="e3bac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3bac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3bac-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3bac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e3bac-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3bac-116">Request headers</span></span>
|<span data-ttu-id="e3bac-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3bac-117">Header</span></span>|<span data-ttu-id="e3bac-118">値</span><span class="sxs-lookup"><span data-stu-id="e3bac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3bac-119">承認</span><span class="sxs-lookup"><span data-stu-id="e3bac-119">Authorization</span></span>|<span data-ttu-id="e3bac-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="e3bac-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3bac-121">承諾</span><span class="sxs-lookup"><span data-stu-id="e3bac-121">Accept</span></span>|<span data-ttu-id="e3bac-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e3bac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3bac-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3bac-123">Request body</span></span>
<span data-ttu-id="e3bac-124">要求本文で、[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3bac-124">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="e3bac-125">次の表に、[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3bac-125">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="e3bac-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3bac-126">Property</span></span>|<span data-ttu-id="e3bac-127">型</span><span class="sxs-lookup"><span data-stu-id="e3bac-127">Type</span></span>|<span data-ttu-id="e3bac-128">説明</span><span class="sxs-lookup"><span data-stu-id="e3bac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3bac-129">id</span><span class="sxs-lookup"><span data-stu-id="e3bac-129">id</span></span>|<span data-ttu-id="e3bac-130">String</span><span class="sxs-lookup"><span data-stu-id="e3bac-130">String</span></span>|<span data-ttu-id="e3bac-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3bac-131">Key of the entity.</span></span> <span data-ttu-id="e3bac-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3bac-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e3bac-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3bac-134">DateTimeOffset</span></span>|<span data-ttu-id="e3bac-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e3bac-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e3bac-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3bac-137">createdDateTime</span></span>|<span data-ttu-id="e3bac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3bac-138">DateTimeOffset</span></span>|<span data-ttu-id="e3bac-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e3bac-139">DateTime the object was created.</span></span> <span data-ttu-id="e3bac-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-141">description</span><span class="sxs-lookup"><span data-stu-id="e3bac-141">description</span></span>|<span data-ttu-id="e3bac-142">String</span><span class="sxs-lookup"><span data-stu-id="e3bac-142">String</span></span>|<span data-ttu-id="e3bac-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e3bac-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e3bac-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e3bac-145">displayName</span></span>|<span data-ttu-id="e3bac-146">String</span><span class="sxs-lookup"><span data-stu-id="e3bac-146">String</span></span>|<span data-ttu-id="e3bac-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e3bac-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e3bac-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-149">version</span><span class="sxs-lookup"><span data-stu-id="e3bac-149">version</span></span>|<span data-ttu-id="e3bac-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e3bac-150">Int32</span></span>|<span data-ttu-id="e3bac-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e3bac-151">Version of the device configuration.</span></span> <span data-ttu-id="e3bac-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3bac-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3bac-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e3bac-153">omaSettings</span></span>|<span data-ttu-id="e3bac-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3bac-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="e3bac-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="e3bac-155">OMA settings.</span></span> <span data-ttu-id="e3bac-156">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e3bac-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e3bac-157">応答</span><span class="sxs-lookup"><span data-stu-id="e3bac-157">Response</span></span>
<span data-ttu-id="e3bac-158">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e3bac-158">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3bac-159">例</span><span class="sxs-lookup"><span data-stu-id="e3bac-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3bac-160">要求</span><span class="sxs-lookup"><span data-stu-id="e3bac-160">Request</span></span>
<span data-ttu-id="e3bac-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3bac-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="e3bac-162">応答</span><span class="sxs-lookup"><span data-stu-id="e3bac-162">Response</span></span>
<span data-ttu-id="e3bac-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3bac-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



