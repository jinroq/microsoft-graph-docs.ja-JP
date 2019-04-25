---
title: iosMobileAppConfiguration の作成
description: 新しい iosMobileAppConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d5ada7a620a131e17a3403ad8c30b52ca4ab5c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577323"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="6e2d3-103">iosMobileAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="6e2d3-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="6e2d3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e2d3-105">新しい [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e2d3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6e2d3-106">Prerequisites</span></span>
<span data-ttu-id="6e2d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e2d3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e2d3-109">Permission type</span></span>|<span data-ttu-id="6e2d3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e2d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e2d3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e2d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e2d3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e2d3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6e2d3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e2d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e2d3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-114">Not supported.</span></span>|
|<span data-ttu-id="6e2d3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e2d3-115">Application</span></span>|<span data-ttu-id="6e2d3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e2d3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e2d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e2d3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e2d3-118">Request headers</span></span>
|<span data-ttu-id="6e2d3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e2d3-119">Header</span></span>|<span data-ttu-id="6e2d3-120">値</span><span class="sxs-lookup"><span data-stu-id="6e2d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e2d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e2d3-121">Authorization</span></span>|<span data-ttu-id="6e2d3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e2d3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6e2d3-123">Accept</span></span>|<span data-ttu-id="6e2d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e2d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e2d3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e2d3-125">Request body</span></span>
<span data-ttu-id="6e2d3-126">要求本文で、iOSMobileAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="6e2d3-127">次の表に、iosMobileAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="6e2d3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e2d3-128">Property</span></span>|<span data-ttu-id="6e2d3-129">型</span><span class="sxs-lookup"><span data-stu-id="6e2d3-129">Type</span></span>|<span data-ttu-id="6e2d3-130">説明</span><span class="sxs-lookup"><span data-stu-id="6e2d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e2d3-131">id</span><span class="sxs-lookup"><span data-stu-id="6e2d3-131">id</span></span>|<span data-ttu-id="6e2d3-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6e2d3-132">String</span></span>|<span data-ttu-id="6e2d3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-133">Key of the entity.</span></span> <span data-ttu-id="6e2d3-134">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6e2d3-135">targetedMobileApps</span></span>|<span data-ttu-id="6e2d3-136">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6e2d3-136">String collection</span></span>|<span data-ttu-id="6e2d3-137">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-137">the associated app.</span></span> <span data-ttu-id="6e2d3-138">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e2d3-139">createdDateTime</span></span>|<span data-ttu-id="6e2d3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e2d3-140">DateTimeOffset</span></span>|<span data-ttu-id="6e2d3-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-141">DateTime the object was created.</span></span> <span data-ttu-id="6e2d3-142">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-143">説明</span><span class="sxs-lookup"><span data-stu-id="6e2d3-143">description</span></span>|<span data-ttu-id="6e2d3-144">String</span><span class="sxs-lookup"><span data-stu-id="6e2d3-144">String</span></span>|<span data-ttu-id="6e2d3-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e2d3-146">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e2d3-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6e2d3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e2d3-148">DateTimeOffset</span></span>|<span data-ttu-id="6e2d3-149">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-149">DateTime the object was last modified.</span></span> <span data-ttu-id="6e2d3-150">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="6e2d3-151">displayName</span></span>|<span data-ttu-id="6e2d3-152">String</span><span class="sxs-lookup"><span data-stu-id="6e2d3-152">String</span></span>|<span data-ttu-id="6e2d3-153">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e2d3-154">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-155">version</span><span class="sxs-lookup"><span data-stu-id="6e2d3-155">version</span></span>|<span data-ttu-id="6e2d3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6e2d3-156">Int32</span></span>|<span data-ttu-id="6e2d3-157">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-157">Version of the device configuration.</span></span> <span data-ttu-id="6e2d3-158">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="6e2d3-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="6e2d3-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="6e2d3-159">encodedSettingXml</span></span>|<span data-ttu-id="6e2d3-160">Binary</span><span class="sxs-lookup"><span data-stu-id="6e2d3-160">Binary</span></span>|<span data-ttu-id="6e2d3-161">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="6e2d3-162">settings</span><span class="sxs-lookup"><span data-stu-id="6e2d3-162">settings</span></span>|<span data-ttu-id="6e2d3-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e2d3-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="6e2d3-164">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="6e2d3-165">応答</span><span class="sxs-lookup"><span data-stu-id="6e2d3-165">Response</span></span>
<span data-ttu-id="6e2d3-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e2d3-167">例</span><span class="sxs-lookup"><span data-stu-id="6e2d3-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e2d3-168">要求</span><span class="sxs-lookup"><span data-stu-id="6e2d3-168">Request</span></span>
<span data-ttu-id="6e2d3-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e2d3-170">応答</span><span class="sxs-lookup"><span data-stu-id="6e2d3-170">Response</span></span>
<span data-ttu-id="6e2d3-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e2d3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



