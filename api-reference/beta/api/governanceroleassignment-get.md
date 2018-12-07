---
title: GovernanceRoleAssignment を取得します。
description: プロパティと、governanceRoleAssignment の関係を取得します。
ms.openlocfilehash: 622fb890422ed0a4cf00542fede5ebaf662e5e71
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191075"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="ff426-103">GovernanceRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff426-103">Get governanceRoleAssignment</span></span>

> <span data-ttu-id="ff426-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff426-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff426-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff426-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff426-106">プロパティと、 [governanceRoleAssignment](../resources/governanceroleassignment.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff426-106">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff426-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff426-107">Permissions</span></span>
<span data-ttu-id="ff426-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff426-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff426-110">Permission type</span></span>      | <span data-ttu-id="ff426-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="ff426-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff426-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff426-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff426-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ff426-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ff426-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff426-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff426-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff426-115">Not supported.</span></span>    |
|<span data-ttu-id="ff426-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff426-116">Application</span></span> | <span data-ttu-id="ff426-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ff426-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff426-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff426-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="ff426-119">リソース上の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff426-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="ff426-120">*注: だけでなく、アクセス許可のスコープが必要ですが少なくとも 1 つのロールの割り当てがあるリソースにするには、リクエスター。*</span><span class="sxs-lookup"><span data-stu-id="ff426-120">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="ff426-121">私の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff426-121">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff426-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff426-122">Optional query parameters</span></span>
<span data-ttu-id="ff426-123">このメソッド**以外の[OData クエリ パラメーター](/graph/query-parameters)をサポートして**`$filter`の応答をカスタマイズするためです。</span><span class="sxs-lookup"><span data-stu-id="ff426-123">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff426-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff426-124">Request headers</span></span>
| <span data-ttu-id="ff426-125">名前</span><span class="sxs-lookup"><span data-stu-id="ff426-125">Name</span></span>      |<span data-ttu-id="ff426-126">説明</span><span class="sxs-lookup"><span data-stu-id="ff426-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff426-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff426-127">Authorization</span></span>  | <span data-ttu-id="ff426-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff426-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff426-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff426-129">Request body</span></span>
<span data-ttu-id="ff426-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff426-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ff426-131">応答</span><span class="sxs-lookup"><span data-stu-id="ff426-131">Response</span></span>
<span data-ttu-id="ff426-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceRoleAssignment](../resources/governanceroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ff426-132">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff426-133">例</span><span class="sxs-lookup"><span data-stu-id="ff426-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="ff426-134">サブスクリプション「Wingtip Toys-商品」で、 [governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff426-134">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="ff426-135">要求</span><span class="sxs-lookup"><span data-stu-id="ff426-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="ff426-136">応答</span><span class="sxs-lookup"><span data-stu-id="ff426-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->