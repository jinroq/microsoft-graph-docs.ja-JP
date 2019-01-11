---
title: リスト governanceRoleDefinitions
description: リソースの governanceRoleDefinitions のコレクションを取得します。
localization_priority: Normal
ms.openlocfilehash: 6586a1fec0be4610aa18d204cb8049a012aa7a04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854748"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="f9fae-103">リスト governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f9fae-103">List governanceRoleDefinitions</span></span>
> <span data-ttu-id="f9fae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9fae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9fae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9fae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9fae-106">リソースの[governanceRoleDefinitions](../resources/governanceroledefinition.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9fae-106">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9fae-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9fae-107">Permissions</span></span>
<span data-ttu-id="f9fae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9fae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9fae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9fae-110">Permission type</span></span>      | <span data-ttu-id="f9fae-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9fae-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9fae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9fae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9fae-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f9fae-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f9fae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9fae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9fae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9fae-115">Not supported.</span></span>    |
|<span data-ttu-id="f9fae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9fae-116">Application</span></span> | <span data-ttu-id="f9fae-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f9fae-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="f9fae-118">以外にも、アクセス許可のスコープは、この API にはリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9fae-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="f9fae-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9fae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9fae-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9fae-120">Optional query parameters</span></span>
<span data-ttu-id="f9fae-121">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f9fae-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9fae-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9fae-122">Request headers</span></span>
| <span data-ttu-id="f9fae-123">名前</span><span class="sxs-lookup"><span data-stu-id="f9fae-123">Name</span></span>      |<span data-ttu-id="f9fae-124">説明</span><span class="sxs-lookup"><span data-stu-id="f9fae-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9fae-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9fae-125">Authorization</span></span>  | <span data-ttu-id="f9fae-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f9fae-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9fae-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9fae-127">Request body</span></span>
<span data-ttu-id="f9fae-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f9fae-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f9fae-129">応答</span><span class="sxs-lookup"><span data-stu-id="f9fae-129">Response</span></span>
<span data-ttu-id="f9fae-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[governanceRoleDefinition](../resources/governanceroledefinition.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f9fae-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9fae-131">例</span><span class="sxs-lookup"><span data-stu-id="f9fae-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="f9fae-132">次の使用例は、サブスクリプションの Wingtip toys 社の商品のすべてのロールの定義を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f9fae-132">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f9fae-133">要求</span><span class="sxs-lookup"><span data-stu-id="f9fae-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="f9fae-134">応答</span><span class="sxs-lookup"><span data-stu-id="f9fae-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
