---
title: リスト governanceResources
description: 要求者がアクセスできる governanceResource のコレクションを取得します。
localization_priority: Normal
ms.openlocfilehash: 702ab0ae1d47913584a7d3f6e86c939d871d6865
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859154"
---
# <a name="list-governanceresources"></a><span data-ttu-id="8cc9c-103">リスト governanceResources</span><span class="sxs-lookup"><span data-stu-id="8cc9c-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc9c-104">要求者がアクセスできる[governanceResource](../resources/governanceresource.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc9c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cc9c-105">Permissions</span></span>
<span data-ttu-id="8cc9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc9c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cc9c-108">Permission type</span></span>      | <span data-ttu-id="8cc9c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cc9c-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc9c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc9c-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="8cc9c-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8cc9c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc9c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-113">Not supported.</span></span>    |
|<span data-ttu-id="8cc9c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cc9c-114">Application</span></span> | <span data-ttu-id="8cc9c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc9c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cc9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cc9c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8cc9c-117">Optional query parameters</span></span>
<span data-ttu-id="8cc9c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cc9c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cc9c-119">Request headers</span></span>
| <span data-ttu-id="8cc9c-120">名前</span><span class="sxs-lookup"><span data-stu-id="8cc9c-120">Name</span></span>      |<span data-ttu-id="8cc9c-121">説明</span><span class="sxs-lookup"><span data-stu-id="8cc9c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cc9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc9c-122">Authorization</span></span>  | <span data-ttu-id="8cc9c-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8cc9c-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc9c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cc9c-124">Request body</span></span>
<span data-ttu-id="8cc9c-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8cc9c-126">応答</span><span class="sxs-lookup"><span data-stu-id="8cc9c-126">Response</span></span>
<span data-ttu-id="8cc9c-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceResource](../resources/governanceresource.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="8cc9c-128">例</span><span class="sxs-lookup"><span data-stu-id="8cc9c-128">Examples</span></span>

<span data-ttu-id="8cc9c-129">この例では、現在アクセスできるすべてのリソースを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="8cc9c-130">要求</span><span class="sxs-lookup"><span data-stu-id="8cc9c-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8cc9c-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8cc9c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cc9c-132">C#</span><span class="sxs-lookup"><span data-stu-id="8cc9c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cc9c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cc9c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cc9c-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="8cc9c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8cc9c-135">Java</span><span class="sxs-lookup"><span data-stu-id="8cc9c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governanceresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8cc9c-136">応答</span><span class="sxs-lookup"><span data-stu-id="8cc9c-136">Response</span></span>
<span data-ttu-id="8cc9c-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-137">Here is an example of the response.</span></span> 

><span data-ttu-id="8cc9c-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1289

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources",
    "value":[
        {
            "id": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/AnujRG/providers/Microsoft.Storage/storageAccounts/anujstoragefimdev",
            "type": "Microsoft.Storage/storageAccounts",
            "displayName": "anujstoragefimdev",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
