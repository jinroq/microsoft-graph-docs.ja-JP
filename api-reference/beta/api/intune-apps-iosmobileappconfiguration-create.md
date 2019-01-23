---
title: iosMobileAppConfiguration の作成
description: 新しい iosMobileAppConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fd3b9b94d94f78db0db69d5b6e69d269ba0e7bcc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418940"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="3fbd9-103">iosMobileAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="3fbd9-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3fbd9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fbd9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fbd9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fbd9-107">新しい [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fbd9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fbd9-108">Prerequisites</span></span>
<span data-ttu-id="3fbd9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fbd9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fbd9-111">Permission type</span></span>|<span data-ttu-id="3fbd9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fbd9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fbd9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fbd9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fbd9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fbd9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3fbd9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fbd9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fbd9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-116">Not supported.</span></span>|
|<span data-ttu-id="3fbd9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fbd9-117">Application</span></span>|<span data-ttu-id="3fbd9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fbd9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fbd9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3fbd9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fbd9-120">Request headers</span></span>
|<span data-ttu-id="3fbd9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fbd9-121">Header</span></span>|<span data-ttu-id="3fbd9-122">値</span><span class="sxs-lookup"><span data-stu-id="3fbd9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fbd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fbd9-123">Authorization</span></span>|<span data-ttu-id="3fbd9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fbd9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fbd9-125">Accept</span></span>|<span data-ttu-id="3fbd9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fbd9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fbd9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fbd9-127">Request body</span></span>
<span data-ttu-id="3fbd9-128">要求本文で、iOSMobileAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="3fbd9-129">次の表に、iosMobileAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="3fbd9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fbd9-130">Property</span></span>|<span data-ttu-id="3fbd9-131">型</span><span class="sxs-lookup"><span data-stu-id="3fbd9-131">Type</span></span>|<span data-ttu-id="3fbd9-132">説明</span><span class="sxs-lookup"><span data-stu-id="3fbd9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fbd9-133">id</span><span class="sxs-lookup"><span data-stu-id="3fbd9-133">id</span></span>|<span data-ttu-id="3fbd9-134">String</span><span class="sxs-lookup"><span data-stu-id="3fbd9-134">String</span></span>|<span data-ttu-id="3fbd9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-135">Key of the entity.</span></span> <span data-ttu-id="3fbd9-136">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3fbd9-137">targetedMobileApps</span></span>|<span data-ttu-id="3fbd9-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3fbd9-138">String collection</span></span>|<span data-ttu-id="3fbd9-139">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-139">the associated app.</span></span> <span data-ttu-id="3fbd9-140">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fbd9-141">roleScopeTagIds</span></span>|<span data-ttu-id="3fbd9-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3fbd9-142">String collection</span></span>|<span data-ttu-id="3fbd9-143">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="3fbd9-144">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fbd9-145">createdDateTime</span></span>|<span data-ttu-id="3fbd9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fbd9-146">DateTimeOffset</span></span>|<span data-ttu-id="3fbd9-147">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-147">DateTime the object was created.</span></span> <span data-ttu-id="3fbd9-148">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-149">説明</span><span class="sxs-lookup"><span data-stu-id="3fbd9-149">description</span></span>|<span data-ttu-id="3fbd9-150">String</span><span class="sxs-lookup"><span data-stu-id="3fbd9-150">String</span></span>|<span data-ttu-id="3fbd9-151">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3fbd9-152">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fbd9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3fbd9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fbd9-154">DateTimeOffset</span></span>|<span data-ttu-id="3fbd9-155">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-155">DateTime the object was last modified.</span></span> <span data-ttu-id="3fbd9-156">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-157">displayName</span><span class="sxs-lookup"><span data-stu-id="3fbd9-157">displayName</span></span>|<span data-ttu-id="3fbd9-158">String</span><span class="sxs-lookup"><span data-stu-id="3fbd9-158">String</span></span>|<span data-ttu-id="3fbd9-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3fbd9-160">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-161">version</span><span class="sxs-lookup"><span data-stu-id="3fbd9-161">version</span></span>|<span data-ttu-id="3fbd9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbd9-162">Int32</span></span>|<span data-ttu-id="3fbd9-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-163">Version of the device configuration.</span></span> <span data-ttu-id="3fbd9-164">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="3fbd9-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3fbd9-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="3fbd9-165">encodedSettingXml</span></span>|<span data-ttu-id="3fbd9-166">Binary</span><span class="sxs-lookup"><span data-stu-id="3fbd9-166">Binary</span></span>|<span data-ttu-id="3fbd9-167">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="3fbd9-168">設定</span><span class="sxs-lookup"><span data-stu-id="3fbd9-168">settings</span></span>|<span data-ttu-id="3fbd9-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3fbd9-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="3fbd9-170">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="3fbd9-171">応答</span><span class="sxs-lookup"><span data-stu-id="3fbd9-171">Response</span></span>
<span data-ttu-id="3fbd9-172">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fbd9-173">例</span><span class="sxs-lookup"><span data-stu-id="3fbd9-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fbd9-174">要求</span><span class="sxs-lookup"><span data-stu-id="3fbd9-174">Request</span></span>
<span data-ttu-id="3fbd9-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
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

### <a name="response"></a><span data-ttu-id="3fbd9-176">応答</span><span class="sxs-lookup"><span data-stu-id="3fbd9-176">Response</span></span>
<span data-ttu-id="3fbd9-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fbd9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
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




