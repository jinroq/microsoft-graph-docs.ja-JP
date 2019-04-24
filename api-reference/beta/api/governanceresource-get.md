---
title: governanceResource を取得する
description: governanceResource オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: be24fb8822101f7a67a5bd60f1fe018cf1a08f6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463930"
---
# <a name="get-governanceresource"></a><span data-ttu-id="afa39-103">governanceResource を取得する</span><span class="sxs-lookup"><span data-stu-id="afa39-103">Get governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afa39-104">[governanceResource](../resources/governanceresource.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="afa39-104">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afa39-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afa39-105">Permissions</span></span>
<span data-ttu-id="afa39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afa39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa39-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afa39-108">Permission type</span></span>      | <span data-ttu-id="afa39-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afa39-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afa39-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afa39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afa39-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="afa39-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="afa39-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afa39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afa39-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa39-113">Not supported.</span></span>    |
|<span data-ttu-id="afa39-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afa39-114">Application</span></span> | <span data-ttu-id="afa39-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="afa39-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="afa39-116">この API は、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afa39-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="afa39-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afa39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afa39-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="afa39-118">Optional query parameters</span></span>
<span data-ttu-id="afa39-119">このメソッド**は**、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="afa39-119">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afa39-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afa39-120">Request headers</span></span>
| <span data-ttu-id="afa39-121">名前</span><span class="sxs-lookup"><span data-stu-id="afa39-121">Name</span></span>      |<span data-ttu-id="afa39-122">説明</span><span class="sxs-lookup"><span data-stu-id="afa39-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afa39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afa39-123">Authorization</span></span>  | <span data-ttu-id="afa39-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="afa39-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="afa39-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="afa39-125">Request body</span></span>
<span data-ttu-id="afa39-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="afa39-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="afa39-127">応答</span><span class="sxs-lookup"><span data-stu-id="afa39-127">Response</span></span>
<span data-ttu-id="afa39-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceResource](../resources/governanceresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="afa39-128">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afa39-129">例</span><span class="sxs-lookup"><span data-stu-id="afa39-129">Example</span></span>
<span data-ttu-id="afa39-130">この例では、サブスクリプションの Wingtip Toys-生産 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) の詳細を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="afa39-130">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="afa39-131">要求</span><span class="sxs-lookup"><span data-stu-id="afa39-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="afa39-132">応答</span><span class="sxs-lookup"><span data-stu-id="afa39-132">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
