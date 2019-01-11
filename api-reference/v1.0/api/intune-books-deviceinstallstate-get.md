---
title: Get deviceInstallState
description: deviceInstallState オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edb1b3a26164c8c49206c12d372cf172582e87b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860313"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="f4986-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f4986-103">Get deviceInstallState</span></span>

> <span data-ttu-id="f4986-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4986-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4986-105">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4986-105">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4986-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4986-106">Prerequisites</span></span>
<span data-ttu-id="f4986-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4986-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4986-109">Permission type</span></span>|<span data-ttu-id="f4986-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4986-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4986-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4986-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4986-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4986-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4986-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4986-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4986-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4986-114">Not supported.</span></span>|
|<span data-ttu-id="f4986-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4986-115">Application</span></span>|<span data-ttu-id="f4986-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4986-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4986-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4986-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4986-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4986-118">Optional query parameters</span></span>
<span data-ttu-id="f4986-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4986-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f4986-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4986-120">Request headers</span></span>
|<span data-ttu-id="f4986-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4986-121">Header</span></span>|<span data-ttu-id="f4986-122">値</span><span class="sxs-lookup"><span data-stu-id="f4986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4986-123">Authorization</span></span>|<span data-ttu-id="f4986-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4986-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4986-125">Accept</span></span>|<span data-ttu-id="f4986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4986-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4986-127">Request body</span></span>
<span data-ttu-id="f4986-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4986-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4986-129">応答</span><span class="sxs-lookup"><span data-stu-id="f4986-129">Response</span></span>
<span data-ttu-id="f4986-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4986-130">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4986-131">例</span><span class="sxs-lookup"><span data-stu-id="f4986-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4986-132">要求</span><span class="sxs-lookup"><span data-stu-id="f4986-132">Request</span></span>
<span data-ttu-id="f4986-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4986-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="f4986-134">応答</span><span class="sxs-lookup"><span data-stu-id="f4986-134">Response</span></span>
<span data-ttu-id="f4986-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4986-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



