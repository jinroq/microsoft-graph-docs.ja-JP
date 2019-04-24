---
title: governanceResource の登録
description: PIM に管理されていない governanceResource オブジェクトを登録します。
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463951"
---
# <a name="register-governanceresource"></a><span data-ttu-id="37d51-103">governanceResource の登録</span><span class="sxs-lookup"><span data-stu-id="37d51-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37d51-104">管理されていない[governanceResource](../resources/governanceresource.md)オブジェクトを特権 id 管理に登録します。</span><span class="sxs-lookup"><span data-stu-id="37d51-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="37d51-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37d51-105">Permissions</span></span>
<span data-ttu-id="37d51-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="37d51-108">**注:** この API では、要求者がリソースに対して少なくとも1つのアクティブなロール割り当てを持っている必要もあります。</span><span class="sxs-lookup"><span data-stu-id="37d51-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="37d51-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37d51-109">Permission type</span></span>      | <span data-ttu-id="37d51-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37d51-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37d51-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37d51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37d51-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="37d51-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="37d51-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37d51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37d51-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37d51-114">Not supported.</span></span>    |
|<span data-ttu-id="37d51-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37d51-115">Application</span></span> | <span data-ttu-id="37d51-116">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="37d51-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="37d51-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37d51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="37d51-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="37d51-118">Optional query parameters</span></span>
<span data-ttu-id="37d51-119">このメソッド\*\*\*\* は、応答`$select`を`$expand`カスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="37d51-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="37d51-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37d51-120">Request headers</span></span>
| <span data-ttu-id="37d51-121">名前</span><span class="sxs-lookup"><span data-stu-id="37d51-121">Name</span></span>      |<span data-ttu-id="37d51-122">説明</span><span class="sxs-lookup"><span data-stu-id="37d51-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37d51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37d51-123">Authorization</span></span>  | <span data-ttu-id="37d51-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="37d51-124">Bearer {code}</span></span>|
| <span data-ttu-id="37d51-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="37d51-125">Content-type</span></span>  | <span data-ttu-id="37d51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37d51-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="37d51-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="37d51-127">Request body</span></span>

|<span data-ttu-id="37d51-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="37d51-128">Parameters</span></span>      |<span data-ttu-id="37d51-129">Type</span><span class="sxs-lookup"><span data-stu-id="37d51-129">Type</span></span>                 |<span data-ttu-id="37d51-130">必須</span><span class="sxs-lookup"><span data-stu-id="37d51-130">Required</span></span> |<span data-ttu-id="37d51-131">説明</span><span class="sxs-lookup"><span data-stu-id="37d51-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="37d51-132">externalId</span><span class="sxs-lookup"><span data-stu-id="37d51-132">externalId</span></span>    |<span data-ttu-id="37d51-133">String</span><span class="sxs-lookup"><span data-stu-id="37d51-133">String</span></span>                 |<span data-ttu-id="37d51-134">✓</span><span class="sxs-lookup"><span data-stu-id="37d51-134">✓</span></span>        |<span data-ttu-id="37d51-135">PIM に登録するリソースの externalid。</span><span class="sxs-lookup"><span data-stu-id="37d51-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="37d51-136">応答</span><span class="sxs-lookup"><span data-stu-id="37d51-136">Response</span></span>
<span data-ttu-id="37d51-137">成功した場合、このメソッド`200 OK`は応答を返します。</span><span class="sxs-lookup"><span data-stu-id="37d51-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="37d51-138">例</span><span class="sxs-lookup"><span data-stu-id="37d51-138">Example</span></span>
<span data-ttu-id="37d51-139">この例では、Azure サブスクリプションの Wingtip Toys-生産を登録する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="37d51-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="37d51-140">要求</span><span class="sxs-lookup"><span data-stu-id="37d51-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="37d51-141">応答</span><span class="sxs-lookup"><span data-stu-id="37d51-141">Response</span></span>
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
