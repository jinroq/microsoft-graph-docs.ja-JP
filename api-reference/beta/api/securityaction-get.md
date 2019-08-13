---
title: securityAction を取得する
description: SecurityAction オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f28ee0d518656e932dd3c9a1b35c719a5e4c26a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364153"
---
# <a name="get-securityaction"></a><span data-ttu-id="38915-103">securityAction を取得する</span><span class="sxs-lookup"><span data-stu-id="38915-103">Get securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38915-104">[SecurityAction](../resources/securityaction.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="38915-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38915-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38915-105">Permissions</span></span>

<span data-ttu-id="38915-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38915-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38915-108">Permission type</span></span>                        | <span data-ttu-id="38915-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38915-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38915-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38915-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38915-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38915-111">Not supported.</span></span> |
| <span data-ttu-id="38915-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38915-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38915-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38915-113">Not supported.</span></span> |
| <span data-ttu-id="38915-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38915-114">Application</span></span>                            | <span data-ttu-id="38915-115">SecurityActions. All、SecurityActions. すべて</span><span class="sxs-lookup"><span data-stu-id="38915-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38915-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38915-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38915-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="38915-117">Optional query parameters</span></span>

<span data-ttu-id="38915-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="38915-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="38915-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38915-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="38915-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38915-120">Request headers</span></span>

| <span data-ttu-id="38915-121">名前</span><span class="sxs-lookup"><span data-stu-id="38915-121">Name</span></span>      |<span data-ttu-id="38915-122">説明</span><span class="sxs-lookup"><span data-stu-id="38915-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38915-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38915-123">Authorization</span></span> | <span data-ttu-id="38915-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="38915-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="38915-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="38915-125">Request body</span></span>

<span data-ttu-id="38915-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="38915-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38915-127">応答</span><span class="sxs-lookup"><span data-stu-id="38915-127">Response</span></span>

<span data-ttu-id="38915-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityAction](../resources/securityaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38915-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38915-129">例</span><span class="sxs-lookup"><span data-stu-id="38915-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38915-130">要求</span><span class="sxs-lookup"><span data-stu-id="38915-130">Request</span></span>

<span data-ttu-id="38915-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38915-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38915-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="38915-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38915-133">C#</span><span class="sxs-lookup"><span data-stu-id="38915-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38915-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38915-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38915-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="38915-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="38915-136">Java</span><span class="sxs-lookup"><span data-stu-id="38915-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38915-137">応答</span><span class="sxs-lookup"><span data-stu-id="38915-137">Response</span></span>

<span data-ttu-id="38915-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38915-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="38915-139">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="38915-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="38915-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="38915-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
