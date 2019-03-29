---
title: resourceOperations のリスト
description: resourceOperation オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2aadaa4a1355e5088721ec428d393d9bec617c39
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980258"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="95f6c-103">resourceOperations のリスト</span><span class="sxs-lookup"><span data-stu-id="95f6c-103">List resourceOperations</span></span>

> <span data-ttu-id="95f6c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95f6c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f6c-105">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="95f6c-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95f6c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="95f6c-106">Prerequisites</span></span>
<span data-ttu-id="95f6c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95f6c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95f6c-109">Permission type</span></span>|<span data-ttu-id="95f6c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95f6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95f6c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95f6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95f6c-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f6c-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="95f6c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95f6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95f6c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95f6c-114">Not supported.</span></span>|
|<span data-ttu-id="95f6c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95f6c-115">Application</span></span>|<span data-ttu-id="95f6c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95f6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95f6c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95f6c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="95f6c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95f6c-118">Request headers</span></span>
|<span data-ttu-id="95f6c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95f6c-119">Header</span></span>|<span data-ttu-id="95f6c-120">値</span><span class="sxs-lookup"><span data-stu-id="95f6c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95f6c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95f6c-121">Authorization</span></span>|<span data-ttu-id="95f6c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95f6c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95f6c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="95f6c-123">Accept</span></span>|<span data-ttu-id="95f6c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="95f6c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f6c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="95f6c-125">Request body</span></span>
<span data-ttu-id="95f6c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95f6c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95f6c-127">応答</span><span class="sxs-lookup"><span data-stu-id="95f6c-127">Response</span></span>
<span data-ttu-id="95f6c-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="95f6c-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f6c-129">例</span><span class="sxs-lookup"><span data-stu-id="95f6c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="95f6c-130">要求</span><span class="sxs-lookup"><span data-stu-id="95f6c-130">Request</span></span>
<span data-ttu-id="95f6c-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95f6c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="95f6c-132">応答</span><span class="sxs-lookup"><span data-stu-id="95f6c-132">Response</span></span>
<span data-ttu-id="95f6c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95f6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value"
    }
  ]
}
```



