---
title: iosMobileAppConfiguration の更新
description: iosMobileAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: d70b528ca5524c1dfddbc84a21d1c60844f4b0a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360656"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="cb7de-103">iosMobileAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="cb7de-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="cb7de-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb7de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb7de-105">[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb7de-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb7de-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cb7de-106">Prerequisites</span></span>
<span data-ttu-id="cb7de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb7de-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb7de-109">Permission type</span></span>|<span data-ttu-id="cb7de-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb7de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb7de-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb7de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb7de-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb7de-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb7de-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb7de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb7de-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb7de-114">Not supported.</span></span>|
|<span data-ttu-id="cb7de-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb7de-115">Application</span></span>|<span data-ttu-id="cb7de-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb7de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb7de-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb7de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb7de-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb7de-118">Request headers</span></span>
|<span data-ttu-id="cb7de-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb7de-119">Header</span></span>|<span data-ttu-id="cb7de-120">値</span><span class="sxs-lookup"><span data-stu-id="cb7de-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb7de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb7de-121">Authorization</span></span>|<span data-ttu-id="cb7de-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cb7de-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb7de-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cb7de-123">Accept</span></span>|<span data-ttu-id="cb7de-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb7de-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb7de-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb7de-125">Request body</span></span>
<span data-ttu-id="cb7de-126">要求本文で、[iOSMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb7de-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="cb7de-127">次の表に、[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cb7de-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="cb7de-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb7de-128">Property</span></span>|<span data-ttu-id="cb7de-129">種類</span><span class="sxs-lookup"><span data-stu-id="cb7de-129">Type</span></span>|<span data-ttu-id="cb7de-130">説明</span><span class="sxs-lookup"><span data-stu-id="cb7de-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb7de-131">ID</span><span class="sxs-lookup"><span data-stu-id="cb7de-131">id</span></span>|<span data-ttu-id="cb7de-132">String</span><span class="sxs-lookup"><span data-stu-id="cb7de-132">String</span></span>|<span data-ttu-id="cb7de-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb7de-133">Key of the entity.</span></span> <span data-ttu-id="cb7de-134">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cb7de-135">targetedMobileApps</span></span>|<span data-ttu-id="cb7de-136">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cb7de-136">String collection</span></span>|<span data-ttu-id="cb7de-137">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="cb7de-137">the associated app.</span></span> <span data-ttu-id="cb7de-138">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb7de-139">createdDateTime</span></span>|<span data-ttu-id="cb7de-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb7de-140">DateTimeOffset</span></span>|<span data-ttu-id="cb7de-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb7de-141">DateTime the object was created.</span></span> <span data-ttu-id="cb7de-142">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-143">説明</span><span class="sxs-lookup"><span data-stu-id="cb7de-143">description</span></span>|<span data-ttu-id="cb7de-144">String</span><span class="sxs-lookup"><span data-stu-id="cb7de-144">String</span></span>|<span data-ttu-id="cb7de-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cb7de-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb7de-146">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb7de-147">lastModifiedDateTime</span></span>|<span data-ttu-id="cb7de-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb7de-148">DateTimeOffset</span></span>|<span data-ttu-id="cb7de-149">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb7de-149">DateTime the object was last modified.</span></span> <span data-ttu-id="cb7de-150">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-151">displayName</span><span class="sxs-lookup"><span data-stu-id="cb7de-151">displayName</span></span>|<span data-ttu-id="cb7de-152">String</span><span class="sxs-lookup"><span data-stu-id="cb7de-152">String</span></span>|<span data-ttu-id="cb7de-153">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cb7de-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb7de-154">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-155">version</span><span class="sxs-lookup"><span data-stu-id="cb7de-155">version</span></span>|<span data-ttu-id="cb7de-156">Int32</span><span class="sxs-lookup"><span data-stu-id="cb7de-156">Int32</span></span>|<span data-ttu-id="cb7de-157">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cb7de-157">Version of the device configuration.</span></span> <span data-ttu-id="cb7de-158">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="cb7de-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cb7de-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="cb7de-159">encodedSettingXml</span></span>|<span data-ttu-id="cb7de-160">Binary</span><span class="sxs-lookup"><span data-stu-id="cb7de-160">Binary</span></span>|<span data-ttu-id="cb7de-161">mdm アプリ 構成 Base 64 バイナリ。</span><span class="sxs-lookup"><span data-stu-id="cb7de-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="cb7de-162">settings</span><span class="sxs-lookup"><span data-stu-id="cb7de-162">settings</span></span>|<span data-ttu-id="cb7de-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb7de-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="cb7de-164">アプリの構成設定アイテム。</span><span class="sxs-lookup"><span data-stu-id="cb7de-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="cb7de-165">応答</span><span class="sxs-lookup"><span data-stu-id="cb7de-165">Response</span></span>
<span data-ttu-id="cb7de-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb7de-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb7de-167">例</span><span class="sxs-lookup"><span data-stu-id="cb7de-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb7de-168">要求</span><span class="sxs-lookup"><span data-stu-id="cb7de-168">Request</span></span>
<span data-ttu-id="cb7de-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb7de-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="cb7de-170">応答</span><span class="sxs-lookup"><span data-stu-id="cb7de-170">Response</span></span>
<span data-ttu-id="cb7de-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb7de-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



