---
title: 登録 governanceResource
description: PIM では、アンマネージの governanceResource オブジェクトを登録します。
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837752"
---
# <a name="register-governanceresource"></a><span data-ttu-id="99e51-103">登録 governanceResource</span><span class="sxs-lookup"><span data-stu-id="99e51-103">Register governanceResource</span></span>

> <span data-ttu-id="99e51-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="99e51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99e51-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99e51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99e51-106">特権 Id 管理では、アンマネージ[governanceResource](../resources/governanceresource.md)オブジェクトを登録します。</span><span class="sxs-lookup"><span data-stu-id="99e51-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e51-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99e51-107">Permissions</span></span>
<span data-ttu-id="99e51-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99e51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="99e51-110">**注:** この API には、依頼者にあるリソースに 1 つ以上のアクティブなロールの割り当てが必要です。</span><span class="sxs-lookup"><span data-stu-id="99e51-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="99e51-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99e51-111">Permission type</span></span>      | <span data-ttu-id="99e51-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="99e51-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e51-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99e51-113">Delegated (work or school account)</span></span> | <span data-ttu-id="99e51-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="99e51-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="99e51-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99e51-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e51-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99e51-116">Not supported.</span></span>    |
|<span data-ttu-id="99e51-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99e51-117">Application</span></span> | <span data-ttu-id="99e51-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="99e51-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="99e51-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99e51-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="99e51-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="99e51-120">Optional query parameters</span></span>
<span data-ttu-id="99e51-121">このメソッド**のみ**をサポートしている、`$select`と`$expand`の応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)です。</span><span class="sxs-lookup"><span data-stu-id="99e51-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="99e51-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99e51-122">Request headers</span></span>
| <span data-ttu-id="99e51-123">名前</span><span class="sxs-lookup"><span data-stu-id="99e51-123">Name</span></span>      |<span data-ttu-id="99e51-124">説明</span><span class="sxs-lookup"><span data-stu-id="99e51-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99e51-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e51-125">Authorization</span></span>  | <span data-ttu-id="99e51-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="99e51-126">Bearer {code}</span></span>|
| <span data-ttu-id="99e51-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="99e51-127">Content-type</span></span>  | <span data-ttu-id="99e51-128">application/json</span><span class="sxs-lookup"><span data-stu-id="99e51-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="99e51-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="99e51-129">Request body</span></span>

|<span data-ttu-id="99e51-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="99e51-130">Parameters</span></span>      |<span data-ttu-id="99e51-131">型</span><span class="sxs-lookup"><span data-stu-id="99e51-131">Type</span></span>                 |<span data-ttu-id="99e51-132">必須</span><span class="sxs-lookup"><span data-stu-id="99e51-132">Required</span></span> |<span data-ttu-id="99e51-133">説明</span><span class="sxs-lookup"><span data-stu-id="99e51-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="99e51-134">externalId</span><span class="sxs-lookup"><span data-stu-id="99e51-134">externalId</span></span>    |<span data-ttu-id="99e51-135">String</span><span class="sxs-lookup"><span data-stu-id="99e51-135">String</span></span>                 |<span data-ttu-id="99e51-136">✓</span><span class="sxs-lookup"><span data-stu-id="99e51-136">✓</span></span>        |<span data-ttu-id="99e51-137">PIM に登録されるリソースの externalId です。</span><span class="sxs-lookup"><span data-stu-id="99e51-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="99e51-138">応答</span><span class="sxs-lookup"><span data-stu-id="99e51-138">Response</span></span>
<span data-ttu-id="99e51-139">かどうかは成功すると、このメソッドが返されます、`200 OK`応答します。</span><span class="sxs-lookup"><span data-stu-id="99e51-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="99e51-140">例</span><span class="sxs-lookup"><span data-stu-id="99e51-140">Example</span></span>
<span data-ttu-id="99e51-141">この例では、Azure のサブスクリプション Wingtip toys 社の商品を登録する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="99e51-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="99e51-142">要求</span><span class="sxs-lookup"><span data-stu-id="99e51-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="99e51-143">応答</span><span class="sxs-lookup"><span data-stu-id="99e51-143">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
