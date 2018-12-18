---
title: memberOf を一覧表示する
description: 'グループが直接メンバーであるグループを取得します。 '
author: dkershaw10
ms.openlocfilehash: 5cd563c8697a0d93ca2d11c42b3b8c19b0ce7ec9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323584"
---
# <a name="list-memberof"></a><span data-ttu-id="29962-103">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="29962-103">List memberOf</span></span>
<span data-ttu-id="29962-104">グループが直接メンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="29962-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="29962-p101">この操作は推移的ではありません。ユーザーの Office 365 のグループ取得と異なり、これは Office 365 のグループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="29962-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="29962-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29962-107">Permissions</span></span>
<span data-ttu-id="29962-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29962-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29962-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29962-110">Permission type</span></span>      | <span data-ttu-id="29962-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29962-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29962-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29962-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29962-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="29962-113">Group.Read.All</span></span>    |
|<span data-ttu-id="29962-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29962-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29962-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29962-115">Not supported.</span></span>    |
|<span data-ttu-id="29962-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29962-116">Application</span></span> | <span data-ttu-id="29962-117">Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="29962-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29962-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29962-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29962-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="29962-119">Optional query parameters</span></span>
<span data-ttu-id="29962-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="29962-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29962-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29962-121">Request headers</span></span>
| <span data-ttu-id="29962-122">名前</span><span class="sxs-lookup"><span data-stu-id="29962-122">Name</span></span>       | <span data-ttu-id="29962-123">種類</span><span class="sxs-lookup"><span data-stu-id="29962-123">Type</span></span> | <span data-ttu-id="29962-124">説明</span><span class="sxs-lookup"><span data-stu-id="29962-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29962-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="29962-125">Authorization</span></span>  | <span data-ttu-id="29962-126">string</span><span class="sxs-lookup"><span data-stu-id="29962-126">string</span></span>  | <span data-ttu-id="29962-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29962-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29962-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="29962-129">Request body</span></span>
<span data-ttu-id="29962-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29962-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29962-131">応答</span><span class="sxs-lookup"><span data-stu-id="29962-131">Response</span></span>
<span data-ttu-id="29962-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="29962-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29962-133">例</span><span class="sxs-lookup"><span data-stu-id="29962-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="29962-134">要求</span><span class="sxs-lookup"><span data-stu-id="29962-134">Request</span></span>
<span data-ttu-id="29962-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29962-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="29962-136">応答</span><span class="sxs-lookup"><span data-stu-id="29962-136">Response</span></span>
<span data-ttu-id="29962-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29962-137">The following is an example of the response.</span></span>
><span data-ttu-id="29962-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="29962-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29962-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="29962-139">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->