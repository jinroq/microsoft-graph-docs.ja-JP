---
title: governanceRoleAssignmentRequest を取得する
description: 'governanceRoleAssignmentRequest を取得します。 '
localization_priority: Normal
ms.openlocfilehash: 6914dbe8c45bcc05bc684b08fb5fdf87405a045a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503703"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="d767a-103">governanceRoleAssignmentRequest を取得する</span><span class="sxs-lookup"><span data-stu-id="d767a-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d767a-104">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="d767a-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d767a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d767a-105">Permissions</span></span>
<span data-ttu-id="d767a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d767a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d767a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d767a-108">Permission type</span></span>      | <span data-ttu-id="d767a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d767a-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d767a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d767a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d767a-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="d767a-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d767a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d767a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d767a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d767a-113">Not supported.</span></span>    |
|<span data-ttu-id="d767a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d767a-114">Application</span></span> | <span data-ttu-id="d767a-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="d767a-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="d767a-116">アクセス許可スコープの他に、要求者が必要です。</span><span class="sxs-lookup"><span data-stu-id="d767a-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="d767a-117">リソースに対して少なくとも1つの役割の割り当てを行う。や</span><span class="sxs-lookup"><span data-stu-id="d767a-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="d767a-118">は、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の件名です。</span><span class="sxs-lookup"><span data-stu-id="d767a-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="d767a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d767a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d767a-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d767a-120">Optional query parameters</span></span>
<span data-ttu-id="d767a-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d767a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d767a-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d767a-122">Request headers</span></span>
| <span data-ttu-id="d767a-123">名前</span><span class="sxs-lookup"><span data-stu-id="d767a-123">Name</span></span>      |<span data-ttu-id="d767a-124">説明</span><span class="sxs-lookup"><span data-stu-id="d767a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d767a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d767a-125">Authorization</span></span>  | <span data-ttu-id="d767a-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d767a-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d767a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d767a-127">Request body</span></span>
<span data-ttu-id="d767a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d767a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d767a-129">応答</span><span class="sxs-lookup"><span data-stu-id="d767a-129">Response</span></span>
<span data-ttu-id="d767a-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d767a-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d767a-131">例</span><span class="sxs-lookup"><span data-stu-id="d767a-131">Example</span></span>
<span data-ttu-id="d767a-132">役割の割り当て要求を取得する</span><span class="sxs-lookup"><span data-stu-id="d767a-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="d767a-133">要求</span><span class="sxs-lookup"><span data-stu-id="d767a-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="d767a-134">応答</span><span class="sxs-lookup"><span data-stu-id="d767a-134">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
