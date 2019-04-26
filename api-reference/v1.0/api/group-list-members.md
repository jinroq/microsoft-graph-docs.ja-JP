---
title: メンバーを一覧表示する
description: グループの直接メンバーの一覧を取得します。 グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 70bf3040402c03dc1918d271a2abb8e4adb5d40b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584650"
---
# <a name="list-members"></a><span data-ttu-id="f5382-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f5382-104">List members</span></span>
<span data-ttu-id="f5382-p102">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="f5382-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5382-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5382-108">Permissions</span></span>
<span data-ttu-id="f5382-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5382-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5382-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5382-111">Permission type</span></span>      | <span data-ttu-id="f5382-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5382-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5382-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5382-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f5382-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5382-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f5382-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5382-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5382-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5382-116">Not supported.</span></span>    |
|<span data-ttu-id="f5382-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5382-117">Application</span></span> | <span data-ttu-id="f5382-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5382-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5382-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5382-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5382-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f5382-120">Optional query parameters</span></span>
<span data-ttu-id="f5382-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f5382-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5382-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5382-122">Request headers</span></span>
| <span data-ttu-id="f5382-123">名前</span><span class="sxs-lookup"><span data-stu-id="f5382-123">Name</span></span>       | <span data-ttu-id="f5382-124">型</span><span class="sxs-lookup"><span data-stu-id="f5382-124">Type</span></span> | <span data-ttu-id="f5382-125">説明</span><span class="sxs-lookup"><span data-stu-id="f5382-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5382-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5382-126">Authorization</span></span>  | <span data-ttu-id="f5382-127">string</span><span class="sxs-lookup"><span data-stu-id="f5382-127">string</span></span>  | <span data-ttu-id="f5382-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5382-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5382-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5382-130">Request body</span></span>
<span data-ttu-id="f5382-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f5382-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5382-132">応答</span><span class="sxs-lookup"><span data-stu-id="f5382-132">Response</span></span>
<span data-ttu-id="f5382-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f5382-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5382-134">例</span><span class="sxs-lookup"><span data-stu-id="f5382-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5382-135">要求</span><span class="sxs-lookup"><span data-stu-id="f5382-135">Request</span></span>
<span data-ttu-id="f5382-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5382-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="f5382-137">応答</span><span class="sxs-lookup"><span data-stu-id="f5382-137">Response</span></span>
<span data-ttu-id="f5382-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5382-138">The following is an example of the response.</span></span>
><span data-ttu-id="f5382-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5382-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f5382-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f5382-140">All the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
