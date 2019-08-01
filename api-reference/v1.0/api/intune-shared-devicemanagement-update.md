---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b845a07d8199fcd4a997304f9095d7b364e0988a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023434"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="54ca8-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="54ca8-103">Update deviceManagement</span></span>

> <span data-ttu-id="54ca8-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54ca8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54ca8-105">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="54ca8-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54ca8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="54ca8-106">Prerequisites</span></span>
<span data-ttu-id="54ca8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54ca8-109">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="54ca8-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="54ca8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54ca8-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="54ca8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54ca8-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="54ca8-112">&nbsp;&nbsp;監査</span><span class="sxs-lookup"><span data-stu-id="54ca8-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="54ca8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-114">&nbsp;&nbsp;会社の使用条件</span><span class="sxs-lookup"><span data-stu-id="54ca8-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="54ca8-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-116">&nbsp;&nbsp;企業の登録</span><span class="sxs-lookup"><span data-stu-id="54ca8-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="54ca8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="54ca8-118">&nbsp;&nbsp;デバイス構成</span><span class="sxs-lookup"><span data-stu-id="54ca8-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="54ca8-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-120">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="54ca8-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="54ca8-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-122">&nbsp;&nbsp;エンドポイント保護</span><span class="sxs-lookup"><span data-stu-id="54ca8-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="54ca8-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-124">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="54ca8-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="54ca8-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-126">&nbsp;&nbsp;オンボード</span><span class="sxs-lookup"><span data-stu-id="54ca8-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="54ca8-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-128">&nbsp;&nbsp;役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="54ca8-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="54ca8-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-130">&nbsp;&nbsp;リモートアシスタンス</span><span class="sxs-lookup"><span data-stu-id="54ca8-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="54ca8-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-132">&nbsp;&nbsp;通信経費管理</span><span class="sxs-lookup"><span data-stu-id="54ca8-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="54ca8-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-134">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="54ca8-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="54ca8-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-136">&nbsp;&nbsp; Windows 情報保護</span><span class="sxs-lookup"><span data-stu-id="54ca8-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="54ca8-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ca8-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="54ca8-138">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54ca8-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54ca8-139">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54ca8-139">Not supported.</span></span>|
| <span data-ttu-id="54ca8-140">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54ca8-140">Application</span></span> | <span data-ttu-id="54ca8-141">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54ca8-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54ca8-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54ca8-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="54ca8-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54ca8-143">Request headers</span></span>
|<span data-ttu-id="54ca8-144">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54ca8-144">Header</span></span>|<span data-ttu-id="54ca8-145">値</span><span class="sxs-lookup"><span data-stu-id="54ca8-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54ca8-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="54ca8-146">Authorization</span></span>|<span data-ttu-id="54ca8-147">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="54ca8-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54ca8-148">承諾</span><span class="sxs-lookup"><span data-stu-id="54ca8-148">Accept</span></span>|<span data-ttu-id="54ca8-149">application/json</span><span class="sxs-lookup"><span data-stu-id="54ca8-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54ca8-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="54ca8-150">Request body</span></span>
<span data-ttu-id="54ca8-151">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="54ca8-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="54ca8-152">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="54ca8-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="54ca8-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54ca8-153">Property</span></span>|<span data-ttu-id="54ca8-154">型</span><span class="sxs-lookup"><span data-stu-id="54ca8-154">Type</span></span>|<span data-ttu-id="54ca8-155">説明</span><span class="sxs-lookup"><span data-stu-id="54ca8-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54ca8-156">id</span><span class="sxs-lookup"><span data-stu-id="54ca8-156">id</span></span>|<span data-ttu-id="54ca8-157">String</span><span class="sxs-lookup"><span data-stu-id="54ca8-157">String</span></span>|<span data-ttu-id="54ca8-158">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="54ca8-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="54ca8-159">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="54ca8-159">**Device configuration**</span></span>|
|<span data-ttu-id="54ca8-160">settings</span><span class="sxs-lookup"><span data-stu-id="54ca8-160">settings</span></span>|[<span data-ttu-id="54ca8-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="54ca8-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="54ca8-162">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="54ca8-162">Account level settings.</span></span>|
|<span data-ttu-id="54ca8-163">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="54ca8-163">**Device management**</span></span>|
|<span data-ttu-id="54ca8-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="54ca8-164">subscriptionState</span></span>|[<span data-ttu-id="54ca8-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="54ca8-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="54ca8-166">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="54ca8-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="54ca8-167">使用可能な値: `pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="54ca8-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="54ca8-168">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="54ca8-168">**Onboarding**</span></span>|
|<span data-ttu-id="54ca8-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="54ca8-169">intuneBrand</span></span>|[<span data-ttu-id="54ca8-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="54ca8-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="54ca8-171">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54ca8-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="54ca8-172">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="54ca8-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="54ca8-173">応答</span><span class="sxs-lookup"><span data-stu-id="54ca8-173">Response</span></span>
<span data-ttu-id="54ca8-174">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="54ca8-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54ca8-175">例</span><span class="sxs-lookup"><span data-stu-id="54ca8-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="54ca8-176">要求</span><span class="sxs-lookup"><span data-stu-id="54ca8-176">Request</span></span>
<span data-ttu-id="54ca8-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54ca8-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="54ca8-178">応答</span><span class="sxs-lookup"><span data-stu-id="54ca8-178">Response</span></span>

<span data-ttu-id="54ca8-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="54ca8-179">Here is an example of the response.</span></span> <span data-ttu-id="54ca8-180">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="54ca8-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="54ca8-181">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="54ca8-181">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



