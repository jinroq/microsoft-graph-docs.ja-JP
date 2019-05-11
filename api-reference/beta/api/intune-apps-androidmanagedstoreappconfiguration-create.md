---
title: AndroidManagedStoreAppConfiguration の作成
description: 新しい androidManagedStoreAppConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3100ce3046522e55ff65fb20d7ac48448089bd6d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937240"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="0bc9b-103">AndroidManagedStoreAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="0bc9b-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="0bc9b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bc9b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bc9b-106">新しい[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bc9b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0bc9b-107">Prerequisites</span></span>
<span data-ttu-id="0bc9b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bc9b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bc9b-110">Permission type</span></span>|<span data-ttu-id="0bc9b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bc9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bc9b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bc9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bc9b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bc9b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0bc9b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bc9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bc9b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-115">Not supported.</span></span>|
|<span data-ttu-id="0bc9b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bc9b-116">Application</span></span>|<span data-ttu-id="0bc9b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bc9b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bc9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0bc9b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bc9b-119">Request headers</span></span>
|<span data-ttu-id="0bc9b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bc9b-120">Header</span></span>|<span data-ttu-id="0bc9b-121">値</span><span class="sxs-lookup"><span data-stu-id="0bc9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bc9b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bc9b-122">Authorization</span></span>|<span data-ttu-id="0bc9b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bc9b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0bc9b-124">Accept</span></span>|<span data-ttu-id="0bc9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bc9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc9b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bc9b-126">Request body</span></span>
<span data-ttu-id="0bc9b-127">要求本文で、androidManagedStoreAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="0bc9b-128">次の表に、androidManagedStoreAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="0bc9b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bc9b-129">Property</span></span>|<span data-ttu-id="0bc9b-130">型</span><span class="sxs-lookup"><span data-stu-id="0bc9b-130">Type</span></span>|<span data-ttu-id="0bc9b-131">説明</span><span class="sxs-lookup"><span data-stu-id="0bc9b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc9b-132">id</span><span class="sxs-lookup"><span data-stu-id="0bc9b-132">id</span></span>|<span data-ttu-id="0bc9b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0bc9b-133">String</span></span>|<span data-ttu-id="0bc9b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-134">Key of the entity.</span></span> <span data-ttu-id="0bc9b-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0bc9b-136">targetedMobileApps</span></span>|<span data-ttu-id="0bc9b-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0bc9b-137">String collection</span></span>|<span data-ttu-id="0bc9b-138">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-138">the associated app.</span></span> <span data-ttu-id="0bc9b-139">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0bc9b-140">roleScopeTagIds</span></span>|<span data-ttu-id="0bc9b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0bc9b-141">String collection</span></span>|<span data-ttu-id="0bc9b-142">このアプリ構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="0bc9b-143">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bc9b-144">createdDateTime</span></span>|<span data-ttu-id="0bc9b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc9b-145">DateTimeOffset</span></span>|<span data-ttu-id="0bc9b-146">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-146">DateTime the object was created.</span></span> <span data-ttu-id="0bc9b-147">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-148">description</span><span class="sxs-lookup"><span data-stu-id="0bc9b-148">description</span></span>|<span data-ttu-id="0bc9b-149">String</span><span class="sxs-lookup"><span data-stu-id="0bc9b-149">String</span></span>|<span data-ttu-id="0bc9b-150">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bc9b-151">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bc9b-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0bc9b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc9b-153">DateTimeOffset</span></span>|<span data-ttu-id="0bc9b-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-154">DateTime the object was last modified.</span></span> <span data-ttu-id="0bc9b-155">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-156">displayName</span><span class="sxs-lookup"><span data-stu-id="0bc9b-156">displayName</span></span>|<span data-ttu-id="0bc9b-157">String</span><span class="sxs-lookup"><span data-stu-id="0bc9b-157">String</span></span>|<span data-ttu-id="0bc9b-158">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bc9b-159">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-160">version</span><span class="sxs-lookup"><span data-stu-id="0bc9b-160">version</span></span>|<span data-ttu-id="0bc9b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc9b-161">Int32</span></span>|<span data-ttu-id="0bc9b-162">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-162">Version of the device configuration.</span></span> <span data-ttu-id="0bc9b-163">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0bc9b-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0bc9b-164">packageId</span><span class="sxs-lookup"><span data-stu-id="0bc9b-164">packageId</span></span>|<span data-ttu-id="0bc9b-165">String</span><span class="sxs-lookup"><span data-stu-id="0bc9b-165">String</span></span>|<span data-ttu-id="0bc9b-166">Android エンタープライズアプリ構成パッケージ id。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="0bc9b-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="0bc9b-167">payloadJson</span></span>|<span data-ttu-id="0bc9b-168">String</span><span class="sxs-lookup"><span data-stu-id="0bc9b-168">String</span></span>|<span data-ttu-id="0bc9b-169">Android エンタープライズアプリ構成 JSON ペイロード。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="0bc9b-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="0bc9b-170">permissionActions</span></span>|<span data-ttu-id="0bc9b-171">[Androidpermissionaction](../resources/intune-apps-androidpermissionaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0bc9b-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="0bc9b-172">Android アプリのアクセス許可と、それに対応するアクセス許可アクションのリスト。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="0bc9b-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="0bc9b-173">appSupportsOemConfig</span></span>|<span data-ttu-id="0bc9b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bc9b-174">Boolean</span></span>|<span data-ttu-id="0bc9b-175">この AppConfig が OEMConfig ポリシーであるかどうか。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0bc9b-176">応答</span><span class="sxs-lookup"><span data-stu-id="0bc9b-176">Response</span></span>
<span data-ttu-id="0bc9b-177">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bc9b-178">例</span><span class="sxs-lookup"><span data-stu-id="0bc9b-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bc9b-179">要求</span><span class="sxs-lookup"><span data-stu-id="0bc9b-179">Request</span></span>
<span data-ttu-id="0bc9b-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 592

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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
  ],
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="0bc9b-181">応答</span><span class="sxs-lookup"><span data-stu-id="0bc9b-181">Response</span></span>
<span data-ttu-id="0bc9b-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0bc9b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 764

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
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
  ],
  "appSupportsOemConfig": true
}
```




