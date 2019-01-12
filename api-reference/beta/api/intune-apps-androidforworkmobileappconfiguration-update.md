---
title: AndroidForWorkMobileAppConfiguration を更新します。
description: AndroidForWorkMobileAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20f28ee3268e8e05563d1ed67d3dbe30e82cb801
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964894"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="9ce5c-103">AndroidForWorkMobileAppConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="9ce5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ce5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ce5c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ce5c-107">[AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ce5c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ce5c-108">Prerequisites</span></span>
<span data-ttu-id="9ce5c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce5c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ce5c-111">Permission type</span></span>|<span data-ttu-id="9ce5c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ce5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ce5c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ce5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ce5c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce5c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ce5c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ce5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce5c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-116">Not supported.</span></span>|
|<span data-ttu-id="9ce5c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ce5c-117">Application</span></span>|<span data-ttu-id="9ce5c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ce5c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ce5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ce5c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ce5c-120">Request headers</span></span>
|<span data-ttu-id="9ce5c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ce5c-121">Header</span></span>|<span data-ttu-id="9ce5c-122">値</span><span class="sxs-lookup"><span data-stu-id="9ce5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ce5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce5c-123">Authorization</span></span>|<span data-ttu-id="9ce5c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ce5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ce5c-125">Accept</span></span>|<span data-ttu-id="9ce5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ce5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ce5c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ce5c-127">Request body</span></span>
<span data-ttu-id="9ce5c-128">要求の本文に[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="9ce5c-129">[AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="9ce5c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ce5c-130">Property</span></span>|<span data-ttu-id="9ce5c-131">種類</span><span class="sxs-lookup"><span data-stu-id="9ce5c-131">Type</span></span>|<span data-ttu-id="9ce5c-132">説明</span><span class="sxs-lookup"><span data-stu-id="9ce5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce5c-133">ID</span><span class="sxs-lookup"><span data-stu-id="9ce5c-133">id</span></span>|<span data-ttu-id="9ce5c-134">String</span><span class="sxs-lookup"><span data-stu-id="9ce5c-134">String</span></span>|<span data-ttu-id="9ce5c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-135">Key of the entity.</span></span> <span data-ttu-id="9ce5c-136">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="9ce5c-137">targetedMobileApps</span></span>|<span data-ttu-id="9ce5c-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9ce5c-138">String collection</span></span>|<span data-ttu-id="9ce5c-139">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-139">the associated app.</span></span> <span data-ttu-id="9ce5c-140">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ce5c-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ce5c-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9ce5c-142">String collection</span></span>|<span data-ttu-id="9ce5c-143">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="9ce5c-144">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce5c-145">createdDateTime</span></span>|<span data-ttu-id="9ce5c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce5c-146">DateTimeOffset</span></span>|<span data-ttu-id="9ce5c-147">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-147">DateTime the object was created.</span></span> <span data-ttu-id="9ce5c-148">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-149">説明</span><span class="sxs-lookup"><span data-stu-id="9ce5c-149">description</span></span>|<span data-ttu-id="9ce5c-150">String</span><span class="sxs-lookup"><span data-stu-id="9ce5c-150">String</span></span>|<span data-ttu-id="9ce5c-151">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ce5c-152">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce5c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9ce5c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce5c-154">DateTimeOffset</span></span>|<span data-ttu-id="9ce5c-155">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-155">DateTime the object was last modified.</span></span> <span data-ttu-id="9ce5c-156">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-157">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce5c-157">displayName</span></span>|<span data-ttu-id="9ce5c-158">String</span><span class="sxs-lookup"><span data-stu-id="9ce5c-158">String</span></span>|<span data-ttu-id="9ce5c-159">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ce5c-160">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-161">version</span><span class="sxs-lookup"><span data-stu-id="9ce5c-161">version</span></span>|<span data-ttu-id="9ce5c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9ce5c-162">Int32</span></span>|<span data-ttu-id="9ce5c-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-163">Version of the device configuration.</span></span> <span data-ttu-id="9ce5c-164">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます</span><span class="sxs-lookup"><span data-stu-id="9ce5c-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9ce5c-165">packageId</span><span class="sxs-lookup"><span data-stu-id="9ce5c-165">packageId</span></span>|<span data-ttu-id="9ce5c-166">String</span><span class="sxs-lookup"><span data-stu-id="9ce5c-166">String</span></span>|<span data-ttu-id="9ce5c-167">Android の作業アプリケーションの構成のパッケージの id です。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="9ce5c-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="9ce5c-168">payloadJson</span></span>|<span data-ttu-id="9ce5c-169">String</span><span class="sxs-lookup"><span data-stu-id="9ce5c-169">String</span></span>|<span data-ttu-id="9ce5c-170">Android の作業アプリケーションの構成の JSON のペイロード。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="9ce5c-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="9ce5c-171">permissionActions</span></span>|<span data-ttu-id="9ce5c-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9ce5c-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="9ce5c-173">Android アプリケーションのアクセス許可とアクセス許可の対応するアクションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="9ce5c-174">応答</span><span class="sxs-lookup"><span data-stu-id="9ce5c-174">Response</span></span>
<span data-ttu-id="9ce5c-175">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce5c-176">例</span><span class="sxs-lookup"><span data-stu-id="9ce5c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ce5c-177">要求</span><span class="sxs-lookup"><span data-stu-id="9ce5c-177">Request</span></span>
<span data-ttu-id="9ce5c-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ce5c-179">応答</span><span class="sxs-lookup"><span data-stu-id="9ce5c-179">Response</span></span>
<span data-ttu-id="9ce5c-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ce5c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





