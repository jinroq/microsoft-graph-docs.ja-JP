# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="f6e71-101">windowsDefenderAdvancedThreatProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="f6e71-101">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="f6e71-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6e71-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6e71-103">新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6e71-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6e71-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6e71-104">Prerequisites</span></span>
<span data-ttu-id="f6e71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6e71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6e71-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6e71-107">Permission type</span></span>|<span data-ttu-id="f6e71-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6e71-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6e71-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6e71-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f6e71-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e71-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6e71-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6e71-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6e71-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6e71-112">Not supported.</span></span>|
|<span data-ttu-id="f6e71-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6e71-113">Application</span></span>|<span data-ttu-id="f6e71-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6e71-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6e71-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6e71-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6e71-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6e71-116">Request headers</span></span>
|<span data-ttu-id="f6e71-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6e71-117">Header</span></span>|<span data-ttu-id="f6e71-118">値</span><span class="sxs-lookup"><span data-stu-id="f6e71-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6e71-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6e71-119">Authorization</span></span>|<span data-ttu-id="f6e71-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6e71-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f6e71-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f6e71-121">Accept</span></span>|<span data-ttu-id="f6e71-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f6e71-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6e71-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6e71-123">Request body</span></span>
<span data-ttu-id="f6e71-124">要求本文で、windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6e71-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f6e71-125">次の表に、windowsDefenderAdvancedThreatProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f6e71-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f6e71-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6e71-126">Property</span></span>|<span data-ttu-id="f6e71-127">型</span><span class="sxs-lookup"><span data-stu-id="f6e71-127">Type</span></span>|<span data-ttu-id="f6e71-128">説明</span><span class="sxs-lookup"><span data-stu-id="f6e71-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e71-129">id</span><span class="sxs-lookup"><span data-stu-id="f6e71-129">id</span></span>|<span data-ttu-id="f6e71-130">String</span><span class="sxs-lookup"><span data-stu-id="f6e71-130">String</span></span>|<span data-ttu-id="f6e71-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f6e71-131">Name of the entity.</span></span> <span data-ttu-id="f6e71-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6e71-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f6e71-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6e71-134">DateTimeOffset</span></span>|<span data-ttu-id="f6e71-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f6e71-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="f6e71-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6e71-137">createdDateTime</span></span>|<span data-ttu-id="f6e71-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6e71-138">DateTimeOffset</span></span>|<span data-ttu-id="f6e71-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f6e71-139">DateTime the object was created.</span></span> <span data-ttu-id="f6e71-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-141">description</span><span class="sxs-lookup"><span data-stu-id="f6e71-141">description</span></span>|<span data-ttu-id="f6e71-142">String</span><span class="sxs-lookup"><span data-stu-id="f6e71-142">String</span></span>|<span data-ttu-id="f6e71-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f6e71-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6e71-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f6e71-145">displayName</span></span>|<span data-ttu-id="f6e71-146">String</span><span class="sxs-lookup"><span data-stu-id="f6e71-146">String</span></span>|<span data-ttu-id="f6e71-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f6e71-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6e71-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-149">version</span><span class="sxs-lookup"><span data-stu-id="f6e71-149">version</span></span>|<span data-ttu-id="f6e71-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e71-150">Int32</span></span>|<span data-ttu-id="f6e71-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f6e71-151">Version of the device configuration.</span></span> <span data-ttu-id="f6e71-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6e71-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e71-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="f6e71-153">allowSampleSharing</span></span>|<span data-ttu-id="f6e71-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6e71-154">Boolean</span></span>|<span data-ttu-id="f6e71-155">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="f6e71-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="f6e71-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="f6e71-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="f6e71-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6e71-157">Boolean</span></span>|<span data-ttu-id="f6e71-158">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="f6e71-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="f6e71-159">応答</span><span class="sxs-lookup"><span data-stu-id="f6e71-159">Response</span></span>
<span data-ttu-id="f6e71-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6e71-160">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6e71-161">例</span><span class="sxs-lookup"><span data-stu-id="f6e71-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6e71-162">要求</span><span class="sxs-lookup"><span data-stu-id="f6e71-162">Request</span></span>
<span data-ttu-id="f6e71-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6e71-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="f6e71-164">応答</span><span class="sxs-lookup"><span data-stu-id="f6e71-164">Response</span></span>
<span data-ttu-id="f6e71-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6e71-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



