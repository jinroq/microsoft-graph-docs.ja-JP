---
title: WindowsProtectionState を取得します。
description: WindowsProtectionState オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: 064b47a9595838d0e77a5378b6238e9f6fd227b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069278"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="5b34d-103">WindowsProtectionState を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b34d-103">Get windowsProtectionState</span></span>

> <span data-ttu-id="5b34d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b34d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b34d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b34d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b34d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b34d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b34d-107">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b34d-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b34d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5b34d-108">Prerequisites</span></span>
<span data-ttu-id="5b34d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b34d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b34d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b34d-111">Permission type</span></span>|<span data-ttu-id="5b34d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b34d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b34d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b34d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b34d-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b34d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5b34d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b34d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b34d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b34d-116">Not supported.</span></span>|
|<span data-ttu-id="5b34d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b34d-117">Application</span></span>|<span data-ttu-id="5b34d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b34d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b34d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b34d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b34d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b34d-120">Optional query parameters</span></span>
<span data-ttu-id="5b34d-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b34d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b34d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b34d-122">Request headers</span></span>
|<span data-ttu-id="5b34d-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b34d-123">Header</span></span>|<span data-ttu-id="5b34d-124">値</span><span class="sxs-lookup"><span data-stu-id="5b34d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b34d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b34d-125">Authorization</span></span>|<span data-ttu-id="5b34d-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5b34d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b34d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5b34d-127">Accept</span></span>|<span data-ttu-id="5b34d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b34d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b34d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b34d-129">Request body</span></span>
<span data-ttu-id="5b34d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b34d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b34d-131">応答</span><span class="sxs-lookup"><span data-stu-id="5b34d-131">Response</span></span>
<span data-ttu-id="5b34d-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5b34d-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b34d-133">例</span><span class="sxs-lookup"><span data-stu-id="5b34d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b34d-134">要求</span><span class="sxs-lookup"><span data-stu-id="5b34d-134">Request</span></span>
<span data-ttu-id="5b34d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b34d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="5b34d-136">応答</span><span class="sxs-lookup"><span data-stu-id="5b34d-136">Response</span></span>
<span data-ttu-id="5b34d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b34d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





