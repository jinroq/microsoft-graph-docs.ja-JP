---
title: GovernanceRoleDefinition を取得します。
description: プロパティと、governanceRoleDefinition の関係を取得します。
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511927"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="13cd5-103">GovernanceRoleDefinition を取得します。</span><span class="sxs-lookup"><span data-stu-id="13cd5-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13cd5-104">プロパティと、 [governanceRoleDefinition](../resources/governanceroledefinition.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="13cd5-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13cd5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13cd5-105">Permissions</span></span>
<span data-ttu-id="13cd5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13cd5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13cd5-108">Permission type</span></span>      | <span data-ttu-id="13cd5-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13cd5-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13cd5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13cd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13cd5-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="13cd5-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="13cd5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13cd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13cd5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13cd5-113">Not supported.</span></span>    |
|<span data-ttu-id="13cd5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13cd5-114">Application</span></span> | <span data-ttu-id="13cd5-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="13cd5-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="13cd5-116">以外にも、アクセス許可のスコープは、この API には、 [governanceRoleDefinition](../resources/governanceroledefinition.md)が属するリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="13cd5-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="13cd5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13cd5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13cd5-118">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="13cd5-118">Optional query parameters</span></span>
<span data-ttu-id="13cd5-119">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポート**しません**。</span><span class="sxs-lookup"><span data-stu-id="13cd5-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13cd5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13cd5-120">Request headers</span></span>
| <span data-ttu-id="13cd5-121">名前</span><span class="sxs-lookup"><span data-stu-id="13cd5-121">Name</span></span>      |<span data-ttu-id="13cd5-122">説明</span><span class="sxs-lookup"><span data-stu-id="13cd5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13cd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13cd5-123">Authorization</span></span>  | <span data-ttu-id="13cd5-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="13cd5-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="13cd5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="13cd5-125">Request body</span></span>
<span data-ttu-id="13cd5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13cd5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13cd5-127">応答</span><span class="sxs-lookup"><span data-stu-id="13cd5-127">Response</span></span>
<span data-ttu-id="13cd5-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceRoleDefinition](../resources/governanceroledefinition.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="13cd5-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13cd5-129">例</span><span class="sxs-lookup"><span data-stu-id="13cd5-129">Example</span></span>
<span data-ttu-id="13cd5-130">次の使用例は、サブスクリプション Wingtip Toys の本番環境で DNS ゾーンの共同作成者の役割定義の詳細を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="13cd5-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="13cd5-131">要求</span><span class="sxs-lookup"><span data-stu-id="13cd5-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="13cd5-132">応答</span><span class="sxs-lookup"><span data-stu-id="13cd5-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
