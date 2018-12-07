---
title: GovernanceRoleAssignmentRequest を取得します。
description: 'GovernanceRoleAssignmentRequest を取得します。 '
ms.openlocfilehash: aac41bd8443d6066a7866462624a072db57b35da
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191096"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="49fc4-103">GovernanceRoleAssignmentRequest を取得します。</span><span class="sxs-lookup"><span data-stu-id="49fc4-103">Get governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="49fc4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49fc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49fc4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49fc4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49fc4-106">の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="49fc4-106">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="49fc4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49fc4-107">Permissions</span></span>
<span data-ttu-id="49fc4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49fc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49fc4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49fc4-110">Permission type</span></span>      | <span data-ttu-id="49fc4-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="49fc4-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49fc4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49fc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49fc4-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="49fc4-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="49fc4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49fc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49fc4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49fc4-115">Not supported.</span></span>    |
|<span data-ttu-id="49fc4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49fc4-116">Application</span></span> | <span data-ttu-id="49fc4-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="49fc4-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="49fc4-118">アクセス許可のスコープ以外にも、リクエスターが必要です。</span><span class="sxs-lookup"><span data-stu-id="49fc4-118">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="49fc4-119">リソースの 1 つ以上のロールの割り当てにまたは</span><span class="sxs-lookup"><span data-stu-id="49fc4-119">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="49fc4-120">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の件名です。</span><span class="sxs-lookup"><span data-stu-id="49fc4-120">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="49fc4-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49fc4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49fc4-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49fc4-122">Optional query parameters</span></span>
<span data-ttu-id="49fc4-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="49fc4-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49fc4-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49fc4-124">Request headers</span></span>
| <span data-ttu-id="49fc4-125">名前</span><span class="sxs-lookup"><span data-stu-id="49fc4-125">Name</span></span>      |<span data-ttu-id="49fc4-126">説明</span><span class="sxs-lookup"><span data-stu-id="49fc4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49fc4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="49fc4-127">Authorization</span></span>  | <span data-ttu-id="49fc4-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="49fc4-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="49fc4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="49fc4-129">Request body</span></span>
<span data-ttu-id="49fc4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="49fc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49fc4-131">応答</span><span class="sxs-lookup"><span data-stu-id="49fc4-131">Response</span></span>
<span data-ttu-id="49fc4-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="49fc4-132">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49fc4-133">例</span><span class="sxs-lookup"><span data-stu-id="49fc4-133">Example</span></span>
<span data-ttu-id="49fc4-134">役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="49fc4-134">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="49fc4-135">要求</span><span class="sxs-lookup"><span data-stu-id="49fc4-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="49fc4-136">応答</span><span class="sxs-lookup"><span data-stu-id="49fc4-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->