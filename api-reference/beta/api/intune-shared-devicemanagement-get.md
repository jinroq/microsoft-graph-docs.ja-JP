---
title: Get deviceManagement
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97c35f52182a82c2ddf2447e4d22935d8410826c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350917"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="7b891-103">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7b891-103">Get deviceManagement</span></span>

> <span data-ttu-id="7b891-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7b891-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b891-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b891-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b891-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b891-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b891-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7b891-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b891-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b891-108">Prerequisites</span></span>

<span data-ttu-id="7b891-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b891-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b891-111">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="7b891-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="7b891-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b891-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="7b891-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b891-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="7b891-114">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="7b891-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="7b891-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7b891-116">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="7b891-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="7b891-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7b891-118">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="7b891-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="7b891-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-120">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="7b891-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7b891-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7b891-122">&nbsp;&nbsp; **デバイスの目的**</span><span class="sxs-lookup"><span data-stu-id="7b891-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="7b891-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="7b891-124">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="7b891-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7b891-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7b891-126">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="7b891-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="7b891-127">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7b891-128">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="7b891-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="7b891-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-130">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="7b891-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="7b891-131">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7b891-132">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="7b891-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="7b891-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="7b891-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="7b891-135">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-136">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="7b891-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b891-137">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-138">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="7b891-138">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="7b891-139">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="7b891-140">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="7b891-140">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="7b891-141">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="7b891-142">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="7b891-142">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="7b891-143">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-144">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="7b891-144">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="7b891-145">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7b891-146">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="7b891-146">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7b891-147">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7b891-148">&nbsp; &nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="7b891-148">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="7b891-149">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b891-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7b891-150">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b891-150">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b891-151">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b891-151">Not supported.</span></span>|
| <span data-ttu-id="7b891-152">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b891-152">Application</span></span> | <span data-ttu-id="7b891-153">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b891-153">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="7b891-154">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b891-154">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b891-155">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b891-155">Optional query parameters</span></span>

<span data-ttu-id="7b891-156">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7b891-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b891-157">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b891-157">Request headers</span></span>
|<span data-ttu-id="7b891-158">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b891-158">Header</span></span>|<span data-ttu-id="7b891-159">値</span><span class="sxs-lookup"><span data-stu-id="7b891-159">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b891-160">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b891-160">Authorization</span></span>|<span data-ttu-id="7b891-161">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b891-161">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b891-162">承諾</span><span class="sxs-lookup"><span data-stu-id="7b891-162">Accept</span></span>|<span data-ttu-id="7b891-163">application/json</span><span class="sxs-lookup"><span data-stu-id="7b891-163">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b891-164">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b891-164">Request body</span></span>

<span data-ttu-id="7b891-165">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7b891-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b891-166">応答</span><span class="sxs-lookup"><span data-stu-id="7b891-166">Response</span></span>

<span data-ttu-id="7b891-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b891-167">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b891-168">例</span><span class="sxs-lookup"><span data-stu-id="7b891-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b891-169">要求</span><span class="sxs-lookup"><span data-stu-id="7b891-169">Request</span></span>

<span data-ttu-id="7b891-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b891-170">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="7b891-171">応答</span><span class="sxs-lookup"><span data-stu-id="7b891-171">Response</span></span>

<span data-ttu-id="7b891-172">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b891-172">Here are example of the response.</span></span> 

<span data-ttu-id="7b891-173">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7b891-173">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="7b891-174">ワークフローに適したプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7b891-174">Properties appropriate for the workflow are returned.</span></span>

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






