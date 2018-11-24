# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="612cd-101">iosDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="612cd-101">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="612cd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="612cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="612cd-103">新しい [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="612cd-103">Create a new [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="612cd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="612cd-104">Prerequisites</span></span>
<span data-ttu-id="612cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="612cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="612cd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="612cd-107">Permission type</span></span>|<span data-ttu-id="612cd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="612cd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="612cd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="612cd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="612cd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612cd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="612cd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="612cd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="612cd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="612cd-112">Not supported.</span></span>|
|<span data-ttu-id="612cd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="612cd-113">Application</span></span>|<span data-ttu-id="612cd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="612cd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="612cd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="612cd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="612cd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="612cd-116">Request headers</span></span>
|<span data-ttu-id="612cd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="612cd-117">Header</span></span>|<span data-ttu-id="612cd-118">値</span><span class="sxs-lookup"><span data-stu-id="612cd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="612cd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="612cd-119">Authorization</span></span>|<span data-ttu-id="612cd-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="612cd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="612cd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="612cd-121">Accept</span></span>|<span data-ttu-id="612cd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="612cd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="612cd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="612cd-123">Request body</span></span>
<span data-ttu-id="612cd-124">要求本文で、iosDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="612cd-124">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="612cd-125">次の表に、iosDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="612cd-125">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="612cd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="612cd-126">Property</span></span>|<span data-ttu-id="612cd-127">型</span><span class="sxs-lookup"><span data-stu-id="612cd-127">Type</span></span>|<span data-ttu-id="612cd-128">説明</span><span class="sxs-lookup"><span data-stu-id="612cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="612cd-129">id</span><span class="sxs-lookup"><span data-stu-id="612cd-129">id</span></span>|<span data-ttu-id="612cd-130">String</span><span class="sxs-lookup"><span data-stu-id="612cd-130">String</span></span>|<span data-ttu-id="612cd-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="612cd-131">Key of the entity.</span></span> <span data-ttu-id="612cd-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="612cd-133">lastModifiedDateTime</span></span>|<span data-ttu-id="612cd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612cd-134">DateTimeOffset</span></span>|<span data-ttu-id="612cd-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="612cd-135">DateTime the object was last modified.</span></span> <span data-ttu-id="612cd-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="612cd-137">createdDateTime</span></span>|<span data-ttu-id="612cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612cd-138">DateTimeOffset</span></span>|<span data-ttu-id="612cd-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="612cd-139">DateTime the object was created.</span></span> <span data-ttu-id="612cd-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-141">description</span><span class="sxs-lookup"><span data-stu-id="612cd-141">description</span></span>|<span data-ttu-id="612cd-142">String</span><span class="sxs-lookup"><span data-stu-id="612cd-142">String</span></span>|<span data-ttu-id="612cd-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="612cd-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="612cd-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="612cd-145">displayName</span></span>|<span data-ttu-id="612cd-146">String</span><span class="sxs-lookup"><span data-stu-id="612cd-146">String</span></span>|<span data-ttu-id="612cd-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="612cd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="612cd-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-149">version</span><span class="sxs-lookup"><span data-stu-id="612cd-149">version</span></span>|<span data-ttu-id="612cd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="612cd-150">Int32</span></span>|<span data-ttu-id="612cd-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="612cd-151">Version of the device configuration.</span></span> <span data-ttu-id="612cd-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="612cd-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="612cd-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="612cd-153">assetTagTemplate</span></span>|<span data-ttu-id="612cd-154">String</span><span class="sxs-lookup"><span data-stu-id="612cd-154">String</span></span>|<span data-ttu-id="612cd-155">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報。</span><span class="sxs-lookup"><span data-stu-id="612cd-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="612cd-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="612cd-156">lockScreenFootnote</span></span>|<span data-ttu-id="612cd-157">String</span><span class="sxs-lookup"><span data-stu-id="612cd-157">String</span></span>|<span data-ttu-id="612cd-158">ログイン ウィンドウとロック画面に表示される脚注。</span><span class="sxs-lookup"><span data-stu-id="612cd-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="612cd-159">iOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="612cd-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="612cd-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="612cd-160">homeScreenDockIcons</span></span>|<span data-ttu-id="612cd-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="612cd-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="612cd-162">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="612cd-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="612cd-163">このコレクションには、最大 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="612cd-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="612cd-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="612cd-164">homeScreenPages</span></span>|<span data-ttu-id="612cd-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="612cd-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="612cd-166">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="612cd-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="612cd-167">このコレクションには、最大 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="612cd-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="612cd-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="612cd-168">notificationSettings</span></span>|<span data-ttu-id="612cd-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="612cd-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="612cd-170">各バンドル ID の通知設定。監視モードのデバイス (iOS 9.3 以降) にのみ適用します。</span><span class="sxs-lookup"><span data-stu-id="612cd-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="612cd-171">このコレクションには、最大 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="612cd-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="612cd-172">応答</span><span class="sxs-lookup"><span data-stu-id="612cd-172">Response</span></span>
<span data-ttu-id="612cd-173">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="612cd-173">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="612cd-174">例</span><span class="sxs-lookup"><span data-stu-id="612cd-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="612cd-175">要求</span><span class="sxs-lookup"><span data-stu-id="612cd-175">Request</span></span>
<span data-ttu-id="612cd-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="612cd-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="612cd-177">応答</span><span class="sxs-lookup"><span data-stu-id="612cd-177">Response</span></span>
<span data-ttu-id="612cd-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="612cd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```



