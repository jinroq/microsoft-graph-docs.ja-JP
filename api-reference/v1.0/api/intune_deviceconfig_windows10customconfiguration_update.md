# <a name="update-windows10customconfiguration"></a><span data-ttu-id="acc2f-101">windows10CustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="acc2f-101">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="acc2f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="acc2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acc2f-103">[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="acc2f-103">Update the properties of a [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acc2f-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="acc2f-104">Prerequisites</span></span>
<span data-ttu-id="acc2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acc2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="acc2f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acc2f-107">Permission type</span></span>|<span data-ttu-id="acc2f-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="acc2f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acc2f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acc2f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="acc2f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc2f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acc2f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acc2f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acc2f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acc2f-112">Not supported.</span></span>|
|<span data-ttu-id="acc2f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acc2f-113">Application</span></span>|<span data-ttu-id="acc2f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acc2f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acc2f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acc2f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="acc2f-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acc2f-116">Request headers</span></span>
|<span data-ttu-id="acc2f-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acc2f-117">Header</span></span>|<span data-ttu-id="acc2f-118">値</span><span class="sxs-lookup"><span data-stu-id="acc2f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acc2f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="acc2f-119">Authorization</span></span>|<span data-ttu-id="acc2f-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="acc2f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acc2f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="acc2f-121">Accept</span></span>|<span data-ttu-id="acc2f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="acc2f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acc2f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="acc2f-123">Request body</span></span>
<span data-ttu-id="acc2f-124">要求本文で、[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="acc2f-124">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="acc2f-125">次の表に、[windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="acc2f-125">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span></span>

|<span data-ttu-id="acc2f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acc2f-126">Property</span></span>|<span data-ttu-id="acc2f-127">型</span><span class="sxs-lookup"><span data-stu-id="acc2f-127">Type</span></span>|<span data-ttu-id="acc2f-128">説明</span><span class="sxs-lookup"><span data-stu-id="acc2f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc2f-129">id</span><span class="sxs-lookup"><span data-stu-id="acc2f-129">id</span></span>|<span data-ttu-id="acc2f-130">String</span><span class="sxs-lookup"><span data-stu-id="acc2f-130">String</span></span>|<span data-ttu-id="acc2f-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="acc2f-131">Key of the entity.</span></span> <span data-ttu-id="acc2f-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acc2f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="acc2f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acc2f-134">DateTimeOffset</span></span>|<span data-ttu-id="acc2f-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="acc2f-135">DateTime the object was last modified.</span></span> <span data-ttu-id="acc2f-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acc2f-137">createdDateTime</span></span>|<span data-ttu-id="acc2f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acc2f-138">DateTimeOffset</span></span>|<span data-ttu-id="acc2f-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="acc2f-139">DateTime the object was created.</span></span> <span data-ttu-id="acc2f-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-141">description</span><span class="sxs-lookup"><span data-stu-id="acc2f-141">description</span></span>|<span data-ttu-id="acc2f-142">String</span><span class="sxs-lookup"><span data-stu-id="acc2f-142">String</span></span>|<span data-ttu-id="acc2f-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="acc2f-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="acc2f-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="acc2f-145">displayName</span></span>|<span data-ttu-id="acc2f-146">String</span><span class="sxs-lookup"><span data-stu-id="acc2f-146">String</span></span>|<span data-ttu-id="acc2f-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="acc2f-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="acc2f-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-149">version</span><span class="sxs-lookup"><span data-stu-id="acc2f-149">version</span></span>|<span data-ttu-id="acc2f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="acc2f-150">Int32</span></span>|<span data-ttu-id="acc2f-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="acc2f-151">Version of the device configuration.</span></span> <span data-ttu-id="acc2f-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acc2f-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acc2f-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="acc2f-153">omaSettings</span></span>|<span data-ttu-id="acc2f-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="acc2f-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="acc2f-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="acc2f-155">OMA settings.</span></span> <span data-ttu-id="acc2f-156">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="acc2f-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="acc2f-157">応答</span><span class="sxs-lookup"><span data-stu-id="acc2f-157">Response</span></span>
<span data-ttu-id="acc2f-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="acc2f-158">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acc2f-159">例</span><span class="sxs-lookup"><span data-stu-id="acc2f-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="acc2f-160">要求</span><span class="sxs-lookup"><span data-stu-id="acc2f-160">Request</span></span>
<span data-ttu-id="acc2f-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="acc2f-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="acc2f-162">応答</span><span class="sxs-lookup"><span data-stu-id="acc2f-162">Response</span></span>
<span data-ttu-id="acc2f-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="acc2f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



