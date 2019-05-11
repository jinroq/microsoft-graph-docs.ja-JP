---
title: DeviceManagementScriptGroupAssignment の取得
description: DeviceManagementScriptGroupAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efd3eca64ce9452eaa16abd2b89e273fbdb79317
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909996"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="69e64-103">DeviceManagementScriptGroupAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="69e64-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="69e64-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69e64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69e64-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69e64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69e64-106">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="69e64-106">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69e64-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="69e64-107">Prerequisites</span></span>
<span data-ttu-id="69e64-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69e64-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69e64-110">Permission type</span></span>|<span data-ttu-id="69e64-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69e64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69e64-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69e64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69e64-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69e64-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="69e64-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69e64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69e64-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69e64-115">Not supported.</span></span>|
|<span data-ttu-id="69e64-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69e64-116">Application</span></span>|<span data-ttu-id="69e64-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69e64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69e64-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69e64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69e64-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="69e64-119">Optional query parameters</span></span>
<span data-ttu-id="69e64-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="69e64-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69e64-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69e64-121">Request headers</span></span>
|<span data-ttu-id="69e64-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69e64-122">Header</span></span>|<span data-ttu-id="69e64-123">値</span><span class="sxs-lookup"><span data-stu-id="69e64-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69e64-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69e64-124">Authorization</span></span>|<span data-ttu-id="69e64-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="69e64-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69e64-126">承諾</span><span class="sxs-lookup"><span data-stu-id="69e64-126">Accept</span></span>|<span data-ttu-id="69e64-127">application/json</span><span class="sxs-lookup"><span data-stu-id="69e64-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69e64-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="69e64-128">Request body</span></span>
<span data-ttu-id="69e64-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="69e64-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69e64-130">応答</span><span class="sxs-lookup"><span data-stu-id="69e64-130">Response</span></span>
<span data-ttu-id="69e64-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69e64-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69e64-132">例</span><span class="sxs-lookup"><span data-stu-id="69e64-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="69e64-133">要求</span><span class="sxs-lookup"><span data-stu-id="69e64-133">Request</span></span>
<span data-ttu-id="69e64-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69e64-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="69e64-135">応答</span><span class="sxs-lookup"><span data-stu-id="69e64-135">Response</span></span>
<span data-ttu-id="69e64-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69e64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```




