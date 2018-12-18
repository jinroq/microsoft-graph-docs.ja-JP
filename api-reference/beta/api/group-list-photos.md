---
title: 写真の一覧表示
description: profilePhoto オブジェクトのリストを取得します。
author: dkershaw10
ms.openlocfilehash: 2597d532d28614bb595ffe44aa6705187619aa44
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315821"
---
# <a name="list-photos"></a><span data-ttu-id="189b4-103">写真の一覧表示</span><span class="sxs-lookup"><span data-stu-id="189b4-103">List photos</span></span>

> <span data-ttu-id="189b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="189b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="189b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="189b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="189b4-106">[profilePhoto](../resources/profilephoto.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="189b4-106">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="189b4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="189b4-107">Permissions</span></span>
<span data-ttu-id="189b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="189b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="189b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="189b4-110">Permission type</span></span>      | <span data-ttu-id="189b4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="189b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="189b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="189b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="189b4-113">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189b4-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="189b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="189b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="189b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="189b4-115">Not supported.</span></span>    |
|<span data-ttu-id="189b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="189b4-116">Application</span></span> | <span data-ttu-id="189b4-117">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189b4-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="189b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="189b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="189b4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="189b4-119">Optional query parameters</span></span>
<span data-ttu-id="189b4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="189b4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="189b4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="189b4-121">Request headers</span></span>
| <span data-ttu-id="189b4-122">名前</span><span class="sxs-lookup"><span data-stu-id="189b4-122">Name</span></span>       | <span data-ttu-id="189b4-123">種類</span><span class="sxs-lookup"><span data-stu-id="189b4-123">Type</span></span> | <span data-ttu-id="189b4-124">説明</span><span class="sxs-lookup"><span data-stu-id="189b4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="189b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="189b4-125">Authorization</span></span>  | <span data-ttu-id="189b4-126">string</span><span class="sxs-lookup"><span data-stu-id="189b4-126">string</span></span>  | <span data-ttu-id="189b4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="189b4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="189b4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="189b4-129">Request body</span></span>
<span data-ttu-id="189b4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="189b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="189b4-131">応答</span><span class="sxs-lookup"><span data-stu-id="189b4-131">Response</span></span>
<span data-ttu-id="189b4-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="189b4-132">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="189b4-133">例</span><span class="sxs-lookup"><span data-stu-id="189b4-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="189b4-134">要求</span><span class="sxs-lookup"><span data-stu-id="189b4-134">Request</span></span>
<span data-ttu-id="189b4-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="189b4-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="189b4-136">応答</span><span class="sxs-lookup"><span data-stu-id="189b4-136">Response</span></span>
<span data-ttu-id="189b4-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="189b4-137">The following is an example of the response.</span></span>
><span data-ttu-id="189b4-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="189b4-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="189b4-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="189b4-139">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->