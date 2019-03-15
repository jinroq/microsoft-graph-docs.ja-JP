---
title: Get deviceManagement
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4a07c2645686722c59e45f039aacb9dc3627a5d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570620"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="d1c55-103">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d1c55-103">Get deviceManagement</span></span>

> <span data-ttu-id="d1c55-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d1c55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1c55-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1c55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1c55-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c55-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d1c55-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1c55-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1c55-108">Prerequisites</span></span>

<span data-ttu-id="d1c55-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1c55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

| <span data-ttu-id="d1c55-111">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="d1c55-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="d1c55-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1c55-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="d1c55-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1c55-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="d1c55-114">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="d1c55-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d1c55-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d1c55-116">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="d1c55-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d1c55-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d1c55-118">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="d1c55-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d1c55-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-120">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="d1c55-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d1c55-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d1c55-122">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="d1c55-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d1c55-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d1c55-124">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="d1c55-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d1c55-125">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d1c55-126">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="d1c55-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d1c55-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-128">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="d1c55-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d1c55-129">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d1c55-130">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="d1c55-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d1c55-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-132">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="d1c55-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d1c55-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="d1c55-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="d1c55-135">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="d1c55-136">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="d1c55-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d1c55-137">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d1c55-138">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="d1c55-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d1c55-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-140">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="d1c55-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d1c55-141">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d1c55-142">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="d1c55-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d1c55-143">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d1c55-144">&nbsp;&nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="d1c55-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d1c55-145">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c55-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d1c55-146">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1c55-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1c55-147">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1c55-147">Not supported.</span></span>|
| <span data-ttu-id="d1c55-148">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1c55-148">Application</span></span> | <span data-ttu-id="d1c55-149">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1c55-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="d1c55-150">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1c55-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1c55-151">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d1c55-151">Optional query parameters</span></span>

<span data-ttu-id="d1c55-152">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d1c55-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1c55-153">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1c55-153">Request headers</span></span>
|<span data-ttu-id="d1c55-154">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1c55-154">Header</span></span>|<span data-ttu-id="d1c55-155">値</span><span class="sxs-lookup"><span data-stu-id="d1c55-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1c55-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1c55-156">Authorization</span></span>|<span data-ttu-id="d1c55-157">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1c55-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1c55-158">承諾</span><span class="sxs-lookup"><span data-stu-id="d1c55-158">Accept</span></span>|<span data-ttu-id="d1c55-159">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c55-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c55-160">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1c55-160">Request body</span></span>

<span data-ttu-id="d1c55-161">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1c55-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1c55-162">応答</span><span class="sxs-lookup"><span data-stu-id="d1c55-162">Response</span></span>

<span data-ttu-id="d1c55-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1c55-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c55-164">例</span><span class="sxs-lookup"><span data-stu-id="d1c55-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c55-165">要求</span><span class="sxs-lookup"><span data-stu-id="d1c55-165">Request</span></span>

<span data-ttu-id="d1c55-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1c55-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="d1c55-167">応答</span><span class="sxs-lookup"><span data-stu-id="d1c55-167">Response</span></span>

<span data-ttu-id="d1c55-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1c55-168">Here are example of the response.</span></span> 

<span data-ttu-id="d1c55-169">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d1c55-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="d1c55-170">ワークフローに適したプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1c55-170">Properties appropriate for the workflow are returned.</span></span>

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



