---
title: deviceManagement の取得
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af4dc08832b09387774ad3ad1642b0103b3b7db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936929"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="15378-103">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="15378-103">Get deviceManagement</span></span>

> <span data-ttu-id="15378-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15378-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15378-105">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="15378-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15378-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="15378-106">Prerequisites</span></span>
<span data-ttu-id="15378-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15378-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15378-109">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="15378-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="15378-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15378-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="15378-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15378-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="15378-112">&nbsp;&nbsp;監査</span><span class="sxs-lookup"><span data-stu-id="15378-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="15378-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="15378-114">&nbsp;&nbsp;会社の用語</span><span class="sxs-lookup"><span data-stu-id="15378-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="15378-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-116">&nbsp;&nbsp;デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="15378-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="15378-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="15378-118">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="15378-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="15378-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="15378-120">&nbsp;&nbsp;登録</span><span class="sxs-lookup"><span data-stu-id="15378-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="15378-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-122">&nbsp;&nbsp;の通知</span><span class="sxs-lookup"><span data-stu-id="15378-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="15378-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-124">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="15378-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="15378-125">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="15378-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="15378-127">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="15378-128">&nbsp;&nbsp;リモート アシスタンス</span><span class="sxs-lookup"><span data-stu-id="15378-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="15378-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-130">&nbsp;&nbsp;通信経費の管理</span><span class="sxs-lookup"><span data-stu-id="15378-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="15378-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="15378-132">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="15378-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="15378-133">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="15378-134">&nbsp;&nbsp; Windows 情報の保護</span><span class="sxs-lookup"><span data-stu-id="15378-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="15378-135">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="15378-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="15378-136">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15378-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15378-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15378-137">Not supported.</span></span>|
| <span data-ttu-id="15378-138">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15378-138">Application</span></span> | <span data-ttu-id="15378-139">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15378-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="15378-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15378-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15378-141">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="15378-141">Optional query parameters</span></span>
<span data-ttu-id="15378-142">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15378-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="15378-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15378-143">Request headers</span></span>
|<span data-ttu-id="15378-144">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15378-144">Header</span></span>|<span data-ttu-id="15378-145">値</span><span class="sxs-lookup"><span data-stu-id="15378-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15378-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="15378-146">Authorization</span></span>|<span data-ttu-id="15378-147">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="15378-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15378-148">Accept</span><span class="sxs-lookup"><span data-stu-id="15378-148">Accept</span></span>|<span data-ttu-id="15378-149">application/json</span><span class="sxs-lookup"><span data-stu-id="15378-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15378-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="15378-150">Request body</span></span>
<span data-ttu-id="15378-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15378-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15378-152">応答</span><span class="sxs-lookup"><span data-stu-id="15378-152">Response</span></span>
<span data-ttu-id="15378-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15378-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15378-154">例</span><span class="sxs-lookup"><span data-stu-id="15378-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="15378-155">要求</span><span class="sxs-lookup"><span data-stu-id="15378-155">Request</span></span>
<span data-ttu-id="15378-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15378-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="15378-157">応答</span><span class="sxs-lookup"><span data-stu-id="15378-157">Response</span></span>
<span data-ttu-id="15378-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15378-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```



