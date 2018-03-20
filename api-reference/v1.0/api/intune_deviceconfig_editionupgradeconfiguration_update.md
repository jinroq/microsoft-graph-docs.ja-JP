# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="ff7a6-101">editionUpgradeConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ff7a6-101">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="ff7a6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff7a6-103">[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-103">Update the properties of a [calendar](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff7a6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff7a6-104">Prerequisites</span></span>
<span data-ttu-id="ff7a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff7a6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff7a6-107">Permission type</span></span>|<span data-ttu-id="ff7a6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff7a6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff7a6-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff7a6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ff7a6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff7a6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff7a6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff7a6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff7a6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-112">Not supported.</span></span>|
|<span data-ttu-id="ff7a6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff7a6-113">Application</span></span>|<span data-ttu-id="ff7a6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff7a6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff7a6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff7a6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff7a6-116">Request headers</span></span>
|<span data-ttu-id="ff7a6-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff7a6-117">Header</span></span>|<span data-ttu-id="ff7a6-118">値</span><span class="sxs-lookup"><span data-stu-id="ff7a6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff7a6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff7a6-119">Authorization</span></span>|<span data-ttu-id="ff7a6-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ff7a6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ff7a6-121">Accept</span></span>|<span data-ttu-id="ff7a6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ff7a6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff7a6-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff7a6-123">Request body</span></span>
<span data-ttu-id="ff7a6-124">要求本文では、[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="ff7a6-125">次の表に、[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ff7a6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff7a6-126">Property</span></span>|<span data-ttu-id="ff7a6-127">型</span><span class="sxs-lookup"><span data-stu-id="ff7a6-127">Type</span></span>|<span data-ttu-id="ff7a6-128">説明</span><span class="sxs-lookup"><span data-stu-id="ff7a6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7a6-129">id</span><span class="sxs-lookup"><span data-stu-id="ff7a6-129">id</span></span>|<span data-ttu-id="ff7a6-130">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-130">String</span></span>|<span data-ttu-id="ff7a6-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-131">Name of the entity.</span></span> <span data-ttu-id="ff7a6-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff7a6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ff7a6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff7a6-134">DateTimeOffset</span></span>|<span data-ttu-id="ff7a6-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="ff7a6-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff7a6-137">createdDateTime</span></span>|<span data-ttu-id="ff7a6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff7a6-138">DateTimeOffset</span></span>|<span data-ttu-id="ff7a6-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-139">DateTime the object was created.</span></span> <span data-ttu-id="ff7a6-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-141">description</span><span class="sxs-lookup"><span data-stu-id="ff7a6-141">description</span></span>|<span data-ttu-id="ff7a6-142">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-142">String</span></span>|<span data-ttu-id="ff7a6-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff7a6-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ff7a6-145">displayName</span></span>|<span data-ttu-id="ff7a6-146">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-146">String</span></span>|<span data-ttu-id="ff7a6-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff7a6-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-149">version</span><span class="sxs-lookup"><span data-stu-id="ff7a6-149">version</span></span>|<span data-ttu-id="ff7a6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ff7a6-150">Int32</span></span>|<span data-ttu-id="ff7a6-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-151">Version of the device configuration.</span></span> <span data-ttu-id="ff7a6-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff7a6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff7a6-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="ff7a6-153">licenseType</span></span>|<span data-ttu-id="ff7a6-154">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-154">String</span></span>|<span data-ttu-id="ff7a6-155">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="ff7a6-156">可能な値は、`productKey`、`licenseFile` です。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="ff7a6-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="ff7a6-157">targetEdition</span></span>|<span data-ttu-id="ff7a6-158">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-158">String</span></span>|<span data-ttu-id="ff7a6-159">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="ff7a6-160">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN` です。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="ff7a6-161">license</span><span class="sxs-lookup"><span data-stu-id="ff7a6-161">License</span></span>|<span data-ttu-id="ff7a6-162">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-162">String</span></span>|<span data-ttu-id="ff7a6-163">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="ff7a6-164">productKey</span><span class="sxs-lookup"><span data-stu-id="ff7a6-164">productKey</span></span>|<span data-ttu-id="ff7a6-165">String</span><span class="sxs-lookup"><span data-stu-id="ff7a6-165">String</span></span>|<span data-ttu-id="ff7a6-166">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="ff7a6-167">応答</span><span class="sxs-lookup"><span data-stu-id="ff7a6-167">Response</span></span>
<span data-ttu-id="ff7a6-168">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-168">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff7a6-169">例</span><span class="sxs-lookup"><span data-stu-id="ff7a6-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff7a6-170">要求</span><span class="sxs-lookup"><span data-stu-id="ff7a6-170">Request</span></span>
<span data-ttu-id="ff7a6-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 309

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="ff7a6-172">応答</span><span class="sxs-lookup"><span data-stu-id="ff7a6-172">Response</span></span>
<span data-ttu-id="ff7a6-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff7a6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



