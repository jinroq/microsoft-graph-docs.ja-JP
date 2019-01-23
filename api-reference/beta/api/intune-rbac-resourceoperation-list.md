---
title: resourceOperations のリスト
description: resourceOperation オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c263445c4083b70bf6d9ea11950c9d756f4fae1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396680"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="63c46-103">resourceOperations のリスト</span><span class="sxs-lookup"><span data-stu-id="63c46-103">List resourceOperations</span></span>

> <span data-ttu-id="63c46-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63c46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63c46-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63c46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63c46-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63c46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63c46-107">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="63c46-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63c46-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="63c46-108">Prerequisites</span></span>
<span data-ttu-id="63c46-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63c46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63c46-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63c46-111">Permission type</span></span>|<span data-ttu-id="63c46-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="63c46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63c46-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63c46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63c46-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="63c46-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="63c46-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63c46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63c46-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63c46-116">Not supported.</span></span>|
|<span data-ttu-id="63c46-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63c46-117">Application</span></span>|<span data-ttu-id="63c46-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63c46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63c46-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63c46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="63c46-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63c46-120">Request headers</span></span>
|<span data-ttu-id="63c46-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63c46-121">Header</span></span>|<span data-ttu-id="63c46-122">値</span><span class="sxs-lookup"><span data-stu-id="63c46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63c46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63c46-123">Authorization</span></span>|<span data-ttu-id="63c46-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="63c46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63c46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63c46-125">Accept</span></span>|<span data-ttu-id="63c46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63c46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63c46-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="63c46-127">Request body</span></span>
<span data-ttu-id="63c46-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="63c46-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63c46-129">応答</span><span class="sxs-lookup"><span data-stu-id="63c46-129">Response</span></span>
<span data-ttu-id="63c46-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="63c46-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63c46-131">例</span><span class="sxs-lookup"><span data-stu-id="63c46-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63c46-132">要求</span><span class="sxs-lookup"><span data-stu-id="63c46-132">Request</span></span>
<span data-ttu-id="63c46-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="63c46-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="63c46-134">応答</span><span class="sxs-lookup"><span data-stu-id="63c46-134">Response</span></span>
<span data-ttu-id="63c46-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63c46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```




