# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="43cfa-101">iosCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="43cfa-101">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="43cfa-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="43cfa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43cfa-103">新しい [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43cfa-103">Create a new [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43cfa-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="43cfa-104">Prerequisites</span></span>
<span data-ttu-id="43cfa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43cfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43cfa-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43cfa-107">Permission type</span></span>|<span data-ttu-id="43cfa-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43cfa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43cfa-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43cfa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43cfa-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43cfa-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43cfa-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43cfa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43cfa-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43cfa-112">Not supported.</span></span>|
|<span data-ttu-id="43cfa-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43cfa-113">Application</span></span>|<span data-ttu-id="43cfa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43cfa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43cfa-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43cfa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43cfa-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43cfa-116">Request headers</span></span>
|<span data-ttu-id="43cfa-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43cfa-117">Header</span></span>|<span data-ttu-id="43cfa-118">値</span><span class="sxs-lookup"><span data-stu-id="43cfa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43cfa-119">承認</span><span class="sxs-lookup"><span data-stu-id="43cfa-119">Authorization</span></span>|<span data-ttu-id="43cfa-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="43cfa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43cfa-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="43cfa-121">Accept</span></span>|<span data-ttu-id="43cfa-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="43cfa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43cfa-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="43cfa-123">Request body</span></span>
<span data-ttu-id="43cfa-124">要求本文で、iosCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43cfa-124">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="43cfa-125">次の表に、iosCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="43cfa-125">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="43cfa-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43cfa-126">Property</span></span>|<span data-ttu-id="43cfa-127">型</span><span class="sxs-lookup"><span data-stu-id="43cfa-127">Type</span></span>|<span data-ttu-id="43cfa-128">説明</span><span class="sxs-lookup"><span data-stu-id="43cfa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cfa-129">ID</span><span class="sxs-lookup"><span data-stu-id="43cfa-129">id</span></span>|<span data-ttu-id="43cfa-130">文字列</span><span class="sxs-lookup"><span data-stu-id="43cfa-130">String</span></span>|<span data-ttu-id="43cfa-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="43cfa-131">Key of the entity.</span></span> <span data-ttu-id="43cfa-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43cfa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="43cfa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cfa-134">DateTimeOffset</span></span>|<span data-ttu-id="43cfa-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43cfa-135">DateTime the object was last modified.</span></span> <span data-ttu-id="43cfa-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43cfa-137">createdDateTime</span></span>|<span data-ttu-id="43cfa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cfa-138">DateTimeOffset</span></span>|<span data-ttu-id="43cfa-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43cfa-139">DateTime the object was created.</span></span> <span data-ttu-id="43cfa-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-141">説明</span><span class="sxs-lookup"><span data-stu-id="43cfa-141">description</span></span>|<span data-ttu-id="43cfa-142">文字列</span><span class="sxs-lookup"><span data-stu-id="43cfa-142">String</span></span>|<span data-ttu-id="43cfa-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="43cfa-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43cfa-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-145">displayName</span><span class="sxs-lookup"><span data-stu-id="43cfa-145">displayName</span></span>|<span data-ttu-id="43cfa-146">文字列</span><span class="sxs-lookup"><span data-stu-id="43cfa-146">String</span></span>|<span data-ttu-id="43cfa-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="43cfa-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43cfa-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="43cfa-149">version</span></span>|<span data-ttu-id="43cfa-150">Int32</span><span class="sxs-lookup"><span data-stu-id="43cfa-150">Int32</span></span>|<span data-ttu-id="43cfa-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="43cfa-151">Version of the device configuration.</span></span> <span data-ttu-id="43cfa-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43cfa-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43cfa-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="43cfa-153">payloadName</span></span>|<span data-ttu-id="43cfa-154">文字列</span><span class="sxs-lookup"><span data-stu-id="43cfa-154">String</span></span>|<span data-ttu-id="43cfa-155">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="43cfa-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="43cfa-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="43cfa-156">payloadFileName</span></span>|<span data-ttu-id="43cfa-157">文字列</span><span class="sxs-lookup"><span data-stu-id="43cfa-157">String</span></span>|<span data-ttu-id="43cfa-158">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="43cfa-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="43cfa-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="43cfa-159">\*.xml).</span></span>|
|<span data-ttu-id="43cfa-160">ペイロード</span><span class="sxs-lookup"><span data-stu-id="43cfa-160">payload</span></span>|<span data-ttu-id="43cfa-161">バイナリ</span><span class="sxs-lookup"><span data-stu-id="43cfa-161">Binary</span></span>|<span data-ttu-id="43cfa-162">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="43cfa-162">Payload.</span></span> <span data-ttu-id="43cfa-163">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="43cfa-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="43cfa-164">応答</span><span class="sxs-lookup"><span data-stu-id="43cfa-164">Response</span></span>
<span data-ttu-id="43cfa-165">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43cfa-165">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43cfa-166">例</span><span class="sxs-lookup"><span data-stu-id="43cfa-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="43cfa-167">要求</span><span class="sxs-lookup"><span data-stu-id="43cfa-167">Request</span></span>
<span data-ttu-id="43cfa-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43cfa-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="43cfa-169">応答</span><span class="sxs-lookup"><span data-stu-id="43cfa-169">Response</span></span>
<span data-ttu-id="43cfa-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43cfa-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








