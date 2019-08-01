---
title: iosDeviceFeaturesConfiguration の作成
description: 新しい iosDeviceFeaturesConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba88edb991817dc1ef843ebdea544d41710030a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017330"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="1830c-103">iosDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="1830c-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="1830c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1830c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1830c-105">新しい [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1830c-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1830c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1830c-106">Prerequisites</span></span>
<span data-ttu-id="1830c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1830c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1830c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1830c-109">Permission type</span></span>|<span data-ttu-id="1830c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1830c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1830c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1830c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1830c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1830c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1830c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1830c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1830c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1830c-114">Not supported.</span></span>|
|<span data-ttu-id="1830c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1830c-115">Application</span></span>|<span data-ttu-id="1830c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1830c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1830c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1830c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1830c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1830c-118">Request headers</span></span>
|<span data-ttu-id="1830c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1830c-119">Header</span></span>|<span data-ttu-id="1830c-120">値</span><span class="sxs-lookup"><span data-stu-id="1830c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1830c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1830c-121">Authorization</span></span>|<span data-ttu-id="1830c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1830c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1830c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1830c-123">Accept</span></span>|<span data-ttu-id="1830c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1830c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1830c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1830c-125">Request body</span></span>
<span data-ttu-id="1830c-126">要求本文で、iosDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1830c-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="1830c-127">次の表に、iosDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1830c-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="1830c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1830c-128">Property</span></span>|<span data-ttu-id="1830c-129">型</span><span class="sxs-lookup"><span data-stu-id="1830c-129">Type</span></span>|<span data-ttu-id="1830c-130">説明</span><span class="sxs-lookup"><span data-stu-id="1830c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1830c-131">id</span><span class="sxs-lookup"><span data-stu-id="1830c-131">id</span></span>|<span data-ttu-id="1830c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1830c-132">String</span></span>|<span data-ttu-id="1830c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1830c-133">Key of the entity.</span></span> <span data-ttu-id="1830c-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1830c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1830c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1830c-136">DateTimeOffset</span></span>|<span data-ttu-id="1830c-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1830c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1830c-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1830c-139">createdDateTime</span></span>|<span data-ttu-id="1830c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1830c-140">DateTimeOffset</span></span>|<span data-ttu-id="1830c-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1830c-141">DateTime the object was created.</span></span> <span data-ttu-id="1830c-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-143">description</span><span class="sxs-lookup"><span data-stu-id="1830c-143">description</span></span>|<span data-ttu-id="1830c-144">String</span><span class="sxs-lookup"><span data-stu-id="1830c-144">String</span></span>|<span data-ttu-id="1830c-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1830c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1830c-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1830c-147">displayName</span></span>|<span data-ttu-id="1830c-148">String</span><span class="sxs-lookup"><span data-stu-id="1830c-148">String</span></span>|<span data-ttu-id="1830c-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1830c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1830c-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-151">version</span><span class="sxs-lookup"><span data-stu-id="1830c-151">version</span></span>|<span data-ttu-id="1830c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1830c-152">Int32</span></span>|<span data-ttu-id="1830c-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1830c-153">Version of the device configuration.</span></span> <span data-ttu-id="1830c-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1830c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1830c-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="1830c-155">assetTagTemplate</span></span>|<span data-ttu-id="1830c-156">String</span><span class="sxs-lookup"><span data-stu-id="1830c-156">String</span></span>|<span data-ttu-id="1830c-157">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="1830c-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="1830c-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="1830c-158">lockScreenFootnote</span></span>|<span data-ttu-id="1830c-159">String</span><span class="sxs-lookup"><span data-stu-id="1830c-159">String</span></span>|<span data-ttu-id="1830c-160">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="1830c-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="1830c-161">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="1830c-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="1830c-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="1830c-162">homeScreenDockIcons</span></span>|<span data-ttu-id="1830c-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1830c-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="1830c-164">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="1830c-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="1830c-165">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1830c-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1830c-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="1830c-166">homeScreenPages</span></span>|<span data-ttu-id="1830c-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1830c-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="1830c-168">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="1830c-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="1830c-169">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1830c-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1830c-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="1830c-170">notificationSettings</span></span>|<span data-ttu-id="1830c-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1830c-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="1830c-172">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="1830c-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="1830c-173">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1830c-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1830c-174">応答</span><span class="sxs-lookup"><span data-stu-id="1830c-174">Response</span></span>
<span data-ttu-id="1830c-175">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1830c-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1830c-176">例</span><span class="sxs-lookup"><span data-stu-id="1830c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="1830c-177">要求</span><span class="sxs-lookup"><span data-stu-id="1830c-177">Request</span></span>
<span data-ttu-id="1830c-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1830c-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1830c-179">応答</span><span class="sxs-lookup"><span data-stu-id="1830c-179">Response</span></span>
<span data-ttu-id="1830c-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1830c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



