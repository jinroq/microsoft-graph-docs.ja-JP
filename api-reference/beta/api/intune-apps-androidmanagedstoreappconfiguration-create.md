---
title: AndroidManagedStoreAppConfiguration の作成
description: 新しい androidManagedStoreAppConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec843c7a16707cd33ebf698c9f32c9ee986cc2f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331890"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="27387-103">AndroidManagedStoreAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="27387-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="27387-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27387-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27387-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27387-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27387-106">新しい[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27387-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27387-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27387-107">Prerequisites</span></span>
<span data-ttu-id="27387-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27387-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27387-110">Permission type</span></span>|<span data-ttu-id="27387-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27387-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27387-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27387-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27387-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27387-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27387-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27387-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27387-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27387-115">Not supported.</span></span>|
|<span data-ttu-id="27387-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27387-116">Application</span></span>|<span data-ttu-id="27387-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27387-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27387-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27387-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="27387-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27387-119">Request headers</span></span>
|<span data-ttu-id="27387-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27387-120">Header</span></span>|<span data-ttu-id="27387-121">値</span><span class="sxs-lookup"><span data-stu-id="27387-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27387-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27387-122">Authorization</span></span>|<span data-ttu-id="27387-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27387-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27387-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27387-124">Accept</span></span>|<span data-ttu-id="27387-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27387-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27387-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27387-126">Request body</span></span>
<span data-ttu-id="27387-127">要求本文で、androidManagedStoreAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27387-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="27387-128">次の表に、androidManagedStoreAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27387-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="27387-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27387-129">Property</span></span>|<span data-ttu-id="27387-130">型</span><span class="sxs-lookup"><span data-stu-id="27387-130">Type</span></span>|<span data-ttu-id="27387-131">説明</span><span class="sxs-lookup"><span data-stu-id="27387-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27387-132">id</span><span class="sxs-lookup"><span data-stu-id="27387-132">id</span></span>|<span data-ttu-id="27387-133">文字列</span><span class="sxs-lookup"><span data-stu-id="27387-133">String</span></span>|<span data-ttu-id="27387-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="27387-134">Key of the entity.</span></span> <span data-ttu-id="27387-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="27387-136">targetedMobileApps</span></span>|<span data-ttu-id="27387-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="27387-137">String collection</span></span>|<span data-ttu-id="27387-138">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="27387-138">the associated app.</span></span> <span data-ttu-id="27387-139">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27387-140">roleScopeTagIds</span></span>|<span data-ttu-id="27387-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="27387-141">String collection</span></span>|<span data-ttu-id="27387-142">このアプリ構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="27387-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="27387-143">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27387-144">createdDateTime</span></span>|<span data-ttu-id="27387-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27387-145">DateTimeOffset</span></span>|<span data-ttu-id="27387-146">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="27387-146">DateTime the object was created.</span></span> <span data-ttu-id="27387-147">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-148">description</span><span class="sxs-lookup"><span data-stu-id="27387-148">description</span></span>|<span data-ttu-id="27387-149">String</span><span class="sxs-lookup"><span data-stu-id="27387-149">String</span></span>|<span data-ttu-id="27387-150">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="27387-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27387-151">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27387-152">lastModifiedDateTime</span></span>|<span data-ttu-id="27387-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27387-153">DateTimeOffset</span></span>|<span data-ttu-id="27387-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="27387-154">DateTime the object was last modified.</span></span> <span data-ttu-id="27387-155">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-156">displayName</span><span class="sxs-lookup"><span data-stu-id="27387-156">displayName</span></span>|<span data-ttu-id="27387-157">String</span><span class="sxs-lookup"><span data-stu-id="27387-157">String</span></span>|<span data-ttu-id="27387-158">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="27387-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27387-159">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-160">version</span><span class="sxs-lookup"><span data-stu-id="27387-160">version</span></span>|<span data-ttu-id="27387-161">Int32</span><span class="sxs-lookup"><span data-stu-id="27387-161">Int32</span></span>|<span data-ttu-id="27387-162">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="27387-162">Version of the device configuration.</span></span> <span data-ttu-id="27387-163">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="27387-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="27387-164">packageId</span><span class="sxs-lookup"><span data-stu-id="27387-164">packageId</span></span>|<span data-ttu-id="27387-165">String</span><span class="sxs-lookup"><span data-stu-id="27387-165">String</span></span>|<span data-ttu-id="27387-166">Android エンタープライズアプリ構成パッケージ id。</span><span class="sxs-lookup"><span data-stu-id="27387-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="27387-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="27387-167">payloadJson</span></span>|<span data-ttu-id="27387-168">String</span><span class="sxs-lookup"><span data-stu-id="27387-168">String</span></span>|<span data-ttu-id="27387-169">Android エンタープライズアプリ構成 JSON ペイロード。</span><span class="sxs-lookup"><span data-stu-id="27387-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="27387-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="27387-170">permissionActions</span></span>|<span data-ttu-id="27387-171">[Androidpermissionaction](../resources/intune-apps-androidpermissionaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="27387-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="27387-172">Android アプリのアクセス許可と、それに対応するアクセス許可アクションのリスト。</span><span class="sxs-lookup"><span data-stu-id="27387-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="27387-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="27387-173">appSupportsOemConfig</span></span>|<span data-ttu-id="27387-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="27387-174">Boolean</span></span>|<span data-ttu-id="27387-175">この AppConfig が OEMConfig ポリシーであるかどうか。</span><span class="sxs-lookup"><span data-stu-id="27387-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="27387-176">応答</span><span class="sxs-lookup"><span data-stu-id="27387-176">Response</span></span>
<span data-ttu-id="27387-177">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27387-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27387-178">例</span><span class="sxs-lookup"><span data-stu-id="27387-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="27387-179">要求</span><span class="sxs-lookup"><span data-stu-id="27387-179">Request</span></span>
<span data-ttu-id="27387-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27387-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27387-181">応答</span><span class="sxs-lookup"><span data-stu-id="27387-181">Response</span></span>
<span data-ttu-id="27387-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27387-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






