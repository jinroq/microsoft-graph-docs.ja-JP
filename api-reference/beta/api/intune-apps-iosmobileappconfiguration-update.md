---
title: iosMobileAppConfiguration の更新
description: iosMobileAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67aa52f71303914aaa7173f266e60ad29d9fa811
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979132"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="7b453-103">iosMobileAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="7b453-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="7b453-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b453-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b453-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b453-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b453-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b453-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b453-107">[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b453-107">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b453-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b453-108">Prerequisites</span></span>
<span data-ttu-id="7b453-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b453-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b453-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b453-111">Permission type</span></span>|<span data-ttu-id="7b453-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b453-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b453-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b453-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b453-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7b453-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b453-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b453-116">Not supported.</span></span>|
|<span data-ttu-id="7b453-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b453-117">Application</span></span>|<span data-ttu-id="7b453-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b453-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b453-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7b453-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b453-120">Request headers</span></span>
|<span data-ttu-id="7b453-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b453-121">Header</span></span>|<span data-ttu-id="7b453-122">値</span><span class="sxs-lookup"><span data-stu-id="7b453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b453-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b453-123">Authorization</span></span>|<span data-ttu-id="7b453-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7b453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b453-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b453-125">Accept</span></span>|<span data-ttu-id="7b453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b453-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b453-127">Request body</span></span>
<span data-ttu-id="7b453-128">要求本文で、[iOSMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b453-128">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="7b453-129">次の表に、[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7b453-129">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="7b453-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b453-130">Property</span></span>|<span data-ttu-id="7b453-131">型</span><span class="sxs-lookup"><span data-stu-id="7b453-131">Type</span></span>|<span data-ttu-id="7b453-132">説明</span><span class="sxs-lookup"><span data-stu-id="7b453-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b453-133">ID</span><span class="sxs-lookup"><span data-stu-id="7b453-133">id</span></span>|<span data-ttu-id="7b453-134">String</span><span class="sxs-lookup"><span data-stu-id="7b453-134">String</span></span>|<span data-ttu-id="7b453-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7b453-135">Key of the entity.</span></span> <span data-ttu-id="7b453-136">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7b453-137">targetedMobileApps</span></span>|<span data-ttu-id="7b453-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b453-138">String collection</span></span>|<span data-ttu-id="7b453-139">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="7b453-139">the associated app.</span></span> <span data-ttu-id="7b453-140">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b453-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b453-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b453-142">String collection</span></span>|<span data-ttu-id="7b453-143">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="7b453-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="7b453-144">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b453-145">createdDateTime</span></span>|<span data-ttu-id="7b453-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b453-146">DateTimeOffset</span></span>|<span data-ttu-id="7b453-147">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b453-147">DateTime the object was created.</span></span> <span data-ttu-id="7b453-148">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-149">説明</span><span class="sxs-lookup"><span data-stu-id="7b453-149">description</span></span>|<span data-ttu-id="7b453-150">String</span><span class="sxs-lookup"><span data-stu-id="7b453-150">String</span></span>|<span data-ttu-id="7b453-151">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7b453-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b453-152">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b453-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7b453-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b453-154">DateTimeOffset</span></span>|<span data-ttu-id="7b453-155">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b453-155">DateTime the object was last modified.</span></span> <span data-ttu-id="7b453-156">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-157">displayName</span><span class="sxs-lookup"><span data-stu-id="7b453-157">displayName</span></span>|<span data-ttu-id="7b453-158">String</span><span class="sxs-lookup"><span data-stu-id="7b453-158">String</span></span>|<span data-ttu-id="7b453-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7b453-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b453-160">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-161">version</span><span class="sxs-lookup"><span data-stu-id="7b453-161">version</span></span>|<span data-ttu-id="7b453-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7b453-162">Int32</span></span>|<span data-ttu-id="7b453-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7b453-163">Version of the device configuration.</span></span> <span data-ttu-id="7b453-164">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="7b453-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b453-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="7b453-165">encodedSettingXml</span></span>|<span data-ttu-id="7b453-166">Binary</span><span class="sxs-lookup"><span data-stu-id="7b453-166">Binary</span></span>|<span data-ttu-id="7b453-167">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="7b453-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="7b453-168">settings</span><span class="sxs-lookup"><span data-stu-id="7b453-168">settings</span></span>|<span data-ttu-id="7b453-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b453-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="7b453-170">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="7b453-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="7b453-171">応答</span><span class="sxs-lookup"><span data-stu-id="7b453-171">Response</span></span>
<span data-ttu-id="7b453-172">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b453-172">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b453-173">例</span><span class="sxs-lookup"><span data-stu-id="7b453-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b453-174">要求</span><span class="sxs-lookup"><span data-stu-id="7b453-174">Request</span></span>
<span data-ttu-id="7b453-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b453-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 596

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="7b453-176">応答</span><span class="sxs-lookup"><span data-stu-id="7b453-176">Response</span></span>
<span data-ttu-id="7b453-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b453-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





