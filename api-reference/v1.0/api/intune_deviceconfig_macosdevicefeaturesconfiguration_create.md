# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="7aad3-101">macOSDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="7aad3-101">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="7aad3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7aad3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7aad3-103">新しい [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7aad3-103">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7aad3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7aad3-104">Prerequisites</span></span>
<span data-ttu-id="7aad3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aad3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7aad3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7aad3-107">Permission type</span></span>|<span data-ttu-id="7aad3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7aad3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aad3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7aad3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7aad3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aad3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7aad3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7aad3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aad3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aad3-112">Not supported.</span></span>|
|<span data-ttu-id="7aad3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7aad3-113">Application</span></span>|<span data-ttu-id="7aad3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aad3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aad3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7aad3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7aad3-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aad3-116">Request headers</span></span>
|<span data-ttu-id="7aad3-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aad3-117">Header</span></span>|<span data-ttu-id="7aad3-118">値</span><span class="sxs-lookup"><span data-stu-id="7aad3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aad3-119">承認</span><span class="sxs-lookup"><span data-stu-id="7aad3-119">Authorization</span></span>|<span data-ttu-id="7aad3-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7aad3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aad3-121">承諾</span><span class="sxs-lookup"><span data-stu-id="7aad3-121">Accept</span></span>|<span data-ttu-id="7aad3-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="7aad3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aad3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7aad3-123">Request body</span></span>
<span data-ttu-id="7aad3-124">要求本文で、macOSDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7aad3-124">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="7aad3-125">次の表に、macOSDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7aad3-125">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="7aad3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7aad3-126">Property</span></span>|<span data-ttu-id="7aad3-127">型</span><span class="sxs-lookup"><span data-stu-id="7aad3-127">Type</span></span>|<span data-ttu-id="7aad3-128">説明</span><span class="sxs-lookup"><span data-stu-id="7aad3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aad3-129">id</span><span class="sxs-lookup"><span data-stu-id="7aad3-129">id</span></span>|<span data-ttu-id="7aad3-130">文字列</span><span class="sxs-lookup"><span data-stu-id="7aad3-130">String</span></span>|<span data-ttu-id="7aad3-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7aad3-131">Key of the entity.</span></span> <span data-ttu-id="7aad3-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7aad3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7aad3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7aad3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aad3-134">DateTimeOffset</span></span>|<span data-ttu-id="7aad3-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7aad3-135">DateTime the object was last modified.</span></span> <span data-ttu-id="7aad3-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7aad3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7aad3-137">createdDateTime</span></span>|<span data-ttu-id="7aad3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aad3-138">DateTimeOffset</span></span>|<span data-ttu-id="7aad3-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7aad3-139">DateTime the object was created.</span></span> <span data-ttu-id="7aad3-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7aad3-141">説明</span><span class="sxs-lookup"><span data-stu-id="7aad3-141">description</span></span>|<span data-ttu-id="7aad3-142">文字列</span><span class="sxs-lookup"><span data-stu-id="7aad3-142">String</span></span>|<span data-ttu-id="7aad3-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7aad3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7aad3-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7aad3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7aad3-145">displayName</span></span>|<span data-ttu-id="7aad3-146">文字列</span><span class="sxs-lookup"><span data-stu-id="7aad3-146">String</span></span>|<span data-ttu-id="7aad3-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7aad3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7aad3-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7aad3-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="7aad3-149">version</span></span>|<span data-ttu-id="7aad3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7aad3-150">Int32</span></span>|<span data-ttu-id="7aad3-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7aad3-151">Version of the device configuration.</span></span> <span data-ttu-id="7aad3-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7aad3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7aad3-153">応答</span><span class="sxs-lookup"><span data-stu-id="7aad3-153">Response</span></span>
<span data-ttu-id="7aad3-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7aad3-154">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aad3-155">例</span><span class="sxs-lookup"><span data-stu-id="7aad3-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="7aad3-156">要求</span><span class="sxs-lookup"><span data-stu-id="7aad3-156">Request</span></span>
<span data-ttu-id="7aad3-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7aad3-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="7aad3-158">応答</span><span class="sxs-lookup"><span data-stu-id="7aad3-158">Response</span></span>
<span data-ttu-id="7aad3-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7aad3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```








