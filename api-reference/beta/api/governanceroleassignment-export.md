---
title: エクスポート governanceRoleAssignmentRequests
description: 形式の governanceRoleAssignmentRequests のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522428"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="0029a-103">エクスポート governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="0029a-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0029a-104">形式の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。</span><span class="sxs-lookup"><span data-stu-id="0029a-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="0029a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0029a-105">Permissions</span></span>
<span data-ttu-id="0029a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0029a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0029a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0029a-108">Permission type</span></span>      | <span data-ttu-id="0029a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0029a-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0029a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0029a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0029a-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0029a-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0029a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0029a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0029a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0029a-113">Not supported.</span></span>    |
|<span data-ttu-id="0029a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0029a-114">Application</span></span> | <span data-ttu-id="0029a-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0029a-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="0029a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0029a-116">HTTP request</span></span>
<span data-ttu-id="0029a-117"><!-- { "blockType": "ignored" } -->リソースの[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="0029a-117"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="0029a-118">**注:** だけでなく、アクセス許可のスコープは、この要求には、リソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="0029a-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="0029a-119">私の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="0029a-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0029a-120">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0029a-120">Optional query parameters</span></span>
<span data-ttu-id="0029a-121">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0029a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0029a-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0029a-122">Request headers</span></span>
| <span data-ttu-id="0029a-123">名前</span><span class="sxs-lookup"><span data-stu-id="0029a-123">Name</span></span>      |<span data-ttu-id="0029a-124">説明</span><span class="sxs-lookup"><span data-stu-id="0029a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0029a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0029a-125">Authorization</span></span>  | <span data-ttu-id="0029a-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0029a-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0029a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0029a-127">Request body</span></span>
<span data-ttu-id="0029a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0029a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0029a-129">応答</span><span class="sxs-lookup"><span data-stu-id="0029a-129">Response</span></span>
<span data-ttu-id="0029a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードとコンテンツの種類の`application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="0029a-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="0029a-131">例</span><span class="sxs-lookup"><span data-stu-id="0029a-131">Example</span></span>
<span data-ttu-id="0029a-132">この例では、サブスクリプションの Wingtip toys 社の商品で .csv ファイルとしてすべてのロールの割り当てを保存します。</span><span class="sxs-lookup"><span data-stu-id="0029a-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="0029a-133">要求</span><span class="sxs-lookup"><span data-stu-id="0029a-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="0029a-134">応答</span><span class="sxs-lookup"><span data-stu-id="0029a-134">Response</span></span>
<span data-ttu-id="0029a-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0029a-135">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-export.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
