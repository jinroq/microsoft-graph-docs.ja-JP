# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="79bca-101">androidCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="79bca-101">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="79bca-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79bca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79bca-103">新しい [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="79bca-103">Create a new [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79bca-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="79bca-104">Prerequisites</span></span>
<span data-ttu-id="79bca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79bca-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79bca-107">Permission type</span></span>|<span data-ttu-id="79bca-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79bca-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79bca-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79bca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79bca-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79bca-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79bca-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79bca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79bca-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79bca-112">Not supported.</span></span>|
|<span data-ttu-id="79bca-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79bca-113">Application</span></span>|<span data-ttu-id="79bca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79bca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79bca-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79bca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79bca-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79bca-116">Request headers</span></span>
|<span data-ttu-id="79bca-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79bca-117">Header</span></span>|<span data-ttu-id="79bca-118">値</span><span class="sxs-lookup"><span data-stu-id="79bca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79bca-119">承認</span><span class="sxs-lookup"><span data-stu-id="79bca-119">Authorization</span></span>|<span data-ttu-id="79bca-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79bca-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79bca-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="79bca-121">Accept</span></span>|<span data-ttu-id="79bca-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="79bca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79bca-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="79bca-123">Request body</span></span>
<span data-ttu-id="79bca-124">要求本文で、androidCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79bca-124">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="79bca-125">次の表に、androidCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79bca-125">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="79bca-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79bca-126">Property</span></span>|<span data-ttu-id="79bca-127">型</span><span class="sxs-lookup"><span data-stu-id="79bca-127">Type</span></span>|<span data-ttu-id="79bca-128">説明</span><span class="sxs-lookup"><span data-stu-id="79bca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79bca-129">ID</span><span class="sxs-lookup"><span data-stu-id="79bca-129">id</span></span>|<span data-ttu-id="79bca-130">文字列</span><span class="sxs-lookup"><span data-stu-id="79bca-130">String</span></span>|<span data-ttu-id="79bca-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="79bca-131">Key of the entity.</span></span> <span data-ttu-id="79bca-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79bca-133">lastModifiedDateTime</span></span>|<span data-ttu-id="79bca-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79bca-134">DateTimeOffset</span></span>|<span data-ttu-id="79bca-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="79bca-135">DateTime the object was last modified.</span></span> <span data-ttu-id="79bca-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79bca-137">createdDateTime</span></span>|<span data-ttu-id="79bca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79bca-138">DateTimeOffset</span></span>|<span data-ttu-id="79bca-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="79bca-139">DateTime the object was created.</span></span> <span data-ttu-id="79bca-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-141">説明</span><span class="sxs-lookup"><span data-stu-id="79bca-141">description</span></span>|<span data-ttu-id="79bca-142">文字列</span><span class="sxs-lookup"><span data-stu-id="79bca-142">String</span></span>|<span data-ttu-id="79bca-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="79bca-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79bca-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-145">displayName</span><span class="sxs-lookup"><span data-stu-id="79bca-145">displayName</span></span>|<span data-ttu-id="79bca-146">文字列</span><span class="sxs-lookup"><span data-stu-id="79bca-146">String</span></span>|<span data-ttu-id="79bca-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="79bca-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79bca-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="79bca-149">version</span></span>|<span data-ttu-id="79bca-150">Int32</span><span class="sxs-lookup"><span data-stu-id="79bca-150">Int32</span></span>|<span data-ttu-id="79bca-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="79bca-151">Version of the device configuration.</span></span> <span data-ttu-id="79bca-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79bca-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79bca-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="79bca-153">omaSettings</span></span>|<span data-ttu-id="79bca-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79bca-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="79bca-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="79bca-155">OMA settings.</span></span> <span data-ttu-id="79bca-156">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="79bca-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="79bca-157">応答</span><span class="sxs-lookup"><span data-stu-id="79bca-157">Response</span></span>
<span data-ttu-id="79bca-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79bca-158">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79bca-159">例</span><span class="sxs-lookup"><span data-stu-id="79bca-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="79bca-160">要求</span><span class="sxs-lookup"><span data-stu-id="79bca-160">Request</span></span>
<span data-ttu-id="79bca-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79bca-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="79bca-162">応答</span><span class="sxs-lookup"><span data-stu-id="79bca-162">Response</span></span>
<span data-ttu-id="79bca-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79bca-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








