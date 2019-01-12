---
title: 写真の一覧表示
description: profilePhoto オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 01fd069173fff1a7a6868f1596326fcb44d77fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932274"
---
# <a name="list-photos"></a><span data-ttu-id="34150-103">写真の一覧表示</span><span class="sxs-lookup"><span data-stu-id="34150-103">List photos</span></span>
<span data-ttu-id="34150-104">[profilePhoto](../resources/profilephoto.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="34150-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="34150-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34150-105">Permissions</span></span>
<span data-ttu-id="34150-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34150-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34150-108">Permission type</span></span>      | <span data-ttu-id="34150-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34150-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34150-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34150-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34150-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34150-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="34150-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34150-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34150-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34150-113">Not supported.</span></span>    |
|<span data-ttu-id="34150-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34150-114">Application</span></span> | <span data-ttu-id="34150-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34150-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34150-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34150-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34150-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="34150-117">Optional query parameters</span></span>
<span data-ttu-id="34150-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="34150-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34150-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34150-119">Request headers</span></span>
| <span data-ttu-id="34150-120">名前</span><span class="sxs-lookup"><span data-stu-id="34150-120">Name</span></span>       | <span data-ttu-id="34150-121">種類</span><span class="sxs-lookup"><span data-stu-id="34150-121">Type</span></span> | <span data-ttu-id="34150-122">説明</span><span class="sxs-lookup"><span data-stu-id="34150-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34150-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34150-123">Authorization</span></span>  | <span data-ttu-id="34150-124">string</span><span class="sxs-lookup"><span data-stu-id="34150-124">string</span></span>  | <span data-ttu-id="34150-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34150-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34150-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="34150-127">Request body</span></span>
<span data-ttu-id="34150-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="34150-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34150-129">応答</span><span class="sxs-lookup"><span data-stu-id="34150-129">Response</span></span>
<span data-ttu-id="34150-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="34150-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34150-131">例</span><span class="sxs-lookup"><span data-stu-id="34150-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="34150-132">要求</span><span class="sxs-lookup"><span data-stu-id="34150-132">Request</span></span>
<span data-ttu-id="34150-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34150-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="34150-134">応答</span><span class="sxs-lookup"><span data-stu-id="34150-134">Response</span></span>
<span data-ttu-id="34150-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34150-135">The following is an example of the response.</span></span>
><span data-ttu-id="34150-136">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="34150-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="34150-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="34150-137">All the properties will be returned from an actual call.</span></span>
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
