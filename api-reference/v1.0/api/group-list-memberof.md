---
title: memberOf を一覧表示する
description: 'グループが直接メンバーであるグループを取得します。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 01cda0abbbfb6f3646cb67b05a6d7a2865eccd2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889144"
---
# <a name="list-memberof"></a><span data-ttu-id="54d17-103">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="54d17-103">List memberOf</span></span>
<span data-ttu-id="54d17-104">グループが直接メンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="54d17-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="54d17-p101">この操作は推移的ではありません。ユーザーの Office 365 のグループ取得と異なり、これは Office 365 のグループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="54d17-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d17-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54d17-107">Permissions</span></span>
<span data-ttu-id="54d17-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54d17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d17-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54d17-110">Permission type</span></span>      | <span data-ttu-id="54d17-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54d17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54d17-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54d17-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54d17-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d17-113">Group.Read.All</span></span>    |
|<span data-ttu-id="54d17-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54d17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d17-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54d17-115">Not supported.</span></span>    |
|<span data-ttu-id="54d17-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54d17-116">Application</span></span> | <span data-ttu-id="54d17-117">Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d17-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d17-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54d17-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54d17-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="54d17-119">Optional query parameters</span></span>
<span data-ttu-id="54d17-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="54d17-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54d17-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54d17-121">Request headers</span></span>
| <span data-ttu-id="54d17-122">名前</span><span class="sxs-lookup"><span data-stu-id="54d17-122">Name</span></span>       | <span data-ttu-id="54d17-123">型</span><span class="sxs-lookup"><span data-stu-id="54d17-123">Type</span></span> | <span data-ttu-id="54d17-124">説明</span><span class="sxs-lookup"><span data-stu-id="54d17-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54d17-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d17-125">Authorization</span></span>  | <span data-ttu-id="54d17-126">string</span><span class="sxs-lookup"><span data-stu-id="54d17-126">string</span></span>  | <span data-ttu-id="54d17-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54d17-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54d17-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="54d17-129">Request body</span></span>
<span data-ttu-id="54d17-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54d17-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d17-131">応答</span><span class="sxs-lookup"><span data-stu-id="54d17-131">Response</span></span>
<span data-ttu-id="54d17-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="54d17-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d17-133">例</span><span class="sxs-lookup"><span data-stu-id="54d17-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="54d17-134">要求</span><span class="sxs-lookup"><span data-stu-id="54d17-134">Request</span></span>
<span data-ttu-id="54d17-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="54d17-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="54d17-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="54d17-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54d17-137">C#</span><span class="sxs-lookup"><span data-stu-id="54d17-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54d17-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="54d17-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54d17-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54d17-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="54d17-140">Java</span><span class="sxs-lookup"><span data-stu-id="54d17-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54d17-141">応答</span><span class="sxs-lookup"><span data-stu-id="54d17-141">Response</span></span>
<span data-ttu-id="54d17-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="54d17-142">The following is an example of the response.</span></span>
><span data-ttu-id="54d17-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="54d17-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="54d17-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="54d17-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
