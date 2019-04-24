---
title: 所有者を一覧表示する
description: 'グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。 '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5c8cf1c82ceab0a7fa2a7f78b6c229165448d46e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584683"
---
# <a name="list-owners"></a><span data-ttu-id="6f185-104">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6f185-104">List owners</span></span>
<span data-ttu-id="6f185-p102">グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="6f185-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6f185-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f185-107">Permissions</span></span>
<span data-ttu-id="6f185-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f185-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f185-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f185-110">Permission type</span></span>      | <span data-ttu-id="6f185-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f185-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f185-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f185-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f185-113">Group.Read.All と User.ReadBasic.All、Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f185-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="6f185-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f185-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f185-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f185-115">Not supported.</span></span>    |
|<span data-ttu-id="6f185-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f185-116">Application</span></span> | <span data-ttu-id="6f185-117">Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f185-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f185-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f185-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f185-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f185-119">Optional query parameters</span></span>
<span data-ttu-id="6f185-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6f185-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f185-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f185-121">Request headers</span></span>
| <span data-ttu-id="6f185-122">名前</span><span class="sxs-lookup"><span data-stu-id="6f185-122">Name</span></span>       | <span data-ttu-id="6f185-123">型</span><span class="sxs-lookup"><span data-stu-id="6f185-123">Type</span></span> | <span data-ttu-id="6f185-124">説明</span><span class="sxs-lookup"><span data-stu-id="6f185-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f185-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f185-125">Authorization</span></span>  | <span data-ttu-id="6f185-126">string</span><span class="sxs-lookup"><span data-stu-id="6f185-126">string</span></span>  | <span data-ttu-id="6f185-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6f185-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f185-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f185-129">Request body</span></span>
<span data-ttu-id="6f185-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f185-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f185-131">応答</span><span class="sxs-lookup"><span data-stu-id="6f185-131">Response</span></span>
<span data-ttu-id="6f185-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6f185-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f185-133">例</span><span class="sxs-lookup"><span data-stu-id="6f185-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6f185-134">要求</span><span class="sxs-lookup"><span data-stu-id="6f185-134">Request</span></span>
<span data-ttu-id="6f185-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f185-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="6f185-136">応答</span><span class="sxs-lookup"><span data-stu-id="6f185-136">Response</span></span>
<span data-ttu-id="6f185-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f185-137">The following is an example of the response.</span></span>
><span data-ttu-id="6f185-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6f185-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6f185-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f185-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
