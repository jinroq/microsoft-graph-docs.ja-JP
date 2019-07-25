---
title: acceptedSenders のリスト化
description: このグループの許可された送信者リストに含まれるユーザーまたはグループの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2ccd38e8f28a348d174afa7cff6025c71262c89f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858545"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="3cece-103">acceptedSenders のリスト化</span><span class="sxs-lookup"><span data-stu-id="3cece-103">List acceptedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cece-104">このグループの許可された送信者リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3cece-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="3cece-p101">承諾済み送信者リスト内のユーザーは、グループの会話を投稿することができます (要求取得 URL で識別)。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="3cece-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cece-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3cece-107">Permissions</span></span>
<span data-ttu-id="3cece-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cece-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cece-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cece-110">Permission type</span></span>      | <span data-ttu-id="3cece-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cece-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cece-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cece-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cece-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cece-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cece-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cece-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cece-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cece-115">Not supported.</span></span>    |
|<span data-ttu-id="3cece-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cece-116">Application</span></span> | <span data-ttu-id="3cece-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cece-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cece-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cece-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cece-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3cece-119">Optional query parameters</span></span>
<span data-ttu-id="3cece-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3cece-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cece-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cece-121">Request headers</span></span>
| <span data-ttu-id="3cece-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cece-122">Header</span></span>       | <span data-ttu-id="3cece-123">値</span><span class="sxs-lookup"><span data-stu-id="3cece-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cece-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cece-124">Authorization</span></span>  | <span data-ttu-id="3cece-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3cece-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cece-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cece-127">Request body</span></span>
<span data-ttu-id="3cece-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3cece-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cece-129">応答</span><span class="sxs-lookup"><span data-stu-id="3cece-129">Response</span></span>
<span data-ttu-id="3cece-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3cece-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cece-131">例</span><span class="sxs-lookup"><span data-stu-id="3cece-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3cece-132">要求</span><span class="sxs-lookup"><span data-stu-id="3cece-132">Request</span></span>
<span data-ttu-id="3cece-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3cece-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3cece-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3cece-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cece-135">C#</span><span class="sxs-lookup"><span data-stu-id="3cece-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cece-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cece-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cece-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="3cece-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3cece-138">Java</span><span class="sxs-lookup"><span data-stu-id="3cece-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-acceptedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3cece-139">応答</span><span class="sxs-lookup"><span data-stu-id="3cece-139">Response</span></span>
<span data-ttu-id="3cece-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3cece-140">The following is an example of the response.</span></span>
><span data-ttu-id="3cece-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3cece-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3cece-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3cece-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
