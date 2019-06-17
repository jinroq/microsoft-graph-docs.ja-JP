---
title: AndroidForWorkMobileAppConfiguration を作成する
description: 新しい androidForWorkMobileAppConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5771a571ec53c8edaeb54e7b983f3be9bba3540
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966426"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="90fe5-103">AndroidForWorkMobileAppConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="90fe5-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="90fe5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90fe5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90fe5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90fe5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90fe5-106">新しい[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="90fe5-106">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90fe5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="90fe5-107">Prerequisites</span></span>
<span data-ttu-id="90fe5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90fe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90fe5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90fe5-110">Permission type</span></span>|<span data-ttu-id="90fe5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90fe5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90fe5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90fe5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90fe5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fe5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90fe5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90fe5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90fe5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90fe5-115">Not supported.</span></span>|
|<span data-ttu-id="90fe5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90fe5-116">Application</span></span>|<span data-ttu-id="90fe5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90fe5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90fe5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90fe5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90fe5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90fe5-119">Request headers</span></span>
|<span data-ttu-id="90fe5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90fe5-120">Header</span></span>|<span data-ttu-id="90fe5-121">値</span><span class="sxs-lookup"><span data-stu-id="90fe5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90fe5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90fe5-122">Authorization</span></span>|<span data-ttu-id="90fe5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="90fe5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90fe5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="90fe5-124">Accept</span></span>|<span data-ttu-id="90fe5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90fe5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90fe5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="90fe5-126">Request body</span></span>
<span data-ttu-id="90fe5-127">要求本文で、androidForWorkMobileAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="90fe5-127">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="90fe5-128">次の表に、androidForWorkMobileAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90fe5-128">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="90fe5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90fe5-129">Property</span></span>|<span data-ttu-id="90fe5-130">型</span><span class="sxs-lookup"><span data-stu-id="90fe5-130">Type</span></span>|<span data-ttu-id="90fe5-131">説明</span><span class="sxs-lookup"><span data-stu-id="90fe5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90fe5-132">id</span><span class="sxs-lookup"><span data-stu-id="90fe5-132">id</span></span>|<span data-ttu-id="90fe5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="90fe5-133">String</span></span>|<span data-ttu-id="90fe5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="90fe5-134">Key of the entity.</span></span> <span data-ttu-id="90fe5-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="90fe5-136">targetedMobileApps</span></span>|<span data-ttu-id="90fe5-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="90fe5-137">String collection</span></span>|<span data-ttu-id="90fe5-138">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="90fe5-138">the associated app.</span></span> <span data-ttu-id="90fe5-139">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90fe5-140">roleScopeTagIds</span></span>|<span data-ttu-id="90fe5-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="90fe5-141">String collection</span></span>|<span data-ttu-id="90fe5-142">このアプリ構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="90fe5-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="90fe5-143">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90fe5-144">createdDateTime</span></span>|<span data-ttu-id="90fe5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90fe5-145">DateTimeOffset</span></span>|<span data-ttu-id="90fe5-146">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90fe5-146">DateTime the object was created.</span></span> <span data-ttu-id="90fe5-147">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-148">description</span><span class="sxs-lookup"><span data-stu-id="90fe5-148">description</span></span>|<span data-ttu-id="90fe5-149">String</span><span class="sxs-lookup"><span data-stu-id="90fe5-149">String</span></span>|<span data-ttu-id="90fe5-150">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="90fe5-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90fe5-151">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90fe5-152">lastModifiedDateTime</span></span>|<span data-ttu-id="90fe5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90fe5-153">DateTimeOffset</span></span>|<span data-ttu-id="90fe5-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90fe5-154">DateTime the object was last modified.</span></span> <span data-ttu-id="90fe5-155">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-156">displayName</span><span class="sxs-lookup"><span data-stu-id="90fe5-156">displayName</span></span>|<span data-ttu-id="90fe5-157">String</span><span class="sxs-lookup"><span data-stu-id="90fe5-157">String</span></span>|<span data-ttu-id="90fe5-158">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="90fe5-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90fe5-159">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-160">version</span><span class="sxs-lookup"><span data-stu-id="90fe5-160">version</span></span>|<span data-ttu-id="90fe5-161">Int32</span><span class="sxs-lookup"><span data-stu-id="90fe5-161">Int32</span></span>|<span data-ttu-id="90fe5-162">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="90fe5-162">Version of the device configuration.</span></span> <span data-ttu-id="90fe5-163">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="90fe5-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="90fe5-164">packageId</span><span class="sxs-lookup"><span data-stu-id="90fe5-164">packageId</span></span>|<span data-ttu-id="90fe5-165">String</span><span class="sxs-lookup"><span data-stu-id="90fe5-165">String</span></span>|<span data-ttu-id="90fe5-166">Android For Work アプリの構成パッケージ id。</span><span class="sxs-lookup"><span data-stu-id="90fe5-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="90fe5-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="90fe5-167">payloadJson</span></span>|<span data-ttu-id="90fe5-168">String</span><span class="sxs-lookup"><span data-stu-id="90fe5-168">String</span></span>|<span data-ttu-id="90fe5-169">Android For Work アプリ構成 JSON ペイロード。</span><span class="sxs-lookup"><span data-stu-id="90fe5-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="90fe5-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="90fe5-170">permissionActions</span></span>|<span data-ttu-id="90fe5-171">[Androidpermissionaction](../resources/intune-apps-androidpermissionaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90fe5-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="90fe5-172">Android アプリのアクセス許可と、それに対応するアクセス許可アクションのリスト。</span><span class="sxs-lookup"><span data-stu-id="90fe5-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="90fe5-173">応答</span><span class="sxs-lookup"><span data-stu-id="90fe5-173">Response</span></span>
<span data-ttu-id="90fe5-174">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90fe5-174">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90fe5-175">例</span><span class="sxs-lookup"><span data-stu-id="90fe5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="90fe5-176">要求</span><span class="sxs-lookup"><span data-stu-id="90fe5-176">Request</span></span>
<span data-ttu-id="90fe5-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90fe5-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="90fe5-178">応答</span><span class="sxs-lookup"><span data-stu-id="90fe5-178">Response</span></span>
<span data-ttu-id="90fe5-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90fe5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 732

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
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
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ]
}
```





