---
title: GovernanceRoleAssignment を取得します。
description: プロパティと、governanceRoleAssignment の関係を取得します。
localization_priority: Normal
ms.openlocfilehash: f699e1b5332652b2b87f3972d2ae47b06894b2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508840"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="03d1e-103">GovernanceRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d1e-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03d1e-104">プロパティと、 [governanceRoleAssignment](../resources/governanceroleassignment.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d1e-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03d1e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03d1e-105">Permissions</span></span>
<span data-ttu-id="03d1e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03d1e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03d1e-108">Permission type</span></span>      | <span data-ttu-id="03d1e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03d1e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03d1e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03d1e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03d1e-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="03d1e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="03d1e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03d1e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03d1e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03d1e-113">Not supported.</span></span>    |
|<span data-ttu-id="03d1e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03d1e-114">Application</span></span> | <span data-ttu-id="03d1e-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="03d1e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="03d1e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03d1e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="03d1e-117">リソース上の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d1e-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="03d1e-118">*注: だけでなく、アクセス許可のスコープが必要ですが少なくとも 1 つのロールの割り当てがあるリソースにするには、リクエスター。*</span><span class="sxs-lookup"><span data-stu-id="03d1e-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="03d1e-119">私の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d1e-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03d1e-120">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="03d1e-120">Optional query parameters</span></span>
<span data-ttu-id="03d1e-121">このメソッド**以外の[OData クエリ パラメーター](/graph/query-parameters)をサポートして**`$filter`の応答をカスタマイズするためです。</span><span class="sxs-lookup"><span data-stu-id="03d1e-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03d1e-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03d1e-122">Request headers</span></span>
| <span data-ttu-id="03d1e-123">名前</span><span class="sxs-lookup"><span data-stu-id="03d1e-123">Name</span></span>      |<span data-ttu-id="03d1e-124">説明</span><span class="sxs-lookup"><span data-stu-id="03d1e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03d1e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="03d1e-125">Authorization</span></span>  | <span data-ttu-id="03d1e-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="03d1e-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="03d1e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="03d1e-127">Request body</span></span>
<span data-ttu-id="03d1e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="03d1e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="03d1e-129">応答</span><span class="sxs-lookup"><span data-stu-id="03d1e-129">Response</span></span>
<span data-ttu-id="03d1e-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceRoleAssignment](../resources/governanceroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="03d1e-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03d1e-131">例</span><span class="sxs-lookup"><span data-stu-id="03d1e-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="03d1e-132">サブスクリプション「Wingtip Toys-商品」で、 [governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="03d1e-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="03d1e-133">要求</span><span class="sxs-lookup"><span data-stu-id="03d1e-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="03d1e-134">応答</span><span class="sxs-lookup"><span data-stu-id="03d1e-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
