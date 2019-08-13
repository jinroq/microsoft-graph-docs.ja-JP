---
title: deviceManagementPartner の作成
description: 新しい deviceManagementPartner オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20b021b41f73ae08973dfb10983d61b1963ffb26
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352743"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="53e4c-103">deviceManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="53e4c-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="53e4c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53e4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e4c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53e4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e4c-106">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="53e4c-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53e4c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="53e4c-107">Prerequisites</span></span>
<span data-ttu-id="53e4c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53e4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53e4c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53e4c-110">Permission type</span></span>|<span data-ttu-id="53e4c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53e4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53e4c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53e4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53e4c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e4c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53e4c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53e4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53e4c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53e4c-115">Not supported.</span></span>|
|<span data-ttu-id="53e4c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53e4c-116">Application</span></span>|<span data-ttu-id="53e4c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e4c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53e4c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53e4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="53e4c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53e4c-119">Request headers</span></span>
|<span data-ttu-id="53e4c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53e4c-120">Header</span></span>|<span data-ttu-id="53e4c-121">値</span><span class="sxs-lookup"><span data-stu-id="53e4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53e4c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53e4c-122">Authorization</span></span>|<span data-ttu-id="53e4c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="53e4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53e4c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="53e4c-124">Accept</span></span>|<span data-ttu-id="53e4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53e4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e4c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53e4c-126">Request body</span></span>
<span data-ttu-id="53e4c-127">要求本文で、deviceManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53e4c-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="53e4c-128">次の表に、deviceManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53e4c-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="53e4c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53e4c-129">Property</span></span>|<span data-ttu-id="53e4c-130">型</span><span class="sxs-lookup"><span data-stu-id="53e4c-130">Type</span></span>|<span data-ttu-id="53e4c-131">説明</span><span class="sxs-lookup"><span data-stu-id="53e4c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e4c-132">id</span><span class="sxs-lookup"><span data-stu-id="53e4c-132">id</span></span>|<span data-ttu-id="53e4c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="53e4c-133">String</span></span>|<span data-ttu-id="53e4c-134">エンティティの Id</span><span class="sxs-lookup"><span data-stu-id="53e4c-134">Id of the entity</span></span>|
|<span data-ttu-id="53e4c-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="53e4c-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="53e4c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e4c-136">DateTimeOffset</span></span>|<span data-ttu-id="53e4c-137">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="53e4c-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="53e4c-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="53e4c-138">partnerState</span></span>|[<span data-ttu-id="53e4c-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="53e4c-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="53e4c-140">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="53e4c-140">Partner state of this tenant.</span></span> <span data-ttu-id="53e4c-141">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="53e4c-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="53e4c-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="53e4c-142">partnerAppType</span></span>|[<span data-ttu-id="53e4c-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="53e4c-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="53e4c-144">パートナーアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="53e4c-144">Partner App type.</span></span> <span data-ttu-id="53e4c-145">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="53e4c-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="53e4c-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="53e4c-146">singleTenantAppId</span></span>|<span data-ttu-id="53e4c-147">String</span><span class="sxs-lookup"><span data-stu-id="53e4c-147">String</span></span>|<span data-ttu-id="53e4c-148">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="53e4c-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="53e4c-149">displayName</span><span class="sxs-lookup"><span data-stu-id="53e4c-149">displayName</span></span>|<span data-ttu-id="53e4c-150">String</span><span class="sxs-lookup"><span data-stu-id="53e4c-150">String</span></span>|<span data-ttu-id="53e4c-151">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="53e4c-151">Partner display name</span></span>|
|<span data-ttu-id="53e4c-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="53e4c-152">isConfigured</span></span>|<span data-ttu-id="53e4c-153">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="53e4c-153">Boolean</span></span>|<span data-ttu-id="53e4c-154">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="53e4c-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="53e4c-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="53e4c-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="53e4c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e4c-156">DateTimeOffset</span></span>|<span data-ttu-id="53e4c-157">パートナーデバイスが削除される日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="53e4c-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="53e4c-158">これはすぐに obselete になります。</span><span class="sxs-lookup"><span data-stu-id="53e4c-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="53e4c-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="53e4c-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="53e4c-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e4c-160">DateTimeOffset</span></span>|<span data-ttu-id="53e4c-161">パートナーデバイスが準拠していないとマークされるときの、UTC の DateTime。</span><span class="sxs-lookup"><span data-stu-id="53e4c-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="53e4c-162">これはすぐに obselete になります。</span><span class="sxs-lookup"><span data-stu-id="53e4c-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="53e4c-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="53e4c-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="53e4c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e4c-164">DateTimeOffset</span></span>|<span data-ttu-id="53e4c-165">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="53e4c-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="53e4c-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="53e4c-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="53e4c-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e4c-167">DateTimeOffset</span></span>|<span data-ttu-id="53e4c-168">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="53e4c-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="53e4c-169">応答</span><span class="sxs-lookup"><span data-stu-id="53e4c-169">Response</span></span>
<span data-ttu-id="53e4c-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53e4c-170">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e4c-171">例</span><span class="sxs-lookup"><span data-stu-id="53e4c-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="53e4c-172">要求</span><span class="sxs-lookup"><span data-stu-id="53e4c-172">Request</span></span>
<span data-ttu-id="53e4c-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53e4c-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="53e4c-174">応答</span><span class="sxs-lookup"><span data-stu-id="53e4c-174">Response</span></span>
<span data-ttu-id="53e4c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53e4c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 713

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```






