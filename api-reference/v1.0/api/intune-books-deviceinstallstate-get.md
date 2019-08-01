---
title: Get deviceInstallState
description: deviceInstallState オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5612e13c536400a83d3f395a8c04627b18ae4434
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001923"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="384cc-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="384cc-103">Get deviceInstallState</span></span>

> <span data-ttu-id="384cc-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="384cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="384cc-105">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="384cc-105">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="384cc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="384cc-106">Prerequisites</span></span>
<span data-ttu-id="384cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="384cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="384cc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="384cc-109">Permission type</span></span>|<span data-ttu-id="384cc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="384cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="384cc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="384cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="384cc-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="384cc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="384cc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="384cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="384cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="384cc-114">Not supported.</span></span>|
|<span data-ttu-id="384cc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="384cc-115">Application</span></span>|<span data-ttu-id="384cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="384cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="384cc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="384cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="384cc-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="384cc-118">Optional query parameters</span></span>
<span data-ttu-id="384cc-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="384cc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="384cc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="384cc-120">Request headers</span></span>
|<span data-ttu-id="384cc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="384cc-121">Header</span></span>|<span data-ttu-id="384cc-122">値</span><span class="sxs-lookup"><span data-stu-id="384cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="384cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="384cc-123">Authorization</span></span>|<span data-ttu-id="384cc-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="384cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="384cc-125">承諾</span><span class="sxs-lookup"><span data-stu-id="384cc-125">Accept</span></span>|<span data-ttu-id="384cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="384cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="384cc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="384cc-127">Request body</span></span>
<span data-ttu-id="384cc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="384cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="384cc-129">応答</span><span class="sxs-lookup"><span data-stu-id="384cc-129">Response</span></span>
<span data-ttu-id="384cc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="384cc-130">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="384cc-131">例</span><span class="sxs-lookup"><span data-stu-id="384cc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="384cc-132">要求</span><span class="sxs-lookup"><span data-stu-id="384cc-132">Request</span></span>
<span data-ttu-id="384cc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="384cc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="384cc-134">応答</span><span class="sxs-lookup"><span data-stu-id="384cc-134">Response</span></span>
<span data-ttu-id="384cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="384cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



