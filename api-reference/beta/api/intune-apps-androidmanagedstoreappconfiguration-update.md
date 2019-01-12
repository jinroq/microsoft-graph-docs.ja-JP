---
title: AndroidManagedStoreAppConfiguration を更新します。
description: AndroidManagedStoreAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d7cd4efcd6bd97488f49050eaf55d6bf408c2a3a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940681"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="0dd0d-103">AndroidManagedStoreAppConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="0dd0d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0dd0d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0dd0d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0dd0d-107">[AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0dd0d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0dd0d-108">Prerequisites</span></span>
<span data-ttu-id="0dd0d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dd0d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0dd0d-111">Permission type</span></span>|<span data-ttu-id="0dd0d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0dd0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dd0d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0dd0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dd0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dd0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0dd0d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0dd0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dd0d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-116">Not supported.</span></span>|
|<span data-ttu-id="0dd0d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0dd0d-117">Application</span></span>|<span data-ttu-id="0dd0d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dd0d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0dd0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0dd0d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dd0d-120">Request headers</span></span>
|<span data-ttu-id="0dd0d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dd0d-121">Header</span></span>|<span data-ttu-id="0dd0d-122">値</span><span class="sxs-lookup"><span data-stu-id="0dd0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dd0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dd0d-123">Authorization</span></span>|<span data-ttu-id="0dd0d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dd0d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0dd0d-125">Accept</span></span>|<span data-ttu-id="0dd0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dd0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dd0d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0dd0d-127">Request body</span></span>
<span data-ttu-id="0dd0d-128">要求の本文に[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="0dd0d-129">[AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="0dd0d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dd0d-130">Property</span></span>|<span data-ttu-id="0dd0d-131">型</span><span class="sxs-lookup"><span data-stu-id="0dd0d-131">Type</span></span>|<span data-ttu-id="0dd0d-132">説明</span><span class="sxs-lookup"><span data-stu-id="0dd0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd0d-133">ID</span><span class="sxs-lookup"><span data-stu-id="0dd0d-133">id</span></span>|<span data-ttu-id="0dd0d-134">String</span><span class="sxs-lookup"><span data-stu-id="0dd0d-134">String</span></span>|<span data-ttu-id="0dd0d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-135">Key of the entity.</span></span> <span data-ttu-id="0dd0d-136">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0dd0d-137">targetedMobileApps</span></span>|<span data-ttu-id="0dd0d-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0dd0d-138">String collection</span></span>|<span data-ttu-id="0dd0d-139">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-139">the associated app.</span></span> <span data-ttu-id="0dd0d-140">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0dd0d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0dd0d-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0dd0d-142">String collection</span></span>|<span data-ttu-id="0dd0d-143">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="0dd0d-144">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0dd0d-145">createdDateTime</span></span>|<span data-ttu-id="0dd0d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dd0d-146">DateTimeOffset</span></span>|<span data-ttu-id="0dd0d-147">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-147">DateTime the object was created.</span></span> <span data-ttu-id="0dd0d-148">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-149">説明</span><span class="sxs-lookup"><span data-stu-id="0dd0d-149">description</span></span>|<span data-ttu-id="0dd0d-150">String</span><span class="sxs-lookup"><span data-stu-id="0dd0d-150">String</span></span>|<span data-ttu-id="0dd0d-151">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0dd0d-152">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dd0d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0dd0d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dd0d-154">DateTimeOffset</span></span>|<span data-ttu-id="0dd0d-155">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-155">DateTime the object was last modified.</span></span> <span data-ttu-id="0dd0d-156">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-157">displayName</span><span class="sxs-lookup"><span data-stu-id="0dd0d-157">displayName</span></span>|<span data-ttu-id="0dd0d-158">String</span><span class="sxs-lookup"><span data-stu-id="0dd0d-158">String</span></span>|<span data-ttu-id="0dd0d-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0dd0d-160">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-161">version</span><span class="sxs-lookup"><span data-stu-id="0dd0d-161">version</span></span>|<span data-ttu-id="0dd0d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0dd0d-162">Int32</span></span>|<span data-ttu-id="0dd0d-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-163">Version of the device configuration.</span></span> <span data-ttu-id="0dd0d-164">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="0dd0d-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0dd0d-165">packageId</span><span class="sxs-lookup"><span data-stu-id="0dd0d-165">packageId</span></span>|<span data-ttu-id="0dd0d-166">String</span><span class="sxs-lookup"><span data-stu-id="0dd0d-166">String</span></span>|<span data-ttu-id="0dd0d-167">Android エンタープライズ アプリケーションの構成パッケージの id。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="0dd0d-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="0dd0d-168">payloadJson</span></span>|<span data-ttu-id="0dd0d-169">String</span><span class="sxs-lookup"><span data-stu-id="0dd0d-169">String</span></span>|<span data-ttu-id="0dd0d-170">Android エンタープライズ アプリケーション構成 JSON ペイロード。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="0dd0d-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="0dd0d-171">permissionActions</span></span>|<span data-ttu-id="0dd0d-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0dd0d-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="0dd0d-173">Android アプリケーションのアクセス許可とアクセス許可の対応するアクションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="0dd0d-174">応答</span><span class="sxs-lookup"><span data-stu-id="0dd0d-174">Response</span></span>
<span data-ttu-id="0dd0d-175">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-175">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dd0d-176">例</span><span class="sxs-lookup"><span data-stu-id="0dd0d-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="0dd0d-177">要求</span><span class="sxs-lookup"><span data-stu-id="0dd0d-177">Request</span></span>
<span data-ttu-id="0dd0d-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 549

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

### <a name="response"></a><span data-ttu-id="0dd0d-179">応答</span><span class="sxs-lookup"><span data-stu-id="0dd0d-179">Response</span></span>
<span data-ttu-id="0dd0d-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0dd0d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

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
  ]
}
```





