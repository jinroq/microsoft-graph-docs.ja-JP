---
title: リスト governanceResources
description: リクエスターは、アクセス権を持つ governanceResource のコレクションを取得します。
ms.openlocfilehash: a8f0fc03dbd880c82bca7c9d8f6e84a2940511d9
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191089"
---
# <a name="list-governanceresources"></a><span data-ttu-id="50253-103">リスト governanceResources</span><span class="sxs-lookup"><span data-stu-id="50253-103">List governanceResources</span></span>

> <span data-ttu-id="50253-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50253-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50253-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50253-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50253-106">リクエスターは、アクセス権を持つ[governanceResource](../resources/governanceresource.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="50253-106">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="50253-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50253-107">Permissions</span></span>
<span data-ttu-id="50253-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50253-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50253-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50253-110">Permission type</span></span>      | <span data-ttu-id="50253-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="50253-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50253-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50253-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50253-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="50253-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="50253-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50253-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50253-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50253-115">Not supported.</span></span>    |
|<span data-ttu-id="50253-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50253-116">Application</span></span> | <span data-ttu-id="50253-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="50253-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="50253-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50253-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50253-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="50253-119">Optional query parameters</span></span>
<span data-ttu-id="50253-120">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="50253-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50253-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50253-121">Request headers</span></span>
| <span data-ttu-id="50253-122">名前</span><span class="sxs-lookup"><span data-stu-id="50253-122">Name</span></span>      |<span data-ttu-id="50253-123">説明</span><span class="sxs-lookup"><span data-stu-id="50253-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50253-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50253-124">Authorization</span></span>  | <span data-ttu-id="50253-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="50253-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="50253-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50253-126">Request body</span></span>
<span data-ttu-id="50253-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="50253-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="50253-128">応答</span><span class="sxs-lookup"><span data-stu-id="50253-128">Response</span></span>
<span data-ttu-id="50253-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[governanceResource](../resources/governanceresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="50253-129">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="50253-130">例</span><span class="sxs-lookup"><span data-stu-id="50253-130">Examples</span></span>

<span data-ttu-id="50253-131">この例では、現在アクセスできるすべてのリソースが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="50253-131">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="50253-132">要求</span><span class="sxs-lookup"><span data-stu-id="50253-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="50253-133">応答</span><span class="sxs-lookup"><span data-stu-id="50253-133">Response</span></span>
<span data-ttu-id="50253-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="50253-134">Here is an example of the response.</span></span> 

><span data-ttu-id="50253-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50253-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
