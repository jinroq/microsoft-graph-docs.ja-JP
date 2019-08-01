---
title: deviceManagementPartner の更新
description: deviceManagementPartner オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7bcbe549357c7f89702acf2194b153230356e20
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024183"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="1f89b-103">deviceManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="1f89b-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="1f89b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f89b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f89b-105">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f89b-105">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f89b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f89b-106">Prerequisites</span></span>
<span data-ttu-id="1f89b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f89b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f89b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f89b-109">Permission type</span></span>|<span data-ttu-id="1f89b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f89b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f89b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f89b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f89b-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f89b-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f89b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f89b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f89b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f89b-114">Not supported.</span></span>|
|<span data-ttu-id="1f89b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f89b-115">Application</span></span>|<span data-ttu-id="1f89b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f89b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f89b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f89b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="1f89b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f89b-118">Request headers</span></span>
|<span data-ttu-id="1f89b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f89b-119">Header</span></span>|<span data-ttu-id="1f89b-120">値</span><span class="sxs-lookup"><span data-stu-id="1f89b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f89b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f89b-121">Authorization</span></span>|<span data-ttu-id="1f89b-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f89b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f89b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1f89b-123">Accept</span></span>|<span data-ttu-id="1f89b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f89b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f89b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f89b-125">Request body</span></span>
<span data-ttu-id="1f89b-126">要求本文で、[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f89b-126">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="1f89b-127">次の表に、[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1f89b-127">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="1f89b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f89b-128">Property</span></span>|<span data-ttu-id="1f89b-129">型</span><span class="sxs-lookup"><span data-stu-id="1f89b-129">Type</span></span>|<span data-ttu-id="1f89b-130">説明</span><span class="sxs-lookup"><span data-stu-id="1f89b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f89b-131">id</span><span class="sxs-lookup"><span data-stu-id="1f89b-131">id</span></span>|<span data-ttu-id="1f89b-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1f89b-132">String</span></span>|<span data-ttu-id="1f89b-133">エンティティの Id</span><span class="sxs-lookup"><span data-stu-id="1f89b-133">Id of the entity</span></span>|
|<span data-ttu-id="1f89b-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1f89b-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1f89b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f89b-135">DateTimeOffset</span></span>|<span data-ttu-id="1f89b-136">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="1f89b-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="1f89b-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="1f89b-137">partnerState</span></span>|[<span data-ttu-id="1f89b-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1f89b-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="1f89b-139">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="1f89b-139">Partner state of this tenant.</span></span> <span data-ttu-id="1f89b-140">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="1f89b-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="1f89b-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="1f89b-141">partnerAppType</span></span>|[<span data-ttu-id="1f89b-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="1f89b-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="1f89b-143">パートナーアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="1f89b-143">Partner App type.</span></span> <span data-ttu-id="1f89b-144">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="1f89b-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="1f89b-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="1f89b-145">singleTenantAppId</span></span>|<span data-ttu-id="1f89b-146">String</span><span class="sxs-lookup"><span data-stu-id="1f89b-146">String</span></span>|<span data-ttu-id="1f89b-147">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="1f89b-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="1f89b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1f89b-148">displayName</span></span>|<span data-ttu-id="1f89b-149">String</span><span class="sxs-lookup"><span data-stu-id="1f89b-149">String</span></span>|<span data-ttu-id="1f89b-150">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="1f89b-150">Partner display name</span></span>|
|<span data-ttu-id="1f89b-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="1f89b-151">isConfigured</span></span>|<span data-ttu-id="1f89b-152">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f89b-152">Boolean</span></span>|<span data-ttu-id="1f89b-153">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="1f89b-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="1f89b-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f89b-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="1f89b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f89b-155">DateTimeOffset</span></span>|<span data-ttu-id="1f89b-156">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="1f89b-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="1f89b-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="1f89b-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="1f89b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f89b-158">DateTimeOffset</span></span>|<span data-ttu-id="1f89b-159">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="1f89b-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="1f89b-160">応答</span><span class="sxs-lookup"><span data-stu-id="1f89b-160">Response</span></span>
<span data-ttu-id="1f89b-161">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1f89b-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f89b-162">例</span><span class="sxs-lookup"><span data-stu-id="1f89b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f89b-163">要求</span><span class="sxs-lookup"><span data-stu-id="1f89b-163">Request</span></span>
<span data-ttu-id="1f89b-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f89b-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1f89b-165">応答</span><span class="sxs-lookup"><span data-stu-id="1f89b-165">Response</span></span>
<span data-ttu-id="1f89b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f89b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



