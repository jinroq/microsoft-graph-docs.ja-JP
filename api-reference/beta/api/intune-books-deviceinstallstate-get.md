---
title: Get deviceInstallState
description: deviceInstallState オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a74deeea60f0b360ffb7f70bfe2e03f4a2210e3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919450"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="0baf4-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="0baf4-103">Get deviceInstallState</span></span>

> <span data-ttu-id="0baf4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0baf4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0baf4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0baf4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0baf4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0baf4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0baf4-107">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0baf4-107">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0baf4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0baf4-108">Prerequisites</span></span>
<span data-ttu-id="0baf4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0baf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0baf4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0baf4-111">Permission type</span></span>|<span data-ttu-id="0baf4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0baf4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0baf4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0baf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0baf4-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0baf4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0baf4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0baf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0baf4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0baf4-116">Not supported.</span></span>|
|<span data-ttu-id="0baf4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0baf4-117">Application</span></span>|<span data-ttu-id="0baf4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0baf4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0baf4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0baf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0baf4-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0baf4-120">Optional query parameters</span></span>
<span data-ttu-id="0baf4-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0baf4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0baf4-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0baf4-122">Request headers</span></span>
|<span data-ttu-id="0baf4-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0baf4-123">Header</span></span>|<span data-ttu-id="0baf4-124">値</span><span class="sxs-lookup"><span data-stu-id="0baf4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0baf4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0baf4-125">Authorization</span></span>|<span data-ttu-id="0baf4-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0baf4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0baf4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0baf4-127">Accept</span></span>|<span data-ttu-id="0baf4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0baf4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0baf4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0baf4-129">Request body</span></span>
<span data-ttu-id="0baf4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0baf4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0baf4-131">応答</span><span class="sxs-lookup"><span data-stu-id="0baf4-131">Response</span></span>
<span data-ttu-id="0baf4-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0baf4-132">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0baf4-133">例</span><span class="sxs-lookup"><span data-stu-id="0baf4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0baf4-134">要求</span><span class="sxs-lookup"><span data-stu-id="0baf4-134">Request</span></span>
<span data-ttu-id="0baf4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0baf4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="0baf4-136">応答</span><span class="sxs-lookup"><span data-stu-id="0baf4-136">Response</span></span>
<span data-ttu-id="0baf4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0baf4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceInstallState",
    "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "installState": "installed",
    "errorCode": "Error Code value",
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "userName": "User Name value"
  }
}
```





