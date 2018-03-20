# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="05038-101">editionUpgradeConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="05038-101">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="05038-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05038-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05038-103">新しい [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05038-103">Create a new [plannerBucket](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05038-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="05038-104">Prerequisites</span></span>
<span data-ttu-id="05038-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05038-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05038-107">Permission type</span></span>|<span data-ttu-id="05038-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05038-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05038-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05038-109">Delegated (work or school account)</span></span>|<span data-ttu-id="05038-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05038-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05038-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05038-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05038-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05038-112">Not supported.</span></span>|
|<span data-ttu-id="05038-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05038-113">Application</span></span>|<span data-ttu-id="05038-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05038-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05038-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05038-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05038-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05038-116">Request headers</span></span>
|<span data-ttu-id="05038-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05038-117">Header</span></span>|<span data-ttu-id="05038-118">値</span><span class="sxs-lookup"><span data-stu-id="05038-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05038-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="05038-119">Authorization</span></span>|<span data-ttu-id="05038-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="05038-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05038-121">Accept</span><span class="sxs-lookup"><span data-stu-id="05038-121">Accept</span></span>|<span data-ttu-id="05038-122">application/json</span><span class="sxs-lookup"><span data-stu-id="05038-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05038-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="05038-123">Request body</span></span>
<span data-ttu-id="05038-124">要求本文では、editionUpgradeConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05038-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="05038-125">次の表に、editionUpgradeConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05038-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="05038-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05038-126">Property</span></span>|<span data-ttu-id="05038-127">型</span><span class="sxs-lookup"><span data-stu-id="05038-127">Type</span></span>|<span data-ttu-id="05038-128">説明</span><span class="sxs-lookup"><span data-stu-id="05038-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05038-129">id</span><span class="sxs-lookup"><span data-stu-id="05038-129">id</span></span>|<span data-ttu-id="05038-130">String</span><span class="sxs-lookup"><span data-stu-id="05038-130">String</span></span>|<span data-ttu-id="05038-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="05038-131">Name of the entity.</span></span> <span data-ttu-id="05038-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05038-133">lastModifiedDateTime</span></span>|<span data-ttu-id="05038-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05038-134">DateTimeOffset</span></span>|<span data-ttu-id="05038-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="05038-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="05038-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05038-137">createdDateTime</span></span>|<span data-ttu-id="05038-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05038-138">DateTimeOffset</span></span>|<span data-ttu-id="05038-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="05038-139">DateTime the object was created.</span></span> <span data-ttu-id="05038-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-141">description</span><span class="sxs-lookup"><span data-stu-id="05038-141">description</span></span>|<span data-ttu-id="05038-142">String</span><span class="sxs-lookup"><span data-stu-id="05038-142">String</span></span>|<span data-ttu-id="05038-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="05038-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05038-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-145">displayName</span><span class="sxs-lookup"><span data-stu-id="05038-145">displayName</span></span>|<span data-ttu-id="05038-146">String</span><span class="sxs-lookup"><span data-stu-id="05038-146">String</span></span>|<span data-ttu-id="05038-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="05038-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05038-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-149">version</span><span class="sxs-lookup"><span data-stu-id="05038-149">version</span></span>|<span data-ttu-id="05038-150">Int32</span><span class="sxs-lookup"><span data-stu-id="05038-150">Int32</span></span>|<span data-ttu-id="05038-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="05038-151">Version of the device configuration.</span></span> <span data-ttu-id="05038-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05038-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05038-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="05038-153">licenseType</span></span>|<span data-ttu-id="05038-154">String</span><span class="sxs-lookup"><span data-stu-id="05038-154">String</span></span>|<span data-ttu-id="05038-155">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="05038-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="05038-156">可能な値は、`productKey`、`licenseFile` です。</span><span class="sxs-lookup"><span data-stu-id="05038-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="05038-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="05038-157">targetEdition</span></span>|<span data-ttu-id="05038-158">String</span><span class="sxs-lookup"><span data-stu-id="05038-158">String</span></span>|<span data-ttu-id="05038-159">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="05038-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="05038-160">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN` です。</span><span class="sxs-lookup"><span data-stu-id="05038-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="05038-161">license</span><span class="sxs-lookup"><span data-stu-id="05038-161">License</span></span>|<span data-ttu-id="05038-162">String</span><span class="sxs-lookup"><span data-stu-id="05038-162">String</span></span>|<span data-ttu-id="05038-163">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="05038-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="05038-164">productKey</span><span class="sxs-lookup"><span data-stu-id="05038-164">productKey</span></span>|<span data-ttu-id="05038-165">String</span><span class="sxs-lookup"><span data-stu-id="05038-165">String</span></span>|<span data-ttu-id="05038-166">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="05038-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="05038-167">応答</span><span class="sxs-lookup"><span data-stu-id="05038-167">Response</span></span>
<span data-ttu-id="05038-168">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05038-168">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05038-169">例</span><span class="sxs-lookup"><span data-stu-id="05038-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="05038-170">要求</span><span class="sxs-lookup"><span data-stu-id="05038-170">Request</span></span>
<span data-ttu-id="05038-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05038-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
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

### <a name="response"></a><span data-ttu-id="05038-172">応答</span><span class="sxs-lookup"><span data-stu-id="05038-172">Response</span></span>
<span data-ttu-id="05038-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05038-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



