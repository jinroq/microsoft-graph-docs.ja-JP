---
title: リスト governanceRoleDefinitions
description: リソース上の governanceRoleDefinitions のコレクションを取得します。
localization_priority: Normal
ms.openlocfilehash: 0e03a75446723743cc43eef63c42dd0f39c86126
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503066"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="3fdb0-103">リスト governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3fdb0-103">List governanceRoleDefinitions</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fdb0-104">リソース上の[governanceRoleDefinitions](../resources/governanceroledefinition.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-104">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fdb0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3fdb0-105">Permissions</span></span>
<span data-ttu-id="3fdb0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fdb0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fdb0-108">Permission type</span></span>      | <span data-ttu-id="3fdb0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3fdb0-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fdb0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fdb0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3fdb0-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="3fdb0-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3fdb0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fdb0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fdb0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-113">Not supported.</span></span>    |
|<span data-ttu-id="3fdb0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fdb0-114">Application</span></span> | <span data-ttu-id="3fdb0-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="3fdb0-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="3fdb0-116">この API は、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="3fdb0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fdb0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3fdb0-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3fdb0-118">Optional query parameters</span></span>
<span data-ttu-id="3fdb0-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fdb0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fdb0-120">Request headers</span></span>
| <span data-ttu-id="3fdb0-121">名前</span><span class="sxs-lookup"><span data-stu-id="3fdb0-121">Name</span></span>      |<span data-ttu-id="3fdb0-122">説明</span><span class="sxs-lookup"><span data-stu-id="3fdb0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fdb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fdb0-123">Authorization</span></span>  | <span data-ttu-id="3fdb0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3fdb0-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fdb0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fdb0-125">Request body</span></span>
<span data-ttu-id="3fdb0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3fdb0-127">応答</span><span class="sxs-lookup"><span data-stu-id="3fdb0-127">Response</span></span>
<span data-ttu-id="3fdb0-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleDefinition](../resources/governanceroledefinition.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fdb0-129">例</span><span class="sxs-lookup"><span data-stu-id="3fdb0-129">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="3fdb0-130">この例では、Wingtip Toys のサブスクリプションのすべてのロール定義を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3fdb0-130">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="3fdb0-131">要求</span><span class="sxs-lookup"><span data-stu-id="3fdb0-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="3fdb0-132">応答</span><span class="sxs-lookup"><span data-stu-id="3fdb0-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
