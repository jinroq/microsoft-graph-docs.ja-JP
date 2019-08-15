---
title: リスト domainNameReferences
description: ドメインへの参照を使用して、directoryObject の一覧を取得します。 返される一覧には、ドメインに依存しているすべてのディレクトリオブジェクトが含まれています。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b39f3f0e2b387a8488e757f210a701b54108a052
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417074"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="443a2-104">リスト domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="443a2-104">List domainNameReferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="443a2-105">ドメインへの参照を使用して、 [Directoryobject](../resources/directoryobject.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="443a2-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="443a2-106">返される一覧には、ドメインに依存しているすべてのディレクトリオブジェクトが含まれています。</span><span class="sxs-lookup"><span data-stu-id="443a2-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="443a2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="443a2-107">Permissions</span></span>

<span data-ttu-id="443a2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="443a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="443a2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="443a2-110">Permission type</span></span>      | <span data-ttu-id="443a2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="443a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="443a2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="443a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="443a2-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="443a2-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="443a2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="443a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="443a2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="443a2-115">Not supported.</span></span>    |
|<span data-ttu-id="443a2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="443a2-116">Application</span></span> | <span data-ttu-id="443a2-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443a2-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="443a2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="443a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="443a2-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="443a2-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="443a2-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="443a2-120">Optional query parameters</span></span>

<span data-ttu-id="443a2-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="443a2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="443a2-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="443a2-122">Request headers</span></span>

| <span data-ttu-id="443a2-123">名前</span><span class="sxs-lookup"><span data-stu-id="443a2-123">Name</span></span>      |<span data-ttu-id="443a2-124">説明</span><span class="sxs-lookup"><span data-stu-id="443a2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="443a2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="443a2-125">Authorization</span></span>  | <span data-ttu-id="443a2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="443a2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="443a2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="443a2-128">Request body</span></span>

<span data-ttu-id="443a2-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="443a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="443a2-130">応答</span><span class="sxs-lookup"><span data-stu-id="443a2-130">Response</span></span>

<span data-ttu-id="443a2-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="443a2-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443a2-132">例</span><span class="sxs-lookup"><span data-stu-id="443a2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="443a2-133">要求</span><span class="sxs-lookup"><span data-stu-id="443a2-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="443a2-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="443a2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="443a2-135">C#</span><span class="sxs-lookup"><span data-stu-id="443a2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="443a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="443a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="443a2-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="443a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="443a2-138">応答</span><span class="sxs-lookup"><span data-stu-id="443a2-138">Response</span></span>
<span data-ttu-id="443a2-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="443a2-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
