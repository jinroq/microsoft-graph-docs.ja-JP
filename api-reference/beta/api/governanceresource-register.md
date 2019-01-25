---
title: 登録 governanceResource
description: PIM では、アンマネージの governanceResource オブジェクトを登録します。
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519046"
---
# <a name="register-governanceresource"></a><span data-ttu-id="226d2-103">登録 governanceResource</span><span class="sxs-lookup"><span data-stu-id="226d2-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="226d2-104">特権 Id 管理では、アンマネージ[governanceResource](../resources/governanceresource.md)オブジェクトを登録します。</span><span class="sxs-lookup"><span data-stu-id="226d2-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="226d2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="226d2-105">Permissions</span></span>
<span data-ttu-id="226d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="226d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="226d2-108">**注:** この API には、依頼者にあるリソースに 1 つ以上のアクティブなロールの割り当てが必要です。</span><span class="sxs-lookup"><span data-stu-id="226d2-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="226d2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="226d2-109">Permission type</span></span>      | <span data-ttu-id="226d2-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="226d2-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="226d2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="226d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="226d2-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="226d2-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="226d2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="226d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="226d2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="226d2-114">Not supported.</span></span>    |
|<span data-ttu-id="226d2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="226d2-115">Application</span></span> | <span data-ttu-id="226d2-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="226d2-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="226d2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="226d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="226d2-118">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="226d2-118">Optional query parameters</span></span>
<span data-ttu-id="226d2-119">このメソッド**のみ**をサポートしている、`$select`と`$expand`の応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="226d2-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="226d2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="226d2-120">Request headers</span></span>
| <span data-ttu-id="226d2-121">名前</span><span class="sxs-lookup"><span data-stu-id="226d2-121">Name</span></span>      |<span data-ttu-id="226d2-122">説明</span><span class="sxs-lookup"><span data-stu-id="226d2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="226d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="226d2-123">Authorization</span></span>  | <span data-ttu-id="226d2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="226d2-124">Bearer {code}</span></span>|
| <span data-ttu-id="226d2-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="226d2-125">Content-type</span></span>  | <span data-ttu-id="226d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="226d2-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="226d2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="226d2-127">Request body</span></span>

|<span data-ttu-id="226d2-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="226d2-128">Parameters</span></span>      |<span data-ttu-id="226d2-129">型</span><span class="sxs-lookup"><span data-stu-id="226d2-129">Type</span></span>                 |<span data-ttu-id="226d2-130">必須</span><span class="sxs-lookup"><span data-stu-id="226d2-130">Required</span></span> |<span data-ttu-id="226d2-131">説明</span><span class="sxs-lookup"><span data-stu-id="226d2-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="226d2-132">externalId</span><span class="sxs-lookup"><span data-stu-id="226d2-132">externalId</span></span>    |<span data-ttu-id="226d2-133">String</span><span class="sxs-lookup"><span data-stu-id="226d2-133">String</span></span>                 |<span data-ttu-id="226d2-134">✓</span><span class="sxs-lookup"><span data-stu-id="226d2-134">✓</span></span>        |<span data-ttu-id="226d2-135">PIM に登録されるリソースの externalId です。</span><span class="sxs-lookup"><span data-stu-id="226d2-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="226d2-136">応答</span><span class="sxs-lookup"><span data-stu-id="226d2-136">Response</span></span>
<span data-ttu-id="226d2-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答します。</span><span class="sxs-lookup"><span data-stu-id="226d2-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="226d2-138">例</span><span class="sxs-lookup"><span data-stu-id="226d2-138">Example</span></span>
<span data-ttu-id="226d2-139">この例では、Azure のサブスクリプション Wingtip toys 社の商品を登録する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="226d2-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="226d2-140">要求</span><span class="sxs-lookup"><span data-stu-id="226d2-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="226d2-141">応答</span><span class="sxs-lookup"><span data-stu-id="226d2-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
