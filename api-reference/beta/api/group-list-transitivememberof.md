---
title: リストグループ推移的な memberOf
description: グループのメンバーであるグループおよび管理単位を取得します。  この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。 ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: edc0a86b0c394bfa71f439dbb3f0dc554f72d492
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323347"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="c889e-105">リストグループ推移的な memberOf</span><span class="sxs-lookup"><span data-stu-id="c889e-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c889e-106">グループのメンバーであるグループおよび管理単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="c889e-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="c889e-107">この操作は推移的で、このグループがネストされたメンバーであるすべてのグループも含みます。</span><span class="sxs-lookup"><span data-stu-id="c889e-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="c889e-108">ユーザーの Office 365 グループを取得する場合とは異なり、Office 365 グループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="c889e-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c889e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c889e-109">Permissions</span></span>

<span data-ttu-id="c889e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c889e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c889e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c889e-112">Permission type</span></span>      | <span data-ttu-id="c889e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c889e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c889e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c889e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c889e-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c889e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c889e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c889e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c889e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c889e-117">Not supported.</span></span>    |
|<span data-ttu-id="c889e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c889e-118">Application</span></span> | <span data-ttu-id="c889e-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c889e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c889e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c889e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c889e-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c889e-121">Optional query parameters</span></span>
<span data-ttu-id="c889e-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c889e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c889e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c889e-123">Request headers</span></span>
| <span data-ttu-id="c889e-124">名前</span><span class="sxs-lookup"><span data-stu-id="c889e-124">Name</span></span>       | <span data-ttu-id="c889e-125">型</span><span class="sxs-lookup"><span data-stu-id="c889e-125">Type</span></span> | <span data-ttu-id="c889e-126">説明</span><span class="sxs-lookup"><span data-stu-id="c889e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c889e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c889e-127">Authorization</span></span>  | <span data-ttu-id="c889e-128">string</span><span class="sxs-lookup"><span data-stu-id="c889e-128">string</span></span>  | <span data-ttu-id="c889e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c889e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c889e-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c889e-131">Request body</span></span>
<span data-ttu-id="c889e-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c889e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c889e-133">応答</span><span class="sxs-lookup"><span data-stu-id="c889e-133">Response</span></span>
<span data-ttu-id="c889e-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c889e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c889e-135">例</span><span class="sxs-lookup"><span data-stu-id="c889e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c889e-136">要求</span><span class="sxs-lookup"><span data-stu-id="c889e-136">Request</span></span>
<span data-ttu-id="c889e-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c889e-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c889e-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c889e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c889e-139">C#</span><span class="sxs-lookup"><span data-stu-id="c889e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c889e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c889e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c889e-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="c889e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c889e-142">Java</span><span class="sxs-lookup"><span data-stu-id="c889e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c889e-143">応答</span><span class="sxs-lookup"><span data-stu-id="c889e-143">Response</span></span>

<span data-ttu-id="c889e-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c889e-144">The following is an example of the response.</span></span>
><span data-ttu-id="c889e-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c889e-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c889e-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c889e-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
