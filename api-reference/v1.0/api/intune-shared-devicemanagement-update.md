---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7351eb15a194c68c4bd3b7abc59d866b5f4f237
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985971"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="fc3af-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="fc3af-103">Update deviceManagement</span></span>

> <span data-ttu-id="fc3af-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc3af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc3af-105">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fc3af-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc3af-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fc3af-106">Prerequisites</span></span>
<span data-ttu-id="fc3af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc3af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc3af-109">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="fc3af-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="fc3af-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc3af-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="fc3af-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc3af-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="fc3af-112">&nbsp;&nbsp;監査</span><span class="sxs-lookup"><span data-stu-id="fc3af-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="fc3af-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-114">&nbsp;&nbsp;会社の用語</span><span class="sxs-lookup"><span data-stu-id="fc3af-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="fc3af-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-116">&nbsp;&nbsp;企業登録</span><span class="sxs-lookup"><span data-stu-id="fc3af-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="fc3af-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="fc3af-118">&nbsp;&nbsp;デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="fc3af-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="fc3af-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-120">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="fc3af-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="fc3af-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-122">&nbsp;&nbsp;エンドポイントの保護</span><span class="sxs-lookup"><span data-stu-id="fc3af-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="fc3af-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-124">&nbsp;&nbsp;の通知</span><span class="sxs-lookup"><span data-stu-id="fc3af-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="fc3af-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-126">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="fc3af-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="fc3af-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-128">&nbsp;&nbsp;ロール ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="fc3af-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="fc3af-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-130">&nbsp;&nbsp;リモート アシスタンス</span><span class="sxs-lookup"><span data-stu-id="fc3af-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="fc3af-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-132">&nbsp;&nbsp;通信経費の管理</span><span class="sxs-lookup"><span data-stu-id="fc3af-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="fc3af-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-134">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="fc3af-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="fc3af-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-136">&nbsp;&nbsp; Windows 情報の保護</span><span class="sxs-lookup"><span data-stu-id="fc3af-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="fc3af-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3af-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="fc3af-138">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc3af-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc3af-139">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc3af-139">Not supported.</span></span>|
| <span data-ttu-id="fc3af-140">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc3af-140">Application</span></span> | <span data-ttu-id="fc3af-141">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc3af-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc3af-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc3af-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="fc3af-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc3af-143">Request headers</span></span>
|<span data-ttu-id="fc3af-144">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc3af-144">Header</span></span>|<span data-ttu-id="fc3af-145">値</span><span class="sxs-lookup"><span data-stu-id="fc3af-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc3af-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc3af-146">Authorization</span></span>|<span data-ttu-id="fc3af-147">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fc3af-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc3af-148">Accept</span><span class="sxs-lookup"><span data-stu-id="fc3af-148">Accept</span></span>|<span data-ttu-id="fc3af-149">application/json</span><span class="sxs-lookup"><span data-stu-id="fc3af-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc3af-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc3af-150">Request body</span></span>
<span data-ttu-id="fc3af-151">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc3af-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="fc3af-152">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fc3af-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="fc3af-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc3af-153">Property</span></span>|<span data-ttu-id="fc3af-154">種類</span><span class="sxs-lookup"><span data-stu-id="fc3af-154">Type</span></span>|<span data-ttu-id="fc3af-155">説明</span><span class="sxs-lookup"><span data-stu-id="fc3af-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc3af-156">ID</span><span class="sxs-lookup"><span data-stu-id="fc3af-156">id</span></span>|<span data-ttu-id="fc3af-157">String</span><span class="sxs-lookup"><span data-stu-id="fc3af-157">String</span></span>|<span data-ttu-id="fc3af-158">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="fc3af-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="fc3af-159">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="fc3af-159">**Device configuration**</span></span>|
|<span data-ttu-id="fc3af-160">settings</span><span class="sxs-lookup"><span data-stu-id="fc3af-160">settings</span></span>|[<span data-ttu-id="fc3af-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="fc3af-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="fc3af-162">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="fc3af-162">Account level settings.</span></span>|
|<span data-ttu-id="fc3af-163">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="fc3af-163">**Device management**</span></span>|
|<span data-ttu-id="fc3af-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="fc3af-164">subscriptionState</span></span>|[<span data-ttu-id="fc3af-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="fc3af-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="fc3af-166">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="fc3af-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="fc3af-167">可能な値: `pending`、 `active`、 `warning`、 `disabled`、 `deleted`、 `blocked`、 `lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="fc3af-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="fc3af-168">**契約時**</span><span class="sxs-lookup"><span data-stu-id="fc3af-168">**Onboarding**</span></span>|
|<span data-ttu-id="fc3af-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="fc3af-169">intuneBrand</span></span>|[<span data-ttu-id="fc3af-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="fc3af-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="fc3af-171">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc3af-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="fc3af-172">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="fc3af-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="fc3af-173">応答</span><span class="sxs-lookup"><span data-stu-id="fc3af-173">Response</span></span>
<span data-ttu-id="fc3af-174">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fc3af-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc3af-175">例</span><span class="sxs-lookup"><span data-stu-id="fc3af-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc3af-176">要求</span><span class="sxs-lookup"><span data-stu-id="fc3af-176">Request</span></span>
<span data-ttu-id="fc3af-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fc3af-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc3af-178">応答</span><span class="sxs-lookup"><span data-stu-id="fc3af-178">Response</span></span>

<span data-ttu-id="fc3af-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fc3af-179">Here is an example of the response.</span></span> <span data-ttu-id="fc3af-180">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fc3af-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fc3af-181">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="fc3af-181">Returned properties vary according to workflow and context.</span></span>

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



