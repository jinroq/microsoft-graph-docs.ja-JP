# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="74a36-101">windows10EnterpriseModernAppManagementConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="74a36-101">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="74a36-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74a36-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74a36-103">新しい [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="74a36-103">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74a36-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="74a36-104">Prerequisites</span></span>
<span data-ttu-id="74a36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74a36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74a36-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74a36-107">Permission type</span></span>|<span data-ttu-id="74a36-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74a36-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74a36-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74a36-109">Delegated (work or school account)</span></span>|<span data-ttu-id="74a36-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a36-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74a36-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74a36-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74a36-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74a36-112">Not supported.</span></span>|
|<span data-ttu-id="74a36-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74a36-113">Application</span></span>|<span data-ttu-id="74a36-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74a36-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74a36-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74a36-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74a36-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74a36-116">Request headers</span></span>
|<span data-ttu-id="74a36-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74a36-117">Header</span></span>|<span data-ttu-id="74a36-118">値</span><span class="sxs-lookup"><span data-stu-id="74a36-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74a36-119">承認</span><span class="sxs-lookup"><span data-stu-id="74a36-119">Authorization</span></span>|<span data-ttu-id="74a36-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74a36-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74a36-121">承諾</span><span class="sxs-lookup"><span data-stu-id="74a36-121">Accept</span></span>|<span data-ttu-id="74a36-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="74a36-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74a36-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="74a36-123">Request body</span></span>
<span data-ttu-id="74a36-124">要求本文で、windows10EnterpriseModernAppManagementConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74a36-124">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="74a36-125">次の表に、windows10EnterpriseModernAppManagementConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="74a36-125">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="74a36-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74a36-126">Property</span></span>|<span data-ttu-id="74a36-127">型</span><span class="sxs-lookup"><span data-stu-id="74a36-127">Type</span></span>|<span data-ttu-id="74a36-128">説明</span><span class="sxs-lookup"><span data-stu-id="74a36-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74a36-129">ID</span><span class="sxs-lookup"><span data-stu-id="74a36-129">id</span></span>|<span data-ttu-id="74a36-130">文字列</span><span class="sxs-lookup"><span data-stu-id="74a36-130">String</span></span>|<span data-ttu-id="74a36-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="74a36-131">Key of the entity.</span></span> <span data-ttu-id="74a36-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74a36-133">lastModifiedDateTime</span></span>|<span data-ttu-id="74a36-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74a36-134">DateTimeOffset</span></span>|<span data-ttu-id="74a36-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="74a36-135">DateTime the object was last modified.</span></span> <span data-ttu-id="74a36-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74a36-137">createdDateTime</span></span>|<span data-ttu-id="74a36-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74a36-138">DateTimeOffset</span></span>|<span data-ttu-id="74a36-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="74a36-139">DateTime the object was created.</span></span> <span data-ttu-id="74a36-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-141">説明</span><span class="sxs-lookup"><span data-stu-id="74a36-141">description</span></span>|<span data-ttu-id="74a36-142">文字列</span><span class="sxs-lookup"><span data-stu-id="74a36-142">String</span></span>|<span data-ttu-id="74a36-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="74a36-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74a36-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-145">displayName</span><span class="sxs-lookup"><span data-stu-id="74a36-145">displayName</span></span>|<span data-ttu-id="74a36-146">文字列</span><span class="sxs-lookup"><span data-stu-id="74a36-146">String</span></span>|<span data-ttu-id="74a36-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="74a36-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74a36-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="74a36-149">version</span></span>|<span data-ttu-id="74a36-150">Int32</span><span class="sxs-lookup"><span data-stu-id="74a36-150">Int32</span></span>|<span data-ttu-id="74a36-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="74a36-151">Version of the device configuration.</span></span> <span data-ttu-id="74a36-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="74a36-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74a36-153">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="74a36-153">uninstallBuiltInApps</span></span>|<span data-ttu-id="74a36-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="74a36-154">Boolean</span></span>|<span data-ttu-id="74a36-155">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="74a36-155">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="74a36-156">応答</span><span class="sxs-lookup"><span data-stu-id="74a36-156">Response</span></span>
<span data-ttu-id="74a36-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74a36-157">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a36-158">例</span><span class="sxs-lookup"><span data-stu-id="74a36-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="74a36-159">要求</span><span class="sxs-lookup"><span data-stu-id="74a36-159">Request</span></span>
<span data-ttu-id="74a36-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74a36-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 286

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="74a36-161">応答</span><span class="sxs-lookup"><span data-stu-id="74a36-161">Response</span></span>
<span data-ttu-id="74a36-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74a36-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```








