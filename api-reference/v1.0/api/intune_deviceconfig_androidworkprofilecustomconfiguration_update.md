# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="e6af9-101">AndroidWorkProfileCustomConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="e6af9-101">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="e6af9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6af9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6af9-103">[AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e6af9-103">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6af9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e6af9-104">Prerequisites</span></span>
<span data-ttu-id="e6af9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6af9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6af9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6af9-107">Permission type</span></span>|<span data-ttu-id="e6af9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6af9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6af9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6af9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e6af9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6af9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6af9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6af9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6af9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6af9-112">Not supported.</span></span>|
|<span data-ttu-id="e6af9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6af9-113">Application</span></span>|<span data-ttu-id="e6af9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6af9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6af9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6af9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e6af9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6af9-116">Request headers</span></span>
|<span data-ttu-id="e6af9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6af9-117">Header</span></span>|<span data-ttu-id="e6af9-118">値</span><span class="sxs-lookup"><span data-stu-id="e6af9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6af9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6af9-119">Authorization</span></span>|<span data-ttu-id="e6af9-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e6af9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6af9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e6af9-121">Accept</span></span>|<span data-ttu-id="e6af9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e6af9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6af9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6af9-123">Request body</span></span>
<span data-ttu-id="e6af9-124">要求の本文に[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6af9-124">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="e6af9-125">[AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e6af9-125">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="e6af9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6af9-126">Property</span></span>|<span data-ttu-id="e6af9-127">型</span><span class="sxs-lookup"><span data-stu-id="e6af9-127">Type</span></span>|<span data-ttu-id="e6af9-128">説明</span><span class="sxs-lookup"><span data-stu-id="e6af9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6af9-129">id</span><span class="sxs-lookup"><span data-stu-id="e6af9-129">id</span></span>|<span data-ttu-id="e6af9-130">String</span><span class="sxs-lookup"><span data-stu-id="e6af9-130">String</span></span>|<span data-ttu-id="e6af9-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e6af9-131">Key of the entity.</span></span> <span data-ttu-id="e6af9-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6af9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e6af9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6af9-134">DateTimeOffset</span></span>|<span data-ttu-id="e6af9-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e6af9-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e6af9-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6af9-137">createdDateTime</span></span>|<span data-ttu-id="e6af9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6af9-138">DateTimeOffset</span></span>|<span data-ttu-id="e6af9-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e6af9-139">DateTime the object was created.</span></span> <span data-ttu-id="e6af9-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-141">説明</span><span class="sxs-lookup"><span data-stu-id="e6af9-141">description</span></span>|<span data-ttu-id="e6af9-142">String</span><span class="sxs-lookup"><span data-stu-id="e6af9-142">String</span></span>|<span data-ttu-id="e6af9-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e6af9-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6af9-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e6af9-145">displayName</span></span>|<span data-ttu-id="e6af9-146">String</span><span class="sxs-lookup"><span data-stu-id="e6af9-146">String</span></span>|<span data-ttu-id="e6af9-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e6af9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6af9-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-149">version</span><span class="sxs-lookup"><span data-stu-id="e6af9-149">version</span></span>|<span data-ttu-id="e6af9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af9-150">Int32</span></span>|<span data-ttu-id="e6af9-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e6af9-151">Version of the device configuration.</span></span> <span data-ttu-id="e6af9-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e6af9-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6af9-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e6af9-153">omaSettings</span></span>|<span data-ttu-id="e6af9-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6af9-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="e6af9-155">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="e6af9-155">OMA settings.</span></span> <span data-ttu-id="e6af9-156">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e6af9-156">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e6af9-157">応答</span><span class="sxs-lookup"><span data-stu-id="e6af9-157">Response</span></span>
<span data-ttu-id="e6af9-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e6af9-158">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6af9-159">例</span><span class="sxs-lookup"><span data-stu-id="e6af9-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6af9-160">要求</span><span class="sxs-lookup"><span data-stu-id="e6af9-160">Request</span></span>
<span data-ttu-id="e6af9-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e6af9-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="e6af9-162">応答</span><span class="sxs-lookup"><span data-stu-id="e6af9-162">Response</span></span>
<span data-ttu-id="e6af9-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6af9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



