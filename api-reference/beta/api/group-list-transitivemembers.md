---
title: グループ推移性のメンバーを一覧表示する
description: グループのメンバーの一覧を取得します。 グループには、ユーザー、連絡先、デバイス、サービスプリンシパル、およびその他のグループをメンバーとして含めることができます。 この操作は推移的であり、入れ子にされたすべてのメンバーのフラットな一覧も返します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f98dc43773a5679a3458ebc52f58c2eab9d455ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953634"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="f41b1-105">グループ推移性のメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f41b1-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f41b1-106">グループのメンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-106">Get a list of the group's members.</span></span> <span data-ttu-id="f41b1-107">グループには、ユーザー、連絡先、デバイス、サービスプリンシパル、およびその他のグループをメンバーとして含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f41b1-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="f41b1-108">この操作は推移的であり、入れ子にされたすべてのメンバーのフラットな一覧も返します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="f41b1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f41b1-109">Permissions</span></span>

<span data-ttu-id="f41b1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f41b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f41b1-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f41b1-112">Permission type</span></span>      | <span data-ttu-id="f41b1-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f41b1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f41b1-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f41b1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f41b1-115">Directory.accessasuser.all。 all、user. all、all、all、all、all、User. all</span><span class="sxs-lookup"><span data-stu-id="f41b1-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="f41b1-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f41b1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f41b1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f41b1-117">Not supported.</span></span>    |
|<span data-ttu-id="f41b1-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f41b1-118">Application</span></span> | <span data-ttu-id="f41b1-119">ディレクトリ。すべてのユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="f41b1-120">注: 非表示のメンバーシップグループのメンバーを一覧表示するには、"Hidden" アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f41b1-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="f41b1-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f41b1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f41b1-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f41b1-122">Optional query parameters</span></span>

<span data-ttu-id="f41b1-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f41b1-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f41b1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f41b1-124">Request headers</span></span>

| <span data-ttu-id="f41b1-125">名前</span><span class="sxs-lookup"><span data-stu-id="f41b1-125">Name</span></span>       | <span data-ttu-id="f41b1-126">型</span><span class="sxs-lookup"><span data-stu-id="f41b1-126">Type</span></span> | <span data-ttu-id="f41b1-127">説明</span><span class="sxs-lookup"><span data-stu-id="f41b1-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f41b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41b1-128">Authorization</span></span>  | <span data-ttu-id="f41b1-129">string</span><span class="sxs-lookup"><span data-stu-id="f41b1-129">string</span></span>  | <span data-ttu-id="f41b1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f41b1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f41b1-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="f41b1-132">Request body</span></span>

<span data-ttu-id="f41b1-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f41b1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f41b1-134">応答</span><span class="sxs-lookup"><span data-stu-id="f41b1-134">Response</span></span>

<span data-ttu-id="f41b1-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f41b1-136">例</span><span class="sxs-lookup"><span data-stu-id="f41b1-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f41b1-137">要求</span><span class="sxs-lookup"><span data-stu-id="f41b1-137">Request</span></span>

<span data-ttu-id="f41b1-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f41b1-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f41b1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f41b1-140">C#</span><span class="sxs-lookup"><span data-stu-id="f41b1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f41b1-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f41b1-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f41b1-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="f41b1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f41b1-143">Java</span><span class="sxs-lookup"><span data-stu-id="f41b1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f41b1-144">応答</span><span class="sxs-lookup"><span data-stu-id="f41b1-144">Response</span></span>

<span data-ttu-id="f41b1-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f41b1-145">The following is an example of the response.</span></span>
><span data-ttu-id="f41b1-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f41b1-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f41b1-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f41b1-147">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
