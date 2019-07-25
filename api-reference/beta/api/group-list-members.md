---
title: グループメンバーを一覧表示する
description: グループの直接メンバーの一覧を取得します。 グループには、ユーザー、連絡先、デバイス、サービスプリンシパル、およびその他のグループをメンバーとして含めることができます。 この操作は推移的ではありません。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 3cb6c9791e6a94d3d7091f21601db6deb6cb6dfb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858433"
---
# <a name="list-group-members"></a><span data-ttu-id="59360-105">グループメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59360-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59360-106">グループの直接メンバーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="59360-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="59360-107">グループには、ユーザー、連絡先、デバイス、サービスプリンシパル、およびその他のグループをメンバーとして含めることができます。</span><span class="sxs-lookup"><span data-stu-id="59360-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="59360-108">この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="59360-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="59360-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59360-109">Permissions</span></span>

<span data-ttu-id="59360-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59360-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59360-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59360-112">Permission type</span></span>      | <span data-ttu-id="59360-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59360-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59360-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59360-114">Delegated (work or school account)</span></span> | <span data-ttu-id="59360-115">Directory.accessasuser.all。 all、user. all、all、all、all、all、User. all</span><span class="sxs-lookup"><span data-stu-id="59360-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="59360-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59360-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59360-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59360-117">Not supported.</span></span>    |
|<span data-ttu-id="59360-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59360-118">Application</span></span> | <span data-ttu-id="59360-119">ディレクトリ。すべてのユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="59360-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="59360-120">注: 非表示のメンバーシップグループのメンバーを一覧表示するには、"Hidden" アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="59360-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="59360-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59360-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59360-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59360-122">Optional query parameters</span></span>
<span data-ttu-id="59360-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59360-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59360-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59360-124">Request headers</span></span>
| <span data-ttu-id="59360-125">名前</span><span class="sxs-lookup"><span data-stu-id="59360-125">Name</span></span>       | <span data-ttu-id="59360-126">型</span><span class="sxs-lookup"><span data-stu-id="59360-126">Type</span></span> | <span data-ttu-id="59360-127">説明</span><span class="sxs-lookup"><span data-stu-id="59360-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59360-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="59360-128">Authorization</span></span>  | <span data-ttu-id="59360-129">string</span><span class="sxs-lookup"><span data-stu-id="59360-129">string</span></span>  | <span data-ttu-id="59360-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59360-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59360-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="59360-132">Request body</span></span>
<span data-ttu-id="59360-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59360-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59360-134">応答</span><span class="sxs-lookup"><span data-stu-id="59360-134">Response</span></span>
<span data-ttu-id="59360-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59360-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59360-136">例</span><span class="sxs-lookup"><span data-stu-id="59360-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="59360-137">要求</span><span class="sxs-lookup"><span data-stu-id="59360-137">Request</span></span>
<span data-ttu-id="59360-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59360-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59360-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="59360-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59360-140">C#</span><span class="sxs-lookup"><span data-stu-id="59360-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59360-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="59360-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59360-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="59360-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59360-143">Java</span><span class="sxs-lookup"><span data-stu-id="59360-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="59360-144">応答</span><span class="sxs-lookup"><span data-stu-id="59360-144">Response</span></span>
<span data-ttu-id="59360-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59360-145">The following is an example of the response.</span></span>
><span data-ttu-id="59360-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="59360-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59360-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="59360-147">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
