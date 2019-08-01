---
title: resourceOperation の取得
description: resourceOperation オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c29d7894a1aabad08321c1c89dd2e7a393234bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023777"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="0d973-103">resourceOperation の取得</span><span class="sxs-lookup"><span data-stu-id="0d973-103">Get resourceOperation</span></span>

> <span data-ttu-id="0d973-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d973-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d973-105">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0d973-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d973-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d973-106">Prerequisites</span></span>
<span data-ttu-id="0d973-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d973-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d973-109">Permission type</span></span>|<span data-ttu-id="0d973-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d973-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d973-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d973-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d973-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d973-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0d973-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d973-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d973-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d973-114">Not supported.</span></span>|
|<span data-ttu-id="0d973-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d973-115">Application</span></span>|<span data-ttu-id="0d973-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d973-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d973-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d973-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d973-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0d973-118">Optional query parameters</span></span>
<span data-ttu-id="0d973-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0d973-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d973-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d973-120">Request headers</span></span>
|<span data-ttu-id="0d973-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d973-121">Header</span></span>|<span data-ttu-id="0d973-122">値</span><span class="sxs-lookup"><span data-stu-id="0d973-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d973-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d973-123">Authorization</span></span>|<span data-ttu-id="0d973-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d973-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d973-125">承諾</span><span class="sxs-lookup"><span data-stu-id="0d973-125">Accept</span></span>|<span data-ttu-id="0d973-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d973-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d973-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d973-127">Request body</span></span>
<span data-ttu-id="0d973-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0d973-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d973-129">応答</span><span class="sxs-lookup"><span data-stu-id="0d973-129">Response</span></span>
<span data-ttu-id="0d973-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d973-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d973-131">例</span><span class="sxs-lookup"><span data-stu-id="0d973-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d973-132">要求</span><span class="sxs-lookup"><span data-stu-id="0d973-132">Request</span></span>
<span data-ttu-id="0d973-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d973-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="0d973-134">応答</span><span class="sxs-lookup"><span data-stu-id="0d973-134">Response</span></span>
<span data-ttu-id="0d973-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d973-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value"
  }
}
```



