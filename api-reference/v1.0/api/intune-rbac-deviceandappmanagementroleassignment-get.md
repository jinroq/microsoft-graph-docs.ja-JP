---
title: deviceAndAppManagementRoleAssignment の取得
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7e45c10cb612edc9731b0ed197728956c96717bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866900"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="0cbcc-103">deviceAndAppManagementRoleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="0cbcc-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="0cbcc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cbcc-105">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cbcc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0cbcc-106">Prerequisites</span></span>
<span data-ttu-id="0cbcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cbcc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cbcc-109">Permission type</span></span>|<span data-ttu-id="0cbcc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cbcc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cbcc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cbcc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0cbcc-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cbcc-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0cbcc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cbcc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cbcc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-114">Not supported.</span></span>|
|<span data-ttu-id="0cbcc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cbcc-115">Application</span></span>|<span data-ttu-id="0cbcc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cbcc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cbcc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cbcc-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0cbcc-118">Optional query parameters</span></span>
<span data-ttu-id="0cbcc-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0cbcc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cbcc-120">Request headers</span></span>
|<span data-ttu-id="0cbcc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cbcc-121">Header</span></span>|<span data-ttu-id="0cbcc-122">値</span><span class="sxs-lookup"><span data-stu-id="0cbcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cbcc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cbcc-123">Authorization</span></span>|<span data-ttu-id="0cbcc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cbcc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cbcc-125">Accept</span></span>|<span data-ttu-id="0cbcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cbcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cbcc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cbcc-127">Request body</span></span>
<span data-ttu-id="0cbcc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cbcc-129">応答</span><span class="sxs-lookup"><span data-stu-id="0cbcc-129">Response</span></span>
<span data-ttu-id="0cbcc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cbcc-131">例</span><span class="sxs-lookup"><span data-stu-id="0cbcc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cbcc-132">要求</span><span class="sxs-lookup"><span data-stu-id="0cbcc-132">Request</span></span>
<span data-ttu-id="0cbcc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0cbcc-134">応答</span><span class="sxs-lookup"><span data-stu-id="0cbcc-134">Response</span></span>
<span data-ttu-id="0cbcc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cbcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```



