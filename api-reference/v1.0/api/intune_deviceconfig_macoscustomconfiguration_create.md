# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="d81c2-101">macOSCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="d81c2-101">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="d81c2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d81c2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d81c2-103">新しい [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d81c2-103">Create a new [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d81c2-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d81c2-104">Prerequisites</span></span>
<span data-ttu-id="d81c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d81c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d81c2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d81c2-107">Permission type</span></span>|<span data-ttu-id="d81c2-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d81c2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81c2-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d81c2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d81c2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81c2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d81c2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d81c2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81c2-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d81c2-112">Not supported.</span></span>|
|<span data-ttu-id="d81c2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d81c2-113">Application</span></span>|<span data-ttu-id="d81c2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d81c2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81c2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d81c2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d81c2-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d81c2-116">Request headers</span></span>
|<span data-ttu-id="d81c2-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d81c2-117">Header</span></span>|<span data-ttu-id="d81c2-118">値</span><span class="sxs-lookup"><span data-stu-id="d81c2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d81c2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d81c2-119">Authorization</span></span>|<span data-ttu-id="d81c2-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d81c2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d81c2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d81c2-121">Accept</span></span>|<span data-ttu-id="d81c2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d81c2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81c2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d81c2-123">Request body</span></span>
<span data-ttu-id="d81c2-124">要求本文で、macOSCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d81c2-124">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="d81c2-125">次の表に、macOSCustomConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d81c2-125">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="d81c2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d81c2-126">Property</span></span>|<span data-ttu-id="d81c2-127">型</span><span class="sxs-lookup"><span data-stu-id="d81c2-127">Type</span></span>|<span data-ttu-id="d81c2-128">説明</span><span class="sxs-lookup"><span data-stu-id="d81c2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81c2-129">id</span><span class="sxs-lookup"><span data-stu-id="d81c2-129">id</span></span>|<span data-ttu-id="d81c2-130">String</span><span class="sxs-lookup"><span data-stu-id="d81c2-130">String</span></span>|<span data-ttu-id="d81c2-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d81c2-131">Key of the entity.</span></span> <span data-ttu-id="d81c2-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d81c2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d81c2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81c2-134">DateTimeOffset</span></span>|<span data-ttu-id="d81c2-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d81c2-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d81c2-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d81c2-137">createdDateTime</span></span>|<span data-ttu-id="d81c2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81c2-138">DateTimeOffset</span></span>|<span data-ttu-id="d81c2-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d81c2-139">DateTime the object was created.</span></span> <span data-ttu-id="d81c2-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-141">description</span><span class="sxs-lookup"><span data-stu-id="d81c2-141">description</span></span>|<span data-ttu-id="d81c2-142">String</span><span class="sxs-lookup"><span data-stu-id="d81c2-142">String</span></span>|<span data-ttu-id="d81c2-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d81c2-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d81c2-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d81c2-145">displayName</span></span>|<span data-ttu-id="d81c2-146">String</span><span class="sxs-lookup"><span data-stu-id="d81c2-146">String</span></span>|<span data-ttu-id="d81c2-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d81c2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d81c2-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-149">version</span><span class="sxs-lookup"><span data-stu-id="d81c2-149">version</span></span>|<span data-ttu-id="d81c2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d81c2-150">Int32</span></span>|<span data-ttu-id="d81c2-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d81c2-151">Version of the device configuration.</span></span> <span data-ttu-id="d81c2-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d81c2-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d81c2-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="d81c2-153">payloadName</span></span>|<span data-ttu-id="d81c2-154">String</span><span class="sxs-lookup"><span data-stu-id="d81c2-154">String</span></span>|<span data-ttu-id="d81c2-155">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="d81c2-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="d81c2-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d81c2-156">payloadFileName</span></span>|<span data-ttu-id="d81c2-157">String</span><span class="sxs-lookup"><span data-stu-id="d81c2-157">String</span></span>|<span data-ttu-id="d81c2-158">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="d81c2-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="d81c2-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="d81c2-159">\*.xml).</span></span>|
|<span data-ttu-id="d81c2-160">payload</span><span class="sxs-lookup"><span data-stu-id="d81c2-160">payload</span></span>|<span data-ttu-id="d81c2-161">Binary</span><span class="sxs-lookup"><span data-stu-id="d81c2-161">Binary</span></span>|<span data-ttu-id="d81c2-162">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="d81c2-162">Payload.</span></span> <span data-ttu-id="d81c2-163">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="d81c2-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="d81c2-164">応答</span><span class="sxs-lookup"><span data-stu-id="d81c2-164">Response</span></span>
<span data-ttu-id="d81c2-165">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d81c2-165">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d81c2-166">例</span><span class="sxs-lookup"><span data-stu-id="d81c2-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="d81c2-167">要求</span><span class="sxs-lookup"><span data-stu-id="d81c2-167">Request</span></span>
<span data-ttu-id="d81c2-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d81c2-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="d81c2-169">応答</span><span class="sxs-lookup"><span data-stu-id="d81c2-169">Response</span></span>
<span data-ttu-id="d81c2-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d81c2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



