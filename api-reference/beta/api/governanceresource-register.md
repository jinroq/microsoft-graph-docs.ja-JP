---
title: 'governanceResource: register'
description: PIM に governanceResource オブジェクトを登録します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713920"
---
# <a name="governanceresource-register"></a><span data-ttu-id="0d24e-103">governanceResource: register</span><span class="sxs-lookup"><span data-stu-id="0d24e-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d24e-104">特権 Id 管理に[governanceResource](../resources/governanceresource.md)オブジェクトを登録します。</span><span class="sxs-lookup"><span data-stu-id="0d24e-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d24e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d24e-105">Permissions</span></span>

<span data-ttu-id="0d24e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d24e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="0d24e-108">**注:** この API では、要求者がリソースに対して少なくとも1つのアクティブなロール割り当てを持っている必要もあります。</span><span class="sxs-lookup"><span data-stu-id="0d24e-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="0d24e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d24e-109">Permission type</span></span> | <span data-ttu-id="0d24e-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d24e-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0d24e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d24e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d24e-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="0d24e-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="0d24e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d24e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d24e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d24e-114">Not supported.</span></span> |
| <span data-ttu-id="0d24e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d24e-115">Application</span></span> | <span data-ttu-id="0d24e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d24e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d24e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d24e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d24e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0d24e-118">Optional query parameters</span></span>

<span data-ttu-id="0d24e-119">このメソッド\*\*\*\* は、応答`$select`を`$expand`カスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="0d24e-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d24e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d24e-120">Request headers</span></span>

| <span data-ttu-id="0d24e-121">名前</span><span class="sxs-lookup"><span data-stu-id="0d24e-121">Name</span></span> | <span data-ttu-id="0d24e-122">説明</span><span class="sxs-lookup"><span data-stu-id="0d24e-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0d24e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d24e-123">Authorization</span></span> | <span data-ttu-id="0d24e-124">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="0d24e-124">Bearer {token}</span></span> |
| <span data-ttu-id="0d24e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0d24e-125">Content-type</span></span> | <span data-ttu-id="0d24e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d24e-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d24e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d24e-127">Request body</span></span>

| <span data-ttu-id="0d24e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d24e-128">Properties</span></span> | <span data-ttu-id="0d24e-129">型</span><span class="sxs-lookup"><span data-stu-id="0d24e-129">Type</span></span> | <span data-ttu-id="0d24e-130">説明</span><span class="sxs-lookup"><span data-stu-id="0d24e-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="0d24e-131">externalId</span><span class="sxs-lookup"><span data-stu-id="0d24e-131">externalId</span></span> | <span data-ttu-id="0d24e-132">String</span><span class="sxs-lookup"><span data-stu-id="0d24e-132">String</span></span> | <span data-ttu-id="0d24e-133">PIM に登録するリソースの外部識別子。</span><span class="sxs-lookup"><span data-stu-id="0d24e-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="0d24e-134">サブスクリプションを登録する場合、識別子はサブスクリプション id の先頭に`/subscriptions/`になります。</span><span class="sxs-lookup"><span data-stu-id="0d24e-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="0d24e-135">たとえば、`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac` などです。</span><span class="sxs-lookup"><span data-stu-id="0d24e-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="0d24e-136">応答</span><span class="sxs-lookup"><span data-stu-id="0d24e-136">Response</span></span>

<span data-ttu-id="0d24e-137">成功した場合、このメソッド`200 OK`は応答を返します。</span><span class="sxs-lookup"><span data-stu-id="0d24e-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="0d24e-138">例</span><span class="sxs-lookup"><span data-stu-id="0d24e-138">Example</span></span>

<span data-ttu-id="0d24e-139">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0d24e-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="0d24e-140">要求</span><span class="sxs-lookup"><span data-stu-id="0d24e-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="0d24e-141">応答</span><span class="sxs-lookup"><span data-stu-id="0d24e-141">Response</span></span>
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
  "suppressions": []
}
-->
