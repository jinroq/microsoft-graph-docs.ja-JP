---
title: deviceManagementPartner の作成
description: 新しい deviceManagementPartner オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e343b507d81d4d33ca61845e5e9810a09ca700b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412773"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="6e9e5-103">deviceManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="6e9e5-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="6e9e5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e9e5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e9e5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e9e5-107">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e9e5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6e9e5-108">Prerequisites</span></span>
<span data-ttu-id="6e9e5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e9e5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e9e5-111">Permission type</span></span>|<span data-ttu-id="6e9e5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e9e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e9e5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e9e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e9e5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e9e5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e9e5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e9e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e9e5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-116">Not supported.</span></span>|
|<span data-ttu-id="6e9e5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e9e5-117">Application</span></span>|<span data-ttu-id="6e9e5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e9e5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e9e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="6e9e5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e9e5-120">Request headers</span></span>
|<span data-ttu-id="6e9e5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e9e5-121">Header</span></span>|<span data-ttu-id="6e9e5-122">値</span><span class="sxs-lookup"><span data-stu-id="6e9e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e9e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e9e5-123">Authorization</span></span>|<span data-ttu-id="6e9e5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e9e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e9e5-125">Accept</span></span>|<span data-ttu-id="6e9e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e9e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e9e5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e9e5-127">Request body</span></span>
<span data-ttu-id="6e9e5-128">要求本文で、deviceManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="6e9e5-129">次の表に、deviceManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="6e9e5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e9e5-130">Property</span></span>|<span data-ttu-id="6e9e5-131">型</span><span class="sxs-lookup"><span data-stu-id="6e9e5-131">Type</span></span>|<span data-ttu-id="6e9e5-132">説明</span><span class="sxs-lookup"><span data-stu-id="6e9e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e9e5-133">id</span><span class="sxs-lookup"><span data-stu-id="6e9e5-133">id</span></span>|<span data-ttu-id="6e9e5-134">String</span><span class="sxs-lookup"><span data-stu-id="6e9e5-134">String</span></span>|<span data-ttu-id="6e9e5-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6e9e5-135">Not yet documented</span></span>|
|<span data-ttu-id="6e9e5-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6e9e5-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6e9e5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e9e5-137">DateTimeOffset</span></span>|<span data-ttu-id="6e9e5-138">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="6e9e5-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="6e9e5-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="6e9e5-139">partnerState</span></span>|[<span data-ttu-id="6e9e5-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="6e9e5-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="6e9e5-141">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-141">Partner state of this tenant.</span></span> <span data-ttu-id="6e9e5-142">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="6e9e5-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="6e9e5-143">partnerAppType</span></span>|[<span data-ttu-id="6e9e5-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="6e9e5-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="6e9e5-145">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-145">Partner App type.</span></span> <span data-ttu-id="6e9e5-146">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="6e9e5-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="6e9e5-147">singleTenantAppId</span></span>|<span data-ttu-id="6e9e5-148">String</span><span class="sxs-lookup"><span data-stu-id="6e9e5-148">String</span></span>|<span data-ttu-id="6e9e5-149">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="6e9e5-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="6e9e5-150">displayName</span><span class="sxs-lookup"><span data-stu-id="6e9e5-150">displayName</span></span>|<span data-ttu-id="6e9e5-151">String</span><span class="sxs-lookup"><span data-stu-id="6e9e5-151">String</span></span>|<span data-ttu-id="6e9e5-152">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="6e9e5-152">Partner display name</span></span>|
|<span data-ttu-id="6e9e5-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="6e9e5-153">isConfigured</span></span>|<span data-ttu-id="6e9e5-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e9e5-154">Boolean</span></span>|<span data-ttu-id="6e9e5-155">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="6e9e5-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="6e9e5-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="6e9e5-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="6e9e5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e9e5-157">DateTimeOffset</span></span>|<span data-ttu-id="6e9e5-158">PartnerDevices が削除されるときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="6e9e5-159">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="6e9e5-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="6e9e5-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="6e9e5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e9e5-161">DateTimeOffset</span></span>|<span data-ttu-id="6e9e5-162">PartnerDevices は、非準拠とマークするときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="6e9e5-163">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="6e9e5-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e9e5-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="6e9e5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e9e5-165">DateTimeOffset</span></span>|<span data-ttu-id="6e9e5-166">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="6e9e5-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="6e9e5-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="6e9e5-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="6e9e5-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e9e5-168">DateTimeOffset</span></span>|<span data-ttu-id="6e9e5-169">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="6e9e5-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="6e9e5-170">応答</span><span class="sxs-lookup"><span data-stu-id="6e9e5-170">Response</span></span>
<span data-ttu-id="6e9e5-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e9e5-172">例</span><span class="sxs-lookup"><span data-stu-id="6e9e5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e9e5-173">要求</span><span class="sxs-lookup"><span data-stu-id="6e9e5-173">Request</span></span>
<span data-ttu-id="6e9e5-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e9e5-175">応答</span><span class="sxs-lookup"><span data-stu-id="6e9e5-175">Response</span></span>
<span data-ttu-id="6e9e5-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e9e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




