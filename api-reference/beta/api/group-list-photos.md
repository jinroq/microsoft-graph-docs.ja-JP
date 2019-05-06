---
title: 写真の一覧表示
description: profilePhoto オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d1ce8094e34370c5a04d770b46e7d7f9982233e5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592842"
---
# <a name="list-photos"></a><span data-ttu-id="e5cda-103">写真の一覧表示</span><span class="sxs-lookup"><span data-stu-id="e5cda-103">List photos</span></span>
<span data-ttu-id="e5cda-104">[profilePhoto](../resources/profilephoto.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e5cda-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5cda-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5cda-105">Permissions</span></span>
<span data-ttu-id="e5cda-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5cda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cda-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5cda-108">Permission type</span></span>      | <span data-ttu-id="e5cda-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5cda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5cda-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5cda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5cda-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cda-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="e5cda-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5cda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5cda-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5cda-113">Not supported.</span></span>    |
|<span data-ttu-id="e5cda-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5cda-114">Application</span></span> | <span data-ttu-id="e5cda-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cda-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5cda-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5cda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5cda-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e5cda-117">Optional query parameters</span></span>
<span data-ttu-id="e5cda-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e5cda-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5cda-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5cda-119">Request headers</span></span>
| <span data-ttu-id="e5cda-120">名前</span><span class="sxs-lookup"><span data-stu-id="e5cda-120">Name</span></span>       | <span data-ttu-id="e5cda-121">型</span><span class="sxs-lookup"><span data-stu-id="e5cda-121">Type</span></span> | <span data-ttu-id="e5cda-122">説明</span><span class="sxs-lookup"><span data-stu-id="e5cda-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5cda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5cda-123">Authorization</span></span>  | <span data-ttu-id="e5cda-124">string</span><span class="sxs-lookup"><span data-stu-id="e5cda-124">string</span></span>  | <span data-ttu-id="e5cda-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5cda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5cda-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5cda-127">Request body</span></span>
<span data-ttu-id="e5cda-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5cda-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5cda-129">応答</span><span class="sxs-lookup"><span data-stu-id="e5cda-129">Response</span></span>
<span data-ttu-id="e5cda-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e5cda-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cda-131">例</span><span class="sxs-lookup"><span data-stu-id="e5cda-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e5cda-132">要求</span><span class="sxs-lookup"><span data-stu-id="e5cda-132">Request</span></span>
<span data-ttu-id="e5cda-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5cda-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="e5cda-134">応答</span><span class="sxs-lookup"><span data-stu-id="e5cda-134">Response</span></span>
<span data-ttu-id="e5cda-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5cda-135">The following is an example of the response.</span></span>
><span data-ttu-id="e5cda-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e5cda-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5cda-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e5cda-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e5cda-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e5cda-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e5cda-139">Visual</span><span class="sxs-lookup"><span data-stu-id="e5cda-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5cda-140">Java</span><span class="sxs-lookup"><span data-stu-id="e5cda-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
