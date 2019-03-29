---
title: iosMobileAppConfiguration の更新
description: iosMobileAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 129c859c78957b345d2c25f320b932e3e24464b3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981679"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="1ebe3-103">iosMobileAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1ebe3-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="1ebe3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ebe3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ebe3-106">[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ebe3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1ebe3-107">Prerequisites</span></span>
<span data-ttu-id="1ebe3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ebe3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ebe3-110">Permission type</span></span>|<span data-ttu-id="1ebe3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ebe3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ebe3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ebe3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ebe3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ebe3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ebe3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ebe3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ebe3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-115">Not supported.</span></span>|
|<span data-ttu-id="1ebe3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ebe3-116">Application</span></span>|<span data-ttu-id="1ebe3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ebe3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ebe3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1ebe3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ebe3-119">Request headers</span></span>
|<span data-ttu-id="1ebe3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ebe3-120">Header</span></span>|<span data-ttu-id="1ebe3-121">値</span><span class="sxs-lookup"><span data-stu-id="1ebe3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ebe3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ebe3-122">Authorization</span></span>|<span data-ttu-id="1ebe3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ebe3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1ebe3-124">Accept</span></span>|<span data-ttu-id="1ebe3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ebe3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ebe3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ebe3-126">Request body</span></span>
<span data-ttu-id="1ebe3-127">要求本文で、[iOSMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="1ebe3-128">次の表に、[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="1ebe3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ebe3-129">Property</span></span>|<span data-ttu-id="1ebe3-130">型</span><span class="sxs-lookup"><span data-stu-id="1ebe3-130">Type</span></span>|<span data-ttu-id="1ebe3-131">説明</span><span class="sxs-lookup"><span data-stu-id="1ebe3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ebe3-132">id</span><span class="sxs-lookup"><span data-stu-id="1ebe3-132">id</span></span>|<span data-ttu-id="1ebe3-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1ebe3-133">String</span></span>|<span data-ttu-id="1ebe3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-134">Key of the entity.</span></span> <span data-ttu-id="1ebe3-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1ebe3-136">targetedMobileApps</span></span>|<span data-ttu-id="1ebe3-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1ebe3-137">String collection</span></span>|<span data-ttu-id="1ebe3-138">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-138">the associated app.</span></span> <span data-ttu-id="1ebe3-139">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ebe3-140">roleScopeTagIds</span></span>|<span data-ttu-id="1ebe3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1ebe3-141">String collection</span></span>|<span data-ttu-id="1ebe3-142">このアプリ構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="1ebe3-143">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ebe3-144">createdDateTime</span></span>|<span data-ttu-id="1ebe3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ebe3-145">DateTimeOffset</span></span>|<span data-ttu-id="1ebe3-146">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-146">DateTime the object was created.</span></span> <span data-ttu-id="1ebe3-147">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-148">description</span><span class="sxs-lookup"><span data-stu-id="1ebe3-148">description</span></span>|<span data-ttu-id="1ebe3-149">String</span><span class="sxs-lookup"><span data-stu-id="1ebe3-149">String</span></span>|<span data-ttu-id="1ebe3-150">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ebe3-151">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ebe3-152">lastModifiedDateTime</span></span>|<span data-ttu-id="1ebe3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ebe3-153">DateTimeOffset</span></span>|<span data-ttu-id="1ebe3-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-154">DateTime the object was last modified.</span></span> <span data-ttu-id="1ebe3-155">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-156">displayName</span><span class="sxs-lookup"><span data-stu-id="1ebe3-156">displayName</span></span>|<span data-ttu-id="1ebe3-157">String</span><span class="sxs-lookup"><span data-stu-id="1ebe3-157">String</span></span>|<span data-ttu-id="1ebe3-158">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ebe3-159">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-160">version</span><span class="sxs-lookup"><span data-stu-id="1ebe3-160">version</span></span>|<span data-ttu-id="1ebe3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1ebe3-161">Int32</span></span>|<span data-ttu-id="1ebe3-162">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-162">Version of the device configuration.</span></span> <span data-ttu-id="1ebe3-163">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="1ebe3-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ebe3-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="1ebe3-164">encodedSettingXml</span></span>|<span data-ttu-id="1ebe3-165">Binary</span><span class="sxs-lookup"><span data-stu-id="1ebe3-165">Binary</span></span>|<span data-ttu-id="1ebe3-166">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="1ebe3-167">settings</span><span class="sxs-lookup"><span data-stu-id="1ebe3-167">settings</span></span>|<span data-ttu-id="1ebe3-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1ebe3-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="1ebe3-169">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="1ebe3-170">応答</span><span class="sxs-lookup"><span data-stu-id="1ebe3-170">Response</span></span>
<span data-ttu-id="1ebe3-171">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-171">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ebe3-172">例</span><span class="sxs-lookup"><span data-stu-id="1ebe3-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ebe3-173">要求</span><span class="sxs-lookup"><span data-stu-id="1ebe3-173">Request</span></span>
<span data-ttu-id="1ebe3-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="1ebe3-175">応答</span><span class="sxs-lookup"><span data-stu-id="1ebe3-175">Response</span></span>
<span data-ttu-id="1ebe3-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ebe3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




