---
title: deviceManagementPartner の更新
description: deviceManagementPartner オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 47aba10ebe744d4f8211081e5c947df4d61599ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356323"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="81b65-103">deviceManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="81b65-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="81b65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81b65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81b65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81b65-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81b65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81b65-107">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="81b65-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81b65-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="81b65-108">Prerequisites</span></span>
<span data-ttu-id="81b65-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81b65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81b65-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81b65-111">Permission type</span></span>|<span data-ttu-id="81b65-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81b65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81b65-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81b65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81b65-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b65-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81b65-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81b65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81b65-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b65-116">Not supported.</span></span>|
|<span data-ttu-id="81b65-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81b65-117">Application</span></span>|<span data-ttu-id="81b65-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81b65-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81b65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="81b65-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81b65-120">Request headers</span></span>
|<span data-ttu-id="81b65-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81b65-121">Header</span></span>|<span data-ttu-id="81b65-122">値</span><span class="sxs-lookup"><span data-stu-id="81b65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81b65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81b65-123">Authorization</span></span>|<span data-ttu-id="81b65-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="81b65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81b65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81b65-125">Accept</span></span>|<span data-ttu-id="81b65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81b65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81b65-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="81b65-127">Request body</span></span>
<span data-ttu-id="81b65-128">要求本文で、[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81b65-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="81b65-129">次の表に、[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="81b65-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="81b65-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81b65-130">Property</span></span>|<span data-ttu-id="81b65-131">種類</span><span class="sxs-lookup"><span data-stu-id="81b65-131">Type</span></span>|<span data-ttu-id="81b65-132">説明</span><span class="sxs-lookup"><span data-stu-id="81b65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b65-133">ID</span><span class="sxs-lookup"><span data-stu-id="81b65-133">id</span></span>|<span data-ttu-id="81b65-134">String</span><span class="sxs-lookup"><span data-stu-id="81b65-134">String</span></span>|<span data-ttu-id="81b65-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="81b65-135">Not yet documented</span></span>|
|<span data-ttu-id="81b65-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="81b65-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="81b65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b65-137">DateTimeOffset</span></span>|<span data-ttu-id="81b65-138">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="81b65-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="81b65-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="81b65-139">partnerState</span></span>|[<span data-ttu-id="81b65-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="81b65-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="81b65-141">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="81b65-141">Partner state of this tenant.</span></span> <span data-ttu-id="81b65-142">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="81b65-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="81b65-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="81b65-143">partnerAppType</span></span>|[<span data-ttu-id="81b65-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="81b65-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="81b65-145">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="81b65-145">Partner App type.</span></span> <span data-ttu-id="81b65-146">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="81b65-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="81b65-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="81b65-147">singleTenantAppId</span></span>|<span data-ttu-id="81b65-148">String</span><span class="sxs-lookup"><span data-stu-id="81b65-148">String</span></span>|<span data-ttu-id="81b65-149">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="81b65-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="81b65-150">displayName</span><span class="sxs-lookup"><span data-stu-id="81b65-150">displayName</span></span>|<span data-ttu-id="81b65-151">String</span><span class="sxs-lookup"><span data-stu-id="81b65-151">String</span></span>|<span data-ttu-id="81b65-152">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="81b65-152">Partner display name</span></span>|
|<span data-ttu-id="81b65-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="81b65-153">isConfigured</span></span>|<span data-ttu-id="81b65-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="81b65-154">Boolean</span></span>|<span data-ttu-id="81b65-155">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="81b65-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="81b65-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="81b65-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="81b65-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b65-157">DateTimeOffset</span></span>|<span data-ttu-id="81b65-158">PartnerDevices が削除されるときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="81b65-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="81b65-159">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="81b65-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="81b65-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="81b65-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="81b65-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b65-161">DateTimeOffset</span></span>|<span data-ttu-id="81b65-162">PartnerDevices は、非準拠とマークするときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="81b65-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="81b65-163">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="81b65-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="81b65-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="81b65-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="81b65-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b65-165">DateTimeOffset</span></span>|<span data-ttu-id="81b65-166">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="81b65-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="81b65-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="81b65-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="81b65-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b65-168">DateTimeOffset</span></span>|<span data-ttu-id="81b65-169">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="81b65-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="81b65-170">応答</span><span class="sxs-lookup"><span data-stu-id="81b65-170">Response</span></span>
<span data-ttu-id="81b65-171">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="81b65-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81b65-172">例</span><span class="sxs-lookup"><span data-stu-id="81b65-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="81b65-173">要求</span><span class="sxs-lookup"><span data-stu-id="81b65-173">Request</span></span>
<span data-ttu-id="81b65-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81b65-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="81b65-175">応答</span><span class="sxs-lookup"><span data-stu-id="81b65-175">Response</span></span>
<span data-ttu-id="81b65-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81b65-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




