---
title: deviceManagementPartner の作成
description: 新しい deviceManagementPartner オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b9ff6eab5bf04277d89616765fb14855d047450c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991084"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="bae60-103">deviceManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="bae60-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="bae60-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bae60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bae60-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bae60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bae60-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bae60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bae60-107">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bae60-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bae60-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bae60-108">Prerequisites</span></span>
<span data-ttu-id="bae60-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bae60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae60-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bae60-111">Permission type</span></span>|<span data-ttu-id="bae60-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bae60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bae60-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bae60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bae60-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae60-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bae60-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bae60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bae60-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bae60-116">Not supported.</span></span>|
|<span data-ttu-id="bae60-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bae60-117">Application</span></span>|<span data-ttu-id="bae60-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bae60-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bae60-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bae60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="bae60-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae60-120">Request headers</span></span>
|<span data-ttu-id="bae60-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae60-121">Header</span></span>|<span data-ttu-id="bae60-122">値</span><span class="sxs-lookup"><span data-stu-id="bae60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bae60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae60-123">Authorization</span></span>|<span data-ttu-id="bae60-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bae60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bae60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bae60-125">Accept</span></span>|<span data-ttu-id="bae60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bae60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae60-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bae60-127">Request body</span></span>
<span data-ttu-id="bae60-128">要求本文で、deviceManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bae60-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="bae60-129">次の表に、deviceManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bae60-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="bae60-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bae60-130">Property</span></span>|<span data-ttu-id="bae60-131">型</span><span class="sxs-lookup"><span data-stu-id="bae60-131">Type</span></span>|<span data-ttu-id="bae60-132">説明</span><span class="sxs-lookup"><span data-stu-id="bae60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bae60-133">ID</span><span class="sxs-lookup"><span data-stu-id="bae60-133">id</span></span>|<span data-ttu-id="bae60-134">String</span><span class="sxs-lookup"><span data-stu-id="bae60-134">String</span></span>|<span data-ttu-id="bae60-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bae60-135">Not yet documented</span></span>|
|<span data-ttu-id="bae60-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="bae60-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="bae60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae60-137">DateTimeOffset</span></span>|<span data-ttu-id="bae60-138">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="bae60-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="bae60-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="bae60-139">partnerState</span></span>|[<span data-ttu-id="bae60-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="bae60-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="bae60-141">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="bae60-141">Partner state of this tenant.</span></span> <span data-ttu-id="bae60-142">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="bae60-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="bae60-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="bae60-143">partnerAppType</span></span>|[<span data-ttu-id="bae60-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="bae60-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="bae60-145">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="bae60-145">Partner App type.</span></span> <span data-ttu-id="bae60-146">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="bae60-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="bae60-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="bae60-147">singleTenantAppId</span></span>|<span data-ttu-id="bae60-148">String</span><span class="sxs-lookup"><span data-stu-id="bae60-148">String</span></span>|<span data-ttu-id="bae60-149">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="bae60-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="bae60-150">displayName</span><span class="sxs-lookup"><span data-stu-id="bae60-150">displayName</span></span>|<span data-ttu-id="bae60-151">String</span><span class="sxs-lookup"><span data-stu-id="bae60-151">String</span></span>|<span data-ttu-id="bae60-152">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="bae60-152">Partner display name</span></span>|
|<span data-ttu-id="bae60-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="bae60-153">isConfigured</span></span>|<span data-ttu-id="bae60-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="bae60-154">Boolean</span></span>|<span data-ttu-id="bae60-155">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="bae60-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="bae60-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="bae60-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="bae60-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae60-157">DateTimeOffset</span></span>|<span data-ttu-id="bae60-158">PartnerDevices が削除されるときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="bae60-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="bae60-159">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="bae60-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="bae60-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="bae60-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="bae60-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae60-161">DateTimeOffset</span></span>|<span data-ttu-id="bae60-162">PartnerDevices は、非準拠とマークするときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="bae60-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="bae60-163">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="bae60-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="bae60-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="bae60-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="bae60-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae60-165">DateTimeOffset</span></span>|<span data-ttu-id="bae60-166">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="bae60-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="bae60-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="bae60-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="bae60-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae60-168">DateTimeOffset</span></span>|<span data-ttu-id="bae60-169">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="bae60-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="bae60-170">応答</span><span class="sxs-lookup"><span data-stu-id="bae60-170">Response</span></span>
<span data-ttu-id="bae60-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bae60-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae60-172">例</span><span class="sxs-lookup"><span data-stu-id="bae60-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="bae60-173">要求</span><span class="sxs-lookup"><span data-stu-id="bae60-173">Request</span></span>
<span data-ttu-id="bae60-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bae60-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bae60-175">応答</span><span class="sxs-lookup"><span data-stu-id="bae60-175">Response</span></span>
<span data-ttu-id="bae60-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bae60-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





