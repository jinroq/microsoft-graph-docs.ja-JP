---
title: governanceRoleDefinition を取得する
description: governanceRoleDefinition のプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 58323718c72c34cd197fcc48e1782150f6e6b9b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329756"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="9ea88-103">governanceRoleDefinition を取得する</span><span class="sxs-lookup"><span data-stu-id="9ea88-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea88-104">[governanceRoleDefinition](../resources/governanceroledefinition.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9ea88-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea88-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ea88-105">Permissions</span></span>
<span data-ttu-id="9ea88-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ea88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea88-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ea88-108">Permission type</span></span>      | <span data-ttu-id="9ea88-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ea88-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ea88-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ea88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ea88-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="9ea88-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9ea88-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ea88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea88-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ea88-113">Not supported.</span></span>    |
|<span data-ttu-id="9ea88-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ea88-114">Application</span></span> | <span data-ttu-id="9ea88-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="9ea88-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="9ea88-116">この API は、アクセス許可のスコープに加えて、 [governanceRoleDefinition](../resources/governanceroledefinition.md)が属しているリソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ea88-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="9ea88-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ea88-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ea88-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9ea88-118">Optional query parameters</span></span>
<span data-ttu-id="9ea88-119">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="9ea88-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ea88-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ea88-120">Request headers</span></span>
| <span data-ttu-id="9ea88-121">名前</span><span class="sxs-lookup"><span data-stu-id="9ea88-121">Name</span></span>      |<span data-ttu-id="9ea88-122">説明</span><span class="sxs-lookup"><span data-stu-id="9ea88-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ea88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ea88-123">Authorization</span></span>  | <span data-ttu-id="9ea88-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9ea88-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="9ea88-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ea88-125">Request body</span></span>
<span data-ttu-id="9ea88-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9ea88-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9ea88-127">応答</span><span class="sxs-lookup"><span data-stu-id="9ea88-127">Response</span></span>
<span data-ttu-id="9ea88-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleDefinition](../resources/governanceroledefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ea88-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ea88-129">例</span><span class="sxs-lookup"><span data-stu-id="9ea88-129">Example</span></span>
<span data-ttu-id="9ea88-130">この例では、サブスクリプション Wingtip Toys-生産のロール定義 DNS ゾーン共同作成者の詳細を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="9ea88-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="9ea88-131">要求</span><span class="sxs-lookup"><span data-stu-id="9ea88-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="9ea88-132">応答</span><span class="sxs-lookup"><span data-stu-id="9ea88-132">Response</span></span>
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
  "suppressions": []
}
-->
