---
title: エクスポート governanceRoleAssignmentRequests
description: 形式の governanceRoleAssignmentRequests のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。
localization_priority: Normal
ms.openlocfilehash: 10fd7c720bf7b6f162a4d8c2189e81a9205e53ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828729"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="72c33-103">エクスポート governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="72c33-103">Export governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="72c33-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72c33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72c33-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72c33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72c33-106">形式の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。</span><span class="sxs-lookup"><span data-stu-id="72c33-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="72c33-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72c33-107">Permissions</span></span>
<span data-ttu-id="72c33-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72c33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c33-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72c33-110">Permission type</span></span>      | <span data-ttu-id="72c33-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="72c33-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72c33-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72c33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72c33-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72c33-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="72c33-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72c33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c33-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72c33-115">Not supported.</span></span>    |
|<span data-ttu-id="72c33-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72c33-116">Application</span></span> | <span data-ttu-id="72c33-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72c33-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="72c33-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72c33-118">HTTP request</span></span>
<span data-ttu-id="72c33-119"><!-- { "blockType": "ignored" } -->リソースの[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="72c33-119"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="72c33-120">**注:** だけでなく、アクセス許可のスコープは、この要求には、リソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="72c33-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="72c33-121">私の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="72c33-121">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72c33-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="72c33-122">Optional query parameters</span></span>
<span data-ttu-id="72c33-123">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="72c33-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72c33-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72c33-124">Request headers</span></span>
| <span data-ttu-id="72c33-125">名前</span><span class="sxs-lookup"><span data-stu-id="72c33-125">Name</span></span>      |<span data-ttu-id="72c33-126">説明</span><span class="sxs-lookup"><span data-stu-id="72c33-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72c33-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c33-127">Authorization</span></span>  | <span data-ttu-id="72c33-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="72c33-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="72c33-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="72c33-129">Request body</span></span>
<span data-ttu-id="72c33-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="72c33-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c33-131">応答</span><span class="sxs-lookup"><span data-stu-id="72c33-131">Response</span></span>
<span data-ttu-id="72c33-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードとコンテンツの種類の`application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="72c33-132">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="72c33-133">例</span><span class="sxs-lookup"><span data-stu-id="72c33-133">Example</span></span>
<span data-ttu-id="72c33-134">この例では、サブスクリプションの Wingtip toys 社の商品で .csv ファイルとしてすべてのロールの割り当てを保存します。</span><span class="sxs-lookup"><span data-stu-id="72c33-134">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="72c33-135">要求</span><span class="sxs-lookup"><span data-stu-id="72c33-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="72c33-136">応答</span><span class="sxs-lookup"><span data-stu-id="72c33-136">Response</span></span>
<span data-ttu-id="72c33-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="72c33-137">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
