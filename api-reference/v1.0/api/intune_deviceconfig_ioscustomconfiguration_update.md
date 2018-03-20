# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="a64c7-101">iosCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a64c7-101">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="a64c7-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a64c7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a64c7-103">[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a64c7-103">Update the properties of a [calendar](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a64c7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a64c7-104">Prerequisites</span></span>
<span data-ttu-id="a64c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a64c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a64c7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a64c7-107">Permission type</span></span>|<span data-ttu-id="a64c7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a64c7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a64c7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a64c7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a64c7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a64c7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a64c7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a64c7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a64c7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a64c7-112">Not supported.</span></span>|
|<span data-ttu-id="a64c7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a64c7-113">Application</span></span>|<span data-ttu-id="a64c7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a64c7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a64c7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a64c7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a64c7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a64c7-116">Request headers</span></span>
|<span data-ttu-id="a64c7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a64c7-117">Header</span></span>|<span data-ttu-id="a64c7-118">値</span><span class="sxs-lookup"><span data-stu-id="a64c7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a64c7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a64c7-119">Authorization</span></span>|<span data-ttu-id="a64c7-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a64c7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a64c7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a64c7-121">Accept</span></span>|<span data-ttu-id="a64c7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a64c7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a64c7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a64c7-123">Request body</span></span>
<span data-ttu-id="a64c7-124">要求本文で、[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a64c7-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="a64c7-125">次の表に、[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a64c7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a64c7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a64c7-126">Property</span></span>|<span data-ttu-id="a64c7-127">型</span><span class="sxs-lookup"><span data-stu-id="a64c7-127">Type</span></span>|<span data-ttu-id="a64c7-128">説明</span><span class="sxs-lookup"><span data-stu-id="a64c7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a64c7-129">id</span><span class="sxs-lookup"><span data-stu-id="a64c7-129">id</span></span>|<span data-ttu-id="a64c7-130">String</span><span class="sxs-lookup"><span data-stu-id="a64c7-130">String</span></span>|<span data-ttu-id="a64c7-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a64c7-131">Name of the entity.</span></span> <span data-ttu-id="a64c7-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a64c7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a64c7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a64c7-134">DateTimeOffset</span></span>|<span data-ttu-id="a64c7-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a64c7-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="a64c7-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a64c7-137">createdDateTime</span></span>|<span data-ttu-id="a64c7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a64c7-138">DateTimeOffset</span></span>|<span data-ttu-id="a64c7-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a64c7-139">DateTime the object was created.</span></span> <span data-ttu-id="a64c7-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-141">description</span><span class="sxs-lookup"><span data-stu-id="a64c7-141">description</span></span>|<span data-ttu-id="a64c7-142">String</span><span class="sxs-lookup"><span data-stu-id="a64c7-142">String</span></span>|<span data-ttu-id="a64c7-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a64c7-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a64c7-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a64c7-145">displayName</span></span>|<span data-ttu-id="a64c7-146">String</span><span class="sxs-lookup"><span data-stu-id="a64c7-146">String</span></span>|<span data-ttu-id="a64c7-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a64c7-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a64c7-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-149">version</span><span class="sxs-lookup"><span data-stu-id="a64c7-149">version</span></span>|<span data-ttu-id="a64c7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a64c7-150">Int32</span></span>|<span data-ttu-id="a64c7-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a64c7-151">Version of the device configuration.</span></span> <span data-ttu-id="a64c7-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a64c7-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a64c7-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="a64c7-153">payloadName</span></span>|<span data-ttu-id="a64c7-154">String</span><span class="sxs-lookup"><span data-stu-id="a64c7-154">String</span></span>|<span data-ttu-id="a64c7-155">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="a64c7-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a64c7-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a64c7-156">payloadFileName</span></span>|<span data-ttu-id="a64c7-157">String</span><span class="sxs-lookup"><span data-stu-id="a64c7-157">String</span></span>|<span data-ttu-id="a64c7-158">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a64c7-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a64c7-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="a64c7-159">\*.xml</span></span>|
|<span data-ttu-id="a64c7-160">payload</span><span class="sxs-lookup"><span data-stu-id="a64c7-160">Notification payload</span></span>|<span data-ttu-id="a64c7-161">Binary</span><span class="sxs-lookup"><span data-stu-id="a64c7-161">Binary</span></span>|<span data-ttu-id="a64c7-162">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="a64c7-162">Payload messages</span></span> <span data-ttu-id="a64c7-163">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="a64c7-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a64c7-164">応答</span><span class="sxs-lookup"><span data-stu-id="a64c7-164">Response</span></span>
<span data-ttu-id="a64c7-165">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a64c7-165">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64c7-166">例</span><span class="sxs-lookup"><span data-stu-id="a64c7-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="a64c7-167">要求</span><span class="sxs-lookup"><span data-stu-id="a64c7-167">Request</span></span>
<span data-ttu-id="a64c7-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a64c7-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 282

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="a64c7-169">応答</span><span class="sxs-lookup"><span data-stu-id="a64c7-169">Response</span></span>
<span data-ttu-id="a64c7-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a64c7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



