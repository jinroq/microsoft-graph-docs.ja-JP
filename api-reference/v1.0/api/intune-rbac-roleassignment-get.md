---
title: Get roleAssignment
description: roleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e5baecf4daaf354c5c6d8a05eef9a6345260f4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023707"
---
# <a name="get-roleassignment"></a><span data-ttu-id="bde40-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="bde40-103">Get roleAssignment</span></span>

> <span data-ttu-id="bde40-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bde40-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bde40-105">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bde40-105">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bde40-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bde40-106">Prerequisites</span></span>
<span data-ttu-id="bde40-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bde40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bde40-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bde40-109">Permission type</span></span>|<span data-ttu-id="bde40-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bde40-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bde40-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bde40-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bde40-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bde40-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="bde40-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bde40-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bde40-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde40-114">Not supported.</span></span>|
|<span data-ttu-id="bde40-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bde40-115">Application</span></span>|<span data-ttu-id="bde40-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde40-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bde40-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bde40-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bde40-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bde40-118">Optional query parameters</span></span>
<span data-ttu-id="bde40-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bde40-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bde40-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bde40-120">Request headers</span></span>
|<span data-ttu-id="bde40-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bde40-121">Header</span></span>|<span data-ttu-id="bde40-122">値</span><span class="sxs-lookup"><span data-stu-id="bde40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bde40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bde40-123">Authorization</span></span>|<span data-ttu-id="bde40-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bde40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bde40-125">承諾</span><span class="sxs-lookup"><span data-stu-id="bde40-125">Accept</span></span>|<span data-ttu-id="bde40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bde40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bde40-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bde40-127">Request body</span></span>
<span data-ttu-id="bde40-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bde40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bde40-129">応答</span><span class="sxs-lookup"><span data-stu-id="bde40-129">Response</span></span>
<span data-ttu-id="bde40-130">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bde40-130">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bde40-131">例</span><span class="sxs-lookup"><span data-stu-id="bde40-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bde40-132">要求</span><span class="sxs-lookup"><span data-stu-id="bde40-132">Request</span></span>
<span data-ttu-id="bde40-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bde40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bde40-134">応答</span><span class="sxs-lookup"><span data-stu-id="bde40-134">Response</span></span>
<span data-ttu-id="bde40-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bde40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```



