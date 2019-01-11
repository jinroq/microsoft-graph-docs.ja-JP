---
title: GovernanceResource を取得します。
description: プロパティと、governanceResource オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 16442ea971a635aedfd89f09c48ffddf14c83b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888033"
---
# <a name="get-governanceresource"></a><span data-ttu-id="54172-103">GovernanceResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="54172-103">Get governanceResource</span></span>

> <span data-ttu-id="54172-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54172-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54172-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54172-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54172-106">プロパティと、 [governanceResource](../resources/governanceresource.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="54172-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54172-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54172-107">Permissions</span></span>
<span data-ttu-id="54172-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54172-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54172-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54172-110">Permission type</span></span>      | <span data-ttu-id="54172-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="54172-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54172-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54172-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54172-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="54172-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="54172-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54172-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54172-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54172-115">Not supported.</span></span>    |
|<span data-ttu-id="54172-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54172-116">Application</span></span> | <span data-ttu-id="54172-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="54172-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="54172-118">以外にも、アクセス許可のスコープは、この API にはリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="54172-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="54172-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54172-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54172-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="54172-120">Optional query parameters</span></span>
<span data-ttu-id="54172-121">このメソッド**のみ**をサポートしている`$select`と`$expand`の応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="54172-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54172-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54172-122">Request headers</span></span>
| <span data-ttu-id="54172-123">名前</span><span class="sxs-lookup"><span data-stu-id="54172-123">Name</span></span>      |<span data-ttu-id="54172-124">説明</span><span class="sxs-lookup"><span data-stu-id="54172-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54172-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="54172-125">Authorization</span></span>  | <span data-ttu-id="54172-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="54172-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="54172-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="54172-127">Request body</span></span>
<span data-ttu-id="54172-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54172-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="54172-129">応答</span><span class="sxs-lookup"><span data-stu-id="54172-129">Response</span></span>
<span data-ttu-id="54172-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceResource](../resources/governanceresource.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="54172-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54172-131">例</span><span class="sxs-lookup"><span data-stu-id="54172-131">Example</span></span>
<span data-ttu-id="54172-132">次の使用例は、Wingtip toys 社の商品 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) のサブスクリプションの詳細を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="54172-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="54172-133">要求</span><span class="sxs-lookup"><span data-stu-id="54172-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="54172-134">応答</span><span class="sxs-lookup"><span data-stu-id="54172-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
