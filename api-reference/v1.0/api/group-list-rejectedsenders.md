---
title: rejectedSenders の一覧表示
description: 'このグループの拒否された送信者リストに含まれるユーザーまたはグループの一覧を取得します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ec7f40c38508bd8cdb12e699d4b0bce6144809f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614104"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="85b62-103">rejectedSenders の一覧表示</span><span class="sxs-lookup"><span data-stu-id="85b62-103">List rejectedSenders</span></span>
<span data-ttu-id="85b62-104">このグループの拒否された送信者リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="85b62-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="85b62-p101">拒否送信者リスト内のユーザーは、グループの会話に投稿できません (取得要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="85b62-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="85b62-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85b62-107">Permissions</span></span>
<span data-ttu-id="85b62-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85b62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85b62-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85b62-110">Permission type</span></span>      | <span data-ttu-id="85b62-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85b62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85b62-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85b62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85b62-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85b62-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="85b62-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85b62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85b62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85b62-115">Not supported.</span></span>    |
|<span data-ttu-id="85b62-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85b62-116">Application</span></span> | <span data-ttu-id="85b62-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85b62-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85b62-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85b62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85b62-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="85b62-119">Optional query parameters</span></span>
<span data-ttu-id="85b62-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="85b62-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85b62-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85b62-121">Request headers</span></span>
| <span data-ttu-id="85b62-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85b62-122">Header</span></span>       | <span data-ttu-id="85b62-123">値</span><span class="sxs-lookup"><span data-stu-id="85b62-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85b62-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85b62-124">Authorization</span></span>  | <span data-ttu-id="85b62-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85b62-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85b62-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="85b62-127">Request body</span></span>
<span data-ttu-id="85b62-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="85b62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85b62-129">応答</span><span class="sxs-lookup"><span data-stu-id="85b62-129">Response</span></span>
<span data-ttu-id="85b62-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="85b62-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85b62-131">例</span><span class="sxs-lookup"><span data-stu-id="85b62-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="85b62-132">要求</span><span class="sxs-lookup"><span data-stu-id="85b62-132">Request</span></span>
<span data-ttu-id="85b62-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85b62-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="85b62-134">応答</span><span class="sxs-lookup"><span data-stu-id="85b62-134">Response</span></span>
<span data-ttu-id="85b62-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85b62-135">The following is an example of the response.</span></span>
><span data-ttu-id="85b62-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="85b62-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85b62-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="85b62-137">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="85b62-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="85b62-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85b62-139">Visual</span><span class="sxs-lookup"><span data-stu-id="85b62-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85b62-140">Java</span><span class="sxs-lookup"><span data-stu-id="85b62-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
