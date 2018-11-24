# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="48236-101">iosMobileAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="48236-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="48236-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="48236-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48236-103">新しい [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="48236-103">Create a new [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48236-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="48236-104">Prerequisites</span></span>
<span data-ttu-id="48236-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48236-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48236-107">Permission type</span></span>|<span data-ttu-id="48236-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="48236-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48236-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="48236-109">Delegated (work or school account)</span></span>|<span data-ttu-id="48236-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48236-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48236-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48236-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48236-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48236-112">Not supported.</span></span>|
|<span data-ttu-id="48236-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48236-113">Application</span></span>|<span data-ttu-id="48236-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48236-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48236-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48236-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48236-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48236-116">Request headers</span></span>
|<span data-ttu-id="48236-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48236-117">Header</span></span>|<span data-ttu-id="48236-118">値</span><span class="sxs-lookup"><span data-stu-id="48236-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48236-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="48236-119">Authorization</span></span>|<span data-ttu-id="48236-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="48236-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48236-121">Accept</span><span class="sxs-lookup"><span data-stu-id="48236-121">Accept</span></span>|<span data-ttu-id="48236-122">application/json</span><span class="sxs-lookup"><span data-stu-id="48236-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48236-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="48236-123">Request body</span></span>
<span data-ttu-id="48236-124">要求本文で、iOSMobileAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="48236-124">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="48236-125">次の表に、iosMobileAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="48236-125">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="48236-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48236-126">Property</span></span>|<span data-ttu-id="48236-127">型</span><span class="sxs-lookup"><span data-stu-id="48236-127">Type</span></span>|<span data-ttu-id="48236-128">説明</span><span class="sxs-lookup"><span data-stu-id="48236-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48236-129">id</span><span class="sxs-lookup"><span data-stu-id="48236-129">id</span></span>|<span data-ttu-id="48236-130">String</span><span class="sxs-lookup"><span data-stu-id="48236-130">String</span></span>|<span data-ttu-id="48236-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="48236-131">Key of the entity.</span></span> <span data-ttu-id="48236-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="48236-133">targetedMobileApps</span></span>|<span data-ttu-id="48236-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="48236-134">String collection</span></span>|<span data-ttu-id="48236-135">関連するアプリ。</span><span class="sxs-lookup"><span data-stu-id="48236-135">the associated app.</span></span> <span data-ttu-id="48236-136">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48236-137">createdDateTime</span></span>|<span data-ttu-id="48236-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48236-138">DateTimeOffset</span></span>|<span data-ttu-id="48236-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="48236-139">DateTime the object was created.</span></span> <span data-ttu-id="48236-140">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-141">description</span><span class="sxs-lookup"><span data-stu-id="48236-141">description</span></span>|<span data-ttu-id="48236-142">String</span><span class="sxs-lookup"><span data-stu-id="48236-142">String</span></span>|<span data-ttu-id="48236-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="48236-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48236-144">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48236-145">lastModifiedDateTime</span></span>|<span data-ttu-id="48236-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48236-146">DateTimeOffset</span></span>|<span data-ttu-id="48236-147">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="48236-147">DateTime the object was last modified.</span></span> <span data-ttu-id="48236-148">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-149">displayName</span><span class="sxs-lookup"><span data-stu-id="48236-149">displayName</span></span>|<span data-ttu-id="48236-150">String</span><span class="sxs-lookup"><span data-stu-id="48236-150">String</span></span>|<span data-ttu-id="48236-151">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="48236-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48236-152">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-153">version</span><span class="sxs-lookup"><span data-stu-id="48236-153">version</span></span>|<span data-ttu-id="48236-154">Int32</span><span class="sxs-lookup"><span data-stu-id="48236-154">Int32</span></span>|<span data-ttu-id="48236-155">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="48236-155">Version of the device configuration.</span></span> <span data-ttu-id="48236-156">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み</span><span class="sxs-lookup"><span data-stu-id="48236-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="48236-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="48236-157">encodedSettingXml</span></span>|<span data-ttu-id="48236-158">Binary</span><span class="sxs-lookup"><span data-stu-id="48236-158">Binary</span></span>|<span data-ttu-id="48236-159">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="48236-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="48236-160">settings</span><span class="sxs-lookup"><span data-stu-id="48236-160">settings</span></span>|<span data-ttu-id="48236-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="48236-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="48236-162">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="48236-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="48236-163">応答</span><span class="sxs-lookup"><span data-stu-id="48236-163">Response</span></span>
<span data-ttu-id="48236-164">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48236-164">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48236-165">例</span><span class="sxs-lookup"><span data-stu-id="48236-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="48236-166">要求</span><span class="sxs-lookup"><span data-stu-id="48236-166">Request</span></span>
<span data-ttu-id="48236-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48236-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="48236-168">応答</span><span class="sxs-lookup"><span data-stu-id="48236-168">Response</span></span>
<span data-ttu-id="48236-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48236-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```



