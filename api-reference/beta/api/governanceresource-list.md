---
title: リスト governanceResources
description: リクエスターは、アクセス権を持つ governanceResource のコレクションを取得します。
localization_priority: Normal
ms.openlocfilehash: 998e18a0139f0cbe41901da935faee2f7f24e9eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525669"
---
# <a name="list-governanceresources"></a><span data-ttu-id="546fc-103">リスト governanceResources</span><span class="sxs-lookup"><span data-stu-id="546fc-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="546fc-104">リクエスターは、アクセス権を持つ[governanceResource](../resources/governanceresource.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="546fc-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="546fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="546fc-105">Permissions</span></span>
<span data-ttu-id="546fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="546fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="546fc-108">Permission type</span></span>      | <span data-ttu-id="546fc-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="546fc-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="546fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="546fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="546fc-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="546fc-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="546fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="546fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="546fc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="546fc-113">Not supported.</span></span>    |
|<span data-ttu-id="546fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="546fc-114">Application</span></span> | <span data-ttu-id="546fc-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="546fc-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="546fc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="546fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="546fc-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="546fc-117">Optional query parameters</span></span>
<span data-ttu-id="546fc-118">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="546fc-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="546fc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="546fc-119">Request headers</span></span>
| <span data-ttu-id="546fc-120">名前</span><span class="sxs-lookup"><span data-stu-id="546fc-120">Name</span></span>      |<span data-ttu-id="546fc-121">説明</span><span class="sxs-lookup"><span data-stu-id="546fc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="546fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="546fc-122">Authorization</span></span>  | <span data-ttu-id="546fc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="546fc-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="546fc-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="546fc-124">Request body</span></span>
<span data-ttu-id="546fc-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="546fc-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="546fc-126">応答</span><span class="sxs-lookup"><span data-stu-id="546fc-126">Response</span></span>
<span data-ttu-id="546fc-127">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[governanceResource](../resources/governanceresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="546fc-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="546fc-128">例</span><span class="sxs-lookup"><span data-stu-id="546fc-128">Examples</span></span>

<span data-ttu-id="546fc-129">この例では、現在アクセスできるすべてのリソースが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="546fc-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="546fc-130">要求</span><span class="sxs-lookup"><span data-stu-id="546fc-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="546fc-131">応答</span><span class="sxs-lookup"><span data-stu-id="546fc-131">Response</span></span>
<span data-ttu-id="546fc-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="546fc-132">Here is an example of the response.</span></span> 

><span data-ttu-id="546fc-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="546fc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
