---
title: rejectedSenders の一覧表示
description: 'このグループの拒否された送信者リストに含まれるユーザーまたはグループの一覧を取得します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 503fc8b2534b540899f63323b09cfb8372843cd0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323373"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="5704d-103">rejectedSenders の一覧表示</span><span class="sxs-lookup"><span data-stu-id="5704d-103">List rejectedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5704d-104">このグループの拒否された送信者リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5704d-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="5704d-p101">拒否送信者リスト内のユーザーは、グループの会話に投稿できません (取得要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="5704d-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5704d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5704d-107">Permissions</span></span>
<span data-ttu-id="5704d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5704d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5704d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5704d-110">Permission type</span></span>      | <span data-ttu-id="5704d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5704d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5704d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5704d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5704d-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5704d-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5704d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5704d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5704d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5704d-115">Not supported.</span></span>    |
|<span data-ttu-id="5704d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5704d-116">Application</span></span> | <span data-ttu-id="5704d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5704d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5704d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5704d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5704d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5704d-119">Optional query parameters</span></span>
<span data-ttu-id="5704d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5704d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5704d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5704d-121">Request headers</span></span>
| <span data-ttu-id="5704d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5704d-122">Header</span></span>       | <span data-ttu-id="5704d-123">値</span><span class="sxs-lookup"><span data-stu-id="5704d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5704d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5704d-124">Authorization</span></span>  | <span data-ttu-id="5704d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5704d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5704d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5704d-127">Request body</span></span>
<span data-ttu-id="5704d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5704d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5704d-129">応答</span><span class="sxs-lookup"><span data-stu-id="5704d-129">Response</span></span>
<span data-ttu-id="5704d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5704d-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5704d-131">例</span><span class="sxs-lookup"><span data-stu-id="5704d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5704d-132">要求</span><span class="sxs-lookup"><span data-stu-id="5704d-132">Request</span></span>
<span data-ttu-id="5704d-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5704d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5704d-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5704d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5704d-135">C#</span><span class="sxs-lookup"><span data-stu-id="5704d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5704d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5704d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5704d-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="5704d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5704d-138">Java</span><span class="sxs-lookup"><span data-stu-id="5704d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5704d-139">応答</span><span class="sxs-lookup"><span data-stu-id="5704d-139">Response</span></span>
<span data-ttu-id="5704d-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5704d-140">The following is an example of the response.</span></span>
><span data-ttu-id="5704d-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5704d-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5704d-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5704d-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
