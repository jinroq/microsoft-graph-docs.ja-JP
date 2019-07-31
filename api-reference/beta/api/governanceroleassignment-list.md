---
title: リスト governanceRoleAssignments
description: GovernanceRoleAssignments のコレクションを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: bd635d2abe405a1e09b6c672cfd4ecb2145ff793
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954201"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="1db9e-103">リスト governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="1db9e-103">List governanceRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1db9e-104">[GovernanceRoleAssignments](../resources/governanceroleassignment.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1db9e-104">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1db9e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1db9e-105">Permissions</span></span>
<span data-ttu-id="1db9e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1db9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1db9e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1db9e-108">Permission type</span></span>      | <span data-ttu-id="1db9e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1db9e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1db9e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1db9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1db9e-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="1db9e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="1db9e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1db9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db9e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1db9e-113">Not supported.</span></span>    |
|<span data-ttu-id="1db9e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1db9e-114">Application</span></span> | <span data-ttu-id="1db9e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1db9e-115">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1db9e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1db9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="1db9e-117">リソース上の[governanceRoleAssignments](../resources/governanceroleassignment.md)のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1db9e-117">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="1db9e-118">**注:** この要求では、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てが必要になります。</span><span class="sxs-lookup"><span data-stu-id="1db9e-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="1db9e-119">採鉱所の[governanceRoleAssignments](../resources/governanceroleassignment.md)のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1db9e-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1db9e-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1db9e-120">Optional query parameters</span></span>
<span data-ttu-id="1db9e-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1db9e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1db9e-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1db9e-122">Request headers</span></span>
| <span data-ttu-id="1db9e-123">名前</span><span class="sxs-lookup"><span data-stu-id="1db9e-123">Name</span></span>      |<span data-ttu-id="1db9e-124">説明</span><span class="sxs-lookup"><span data-stu-id="1db9e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1db9e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1db9e-125">Authorization</span></span>  | <span data-ttu-id="1db9e-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1db9e-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1db9e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1db9e-127">Request body</span></span>
<span data-ttu-id="1db9e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1db9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1db9e-129">応答</span><span class="sxs-lookup"><span data-stu-id="1db9e-129">Response</span></span>
<span data-ttu-id="1db9e-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleAssignment](../resources/governanceroleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1db9e-130">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1db9e-131">例</span><span class="sxs-lookup"><span data-stu-id="1db9e-131">Example</span></span>

<span data-ttu-id="1db9e-132">この例では、Wingtip Toys のサブスクリプションで役割の割り当てを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1db9e-132">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="1db9e-133">要求</span><span class="sxs-lookup"><span data-stu-id="1db9e-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="1db9e-134">応答</span><span class="sxs-lookup"><span data-stu-id="1db9e-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
