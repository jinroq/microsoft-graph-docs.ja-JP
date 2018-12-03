---
title: GovernanceRoleDefinition を取得します。
description: プロパティと、governanceRoleDefinition の関係を取得します。
ms.openlocfilehash: da6f81c57d8070a977482a81f8f2211b85ab0f97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073084"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="0061d-103">GovernanceRoleDefinition を取得します。</span><span class="sxs-lookup"><span data-stu-id="0061d-103">Get governanceRoleDefinition</span></span>

> <span data-ttu-id="0061d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0061d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0061d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0061d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0061d-106">プロパティと、 [governanceRoleDefinition](../resources/governanceroledefinition.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="0061d-106">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0061d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0061d-107">Permissions</span></span>
<span data-ttu-id="0061d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0061d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0061d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0061d-110">Permission type</span></span>      | <span data-ttu-id="0061d-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="0061d-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0061d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0061d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0061d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0061d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0061d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0061d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0061d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0061d-115">Not supported.</span></span>    |
|<span data-ttu-id="0061d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0061d-116">Application</span></span> | <span data-ttu-id="0061d-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0061d-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="0061d-118">以外にも、アクセス許可のスコープは、この API には、 [governanceRoleDefinition](../resources/governanceroledefinition.md)が属するリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="0061d-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="0061d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0061d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0061d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0061d-120">Optional query parameters</span></span>
<span data-ttu-id="0061d-121">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポート**しません**。</span><span class="sxs-lookup"><span data-stu-id="0061d-121">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0061d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0061d-122">Request headers</span></span>
| <span data-ttu-id="0061d-123">名前</span><span class="sxs-lookup"><span data-stu-id="0061d-123">Name</span></span>      |<span data-ttu-id="0061d-124">説明</span><span class="sxs-lookup"><span data-stu-id="0061d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0061d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0061d-125">Authorization</span></span>  | <span data-ttu-id="0061d-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0061d-126">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="0061d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0061d-127">Request body</span></span>
<span data-ttu-id="0061d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0061d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0061d-129">応答</span><span class="sxs-lookup"><span data-stu-id="0061d-129">Response</span></span>
<span data-ttu-id="0061d-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceRoleDefinition](../resources/governanceroledefinition.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0061d-130">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0061d-131">例</span><span class="sxs-lookup"><span data-stu-id="0061d-131">Example</span></span>
<span data-ttu-id="0061d-132">次の使用例は、サブスクリプション Wingtip Toys の本番環境で DNS ゾーンの共同作成者の役割定義の詳細を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="0061d-132">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="0061d-133">要求</span><span class="sxs-lookup"><span data-stu-id="0061d-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="0061d-134">応答</span><span class="sxs-lookup"><span data-stu-id="0061d-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
