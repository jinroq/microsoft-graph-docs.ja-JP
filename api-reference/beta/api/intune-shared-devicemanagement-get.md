---
title: deviceManagement の取得
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c00b60793209904ce184de25f12f1f4ad14fad1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862637"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="b8ff3-103">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="b8ff3-103">Get deviceManagement</span></span>

> <span data-ttu-id="b8ff3-104">\*\*重要: \*\*Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8ff3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8ff3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8ff3-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8ff3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b8ff3-108">Prerequisites</span></span>

<span data-ttu-id="b8ff3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8ff3-111">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="b8ff3-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="b8ff3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8ff3-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="b8ff3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8ff3-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b8ff3-114">&nbsp;&nbsp; **Android の作業**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b8ff3-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b8ff3-116">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b8ff3-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b8ff3-118">&nbsp;&nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b8ff3-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-120">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b8ff3-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b8ff3-122">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b8ff3-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b8ff3-124">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b8ff3-125">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b8ff3-126">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b8ff3-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-128">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b8ff3-129">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b8ff3-130">&nbsp;&nbsp; **の通知**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b8ff3-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-132">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b8ff3-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b8ff3-135">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b8ff3-136">&nbsp;&nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b8ff3-137">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b8ff3-138">&nbsp;&nbsp; **リモート アシスタンス**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b8ff3-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-140">&nbsp;&nbsp; **通信経費の管理**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b8ff3-141">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b8ff3-142">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b8ff3-143">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b8ff3-144">&nbsp;&nbsp; **Windows 情報の保護**</span><span class="sxs-lookup"><span data-stu-id="b8ff3-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b8ff3-145">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8ff3-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b8ff3-146">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8ff3-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8ff3-147">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-147">Not supported.</span></span>|
| <span data-ttu-id="b8ff3-148">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8ff3-148">Application</span></span> | <span data-ttu-id="b8ff3-149">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="b8ff3-150">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8ff3-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8ff3-151">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b8ff3-151">Optional query parameters</span></span>

<span data-ttu-id="b8ff3-152">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8ff3-153">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8ff3-153">Request headers</span></span>
|<span data-ttu-id="b8ff3-154">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8ff3-154">Header</span></span>|<span data-ttu-id="b8ff3-155">値</span><span class="sxs-lookup"><span data-stu-id="b8ff3-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8ff3-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8ff3-156">Authorization</span></span>|<span data-ttu-id="b8ff3-157">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8ff3-158">Accept</span><span class="sxs-lookup"><span data-stu-id="b8ff3-158">Accept</span></span>|<span data-ttu-id="b8ff3-159">application/json</span><span class="sxs-lookup"><span data-stu-id="b8ff3-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8ff3-160">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8ff3-160">Request body</span></span>

<span data-ttu-id="b8ff3-161">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8ff3-162">応答</span><span class="sxs-lookup"><span data-stu-id="b8ff3-162">Response</span></span>

<span data-ttu-id="b8ff3-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8ff3-164">例</span><span class="sxs-lookup"><span data-stu-id="b8ff3-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8ff3-165">要求</span><span class="sxs-lookup"><span data-stu-id="b8ff3-165">Request</span></span>

<span data-ttu-id="b8ff3-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="b8ff3-167">応答</span><span class="sxs-lookup"><span data-stu-id="b8ff3-167">Response</span></span>

<span data-ttu-id="b8ff3-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-168">Here are example of the response.</span></span> 

<span data-ttu-id="b8ff3-169">注: ここに示す応答オブジェクトが簡潔にするために切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-169">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="b8ff3-170">ワークフローの適切なプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b8ff3-170">Properties appropriate for the workflow are returned.</span></span>

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



