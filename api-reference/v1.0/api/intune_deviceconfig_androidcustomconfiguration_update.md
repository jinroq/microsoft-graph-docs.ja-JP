# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="e7e58-101">androidCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e7e58-101">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="e7e58-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7e58-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7e58-103">[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7e58-103">Update the properties of a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7e58-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7e58-104">Prerequisites</span></span>
<span data-ttu-id="e7e58-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7e58-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7e58-107">Permission type</span></span>|<span data-ttu-id="e7e58-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7e58-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7e58-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7e58-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7e58-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7e58-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7e58-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7e58-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7e58-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7e58-112">Not supported.</span></span>|
|<span data-ttu-id="e7e58-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7e58-113">Application</span></span>|<span data-ttu-id="e7e58-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7e58-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7e58-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7e58-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7e58-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7e58-116">Request headers</span></span>
|<span data-ttu-id="e7e58-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7e58-117">Header</span></span>|<span data-ttu-id="e7e58-118">値</span><span class="sxs-lookup"><span data-stu-id="e7e58-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7e58-119">承認</span><span class="sxs-lookup"><span data-stu-id="e7e58-119">Authorization</span></span>|<span data-ttu-id="e7e58-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e7e58-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7e58-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="e7e58-121">Accept</span></span>|<span data-ttu-id="e7e58-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="e7e58-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7e58-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7e58-123">Request body</span></span>
<span data-ttu-id="e7e58-124">要求本文で、[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7e58-124">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="e7e58-125">次の表に、[androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e7e58-125">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="e7e58-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7e58-126">Property</span></span>|<span data-ttu-id="e7e58-127">型</span><span class="sxs-lookup"><span data-stu-id="e7e58-127">Type</span></span>|<span data-ttu-id="e7e58-128">説明</span><span class="sxs-lookup"><span data-stu-id="e7e58-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7e58-129">ID</span><span class="sxs-lookup"><span data-stu-id="e7e58-129">id</span></span>|<span data-ttu-id="e7e58-130">文字列</span><span class="sxs-lookup"><span data-stu-id="e7e58-130">String</span></span>|<span data-ttu-id="e7e58-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7e58-131">Key of the entity.</span></span> <span data-ttu-id="e7e58-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7e58-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e7e58-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7e58-134">DateTimeOffset</span></span>|<span data-ttu-id="e7e58-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7e58-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e7e58-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7e58-137">createdDateTime</span></span>|<span data-ttu-id="e7e58-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7e58-138">DateTimeOffset</span></span>|<span data-ttu-id="e7e58-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7e58-139">DateTime the object was created.</span></span> <span data-ttu-id="e7e58-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-141">説明</span><span class="sxs-lookup"><span data-stu-id="e7e58-141">description</span></span>|<span data-ttu-id="e7e58-142">文字列</span><span class="sxs-lookup"><span data-stu-id="e7e58-142">String</span></span>|<span data-ttu-id="e7e58-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e7e58-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7e58-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e7e58-145">displayName</span></span>|<span data-ttu-id="e7e58-146">文字列</span><span class="sxs-lookup"><span data-stu-id="e7e58-146">String</span></span>|<span data-ttu-id="e7e58-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e7e58-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7e58-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="e7e58-149">version</span></span>|<span data-ttu-id="e7e58-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e7e58-150">Int32</span></span>|<span data-ttu-id="e7e58-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e7e58-151">Version of the device configuration.</span></span> <span data-ttu-id="e7e58-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7e58-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7e58-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e7e58-153">omaSettings</span></span>|<span data-ttu-id="e7e58-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7e58-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="e7e58-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="e7e58-155">OMA settings.</span></span> <span data-ttu-id="e7e58-156">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e7e58-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e7e58-157">応答</span><span class="sxs-lookup"><span data-stu-id="e7e58-157">Response</span></span>
<span data-ttu-id="e7e58-158">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e7e58-158">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7e58-159">例</span><span class="sxs-lookup"><span data-stu-id="e7e58-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7e58-160">要求</span><span class="sxs-lookup"><span data-stu-id="e7e58-160">Request</span></span>
<span data-ttu-id="e7e58-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7e58-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 401

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e7e58-162">応答</span><span class="sxs-lookup"><span data-stu-id="e7e58-162">Response</span></span>
<span data-ttu-id="e7e58-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7e58-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








