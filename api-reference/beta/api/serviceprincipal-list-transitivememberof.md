---
title: ServicePrincipal 推移的な memberOf のリスト
description: このサービスプリンシパルがメンバーになっているグループとディレクトリロールを取得します。 この操作は推移的で、このサービスプリンシパルがネストされたメンバーであるすべてのグループが含まれます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8c124819ed514a2d423b98bdc6ebd881dd31ebe2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363943"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="e6ce7-104">ServicePrincipal 推移的な memberOf のリスト</span><span class="sxs-lookup"><span data-stu-id="e6ce7-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ce7-105">このサービスプリンシパルがメンバーになっているグループとディレクトリロールを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="e6ce7-106">この操作は推移的で、このサービスプリンシパルがネストされたメンバーであるすべてのグループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ce7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6ce7-107">Permissions</span></span>
<span data-ttu-id="e6ce7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ce7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6ce7-110">Permission type</span></span>      | <span data-ttu-id="e6ce7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6ce7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6ce7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6ce7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6ce7-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6ce7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6ce7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6ce7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ce7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-115">Not supported.</span></span>    |
|<span data-ttu-id="e6ce7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6ce7-116">Application</span></span> | <span data-ttu-id="e6ce7-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ce7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6ce7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6ce7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6ce7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6ce7-119">Optional query parameters</span></span>
<span data-ttu-id="e6ce7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6ce7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6ce7-121">Request headers</span></span>
| <span data-ttu-id="e6ce7-122">名前</span><span class="sxs-lookup"><span data-stu-id="e6ce7-122">Name</span></span>       | <span data-ttu-id="e6ce7-123">型</span><span class="sxs-lookup"><span data-stu-id="e6ce7-123">Type</span></span> | <span data-ttu-id="e6ce7-124">説明</span><span class="sxs-lookup"><span data-stu-id="e6ce7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e6ce7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ce7-125">Authorization</span></span>  | <span data-ttu-id="e6ce7-126">string</span><span class="sxs-lookup"><span data-stu-id="e6ce7-126">string</span></span>  | <span data-ttu-id="e6ce7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6ce7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6ce7-129">Request body</span></span>
<span data-ttu-id="e6ce7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6ce7-131">応答</span><span class="sxs-lookup"><span data-stu-id="e6ce7-131">Response</span></span>

<span data-ttu-id="e6ce7-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ce7-133">例</span><span class="sxs-lookup"><span data-stu-id="e6ce7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6ce7-134">要求</span><span class="sxs-lookup"><span data-stu-id="e6ce7-134">Request</span></span>

<span data-ttu-id="e6ce7-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e6ce7-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e6ce7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e6ce7-137">C#</span><span class="sxs-lookup"><span data-stu-id="e6ce7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6ce7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ce7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e6ce7-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="e6ce7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e6ce7-140">Java</span><span class="sxs-lookup"><span data-stu-id="e6ce7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6ce7-141">応答</span><span class="sxs-lookup"><span data-stu-id="e6ce7-141">Response</span></span>

<span data-ttu-id="e6ce7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6ce7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
