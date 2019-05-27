---
title: GovernanceRoleAssignment を取得する
description: GovernanceRoleAssignment のプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: e2e116baad573c8b99ab278771d1149ea3563209
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422424"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="3e371-103">GovernanceRoleAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="3e371-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e371-104">[GovernanceRoleAssignment](../resources/governanceroleassignment.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3e371-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e371-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e371-105">Permissions</span></span>
<span data-ttu-id="3e371-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e371-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e371-108">Permission type</span></span>      | <span data-ttu-id="3e371-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e371-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e371-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e371-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e371-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="3e371-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3e371-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e371-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e371-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e371-113">Not supported.</span></span>    |
|<span data-ttu-id="3e371-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e371-114">Application</span></span> | <span data-ttu-id="3e371-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e371-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e371-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e371-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="3e371-117">リソースで[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得する</span><span class="sxs-lookup"><span data-stu-id="3e371-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="3e371-118">*注: アクセス許可スコープの他に、要求者がリソースに対して少なくとも1つの役割の割り当てを持っている必要があります。*</span><span class="sxs-lookup"><span data-stu-id="3e371-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="3e371-119">自分の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得する</span><span class="sxs-lookup"><span data-stu-id="3e371-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e371-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e371-120">Optional query parameters</span></span>
<span data-ttu-id="3e371-121">このメソッドは、応答をカスタマイズ`$filter`するのではなく、 [OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="3e371-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e371-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e371-122">Request headers</span></span>
| <span data-ttu-id="3e371-123">名前</span><span class="sxs-lookup"><span data-stu-id="3e371-123">Name</span></span>      |<span data-ttu-id="3e371-124">説明</span><span class="sxs-lookup"><span data-stu-id="3e371-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e371-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e371-125">Authorization</span></span>  | <span data-ttu-id="3e371-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3e371-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e371-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e371-127">Request body</span></span>
<span data-ttu-id="3e371-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3e371-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3e371-129">応答</span><span class="sxs-lookup"><span data-stu-id="3e371-129">Response</span></span>
<span data-ttu-id="3e371-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleAssignment](../resources/governanceroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e371-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e371-131">例</span><span class="sxs-lookup"><span data-stu-id="3e371-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="3e371-132">サブスクリプション "Wingtip Toys- [governanceRoleAssignment](../resources/governanceroleassignment.md) " を取得します。</span><span class="sxs-lookup"><span data-stu-id="3e371-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="3e371-133">要求</span><span class="sxs-lookup"><span data-stu-id="3e371-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="3e371-134">応答</span><span class="sxs-lookup"><span data-stu-id="3e371-134">Response</span></span>
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
  "suppressions": []
}
-->
