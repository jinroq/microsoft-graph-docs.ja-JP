---
title: 'group: getMemberObjects'
description: グループがメンバーになっているすべてのグループおよび管理単位を返します。 チェックは推移的です。 注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 772b5967964d39bdee55abc2350a69bd233d709b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326346"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="9d3ac-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="9d3ac-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d3ac-106">グループがメンバーになっているすべてのグループおよび管理単位を返します。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="9d3ac-107">チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-107">The check is transitive.</span></span> <span data-ttu-id="9d3ac-108">注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d3ac-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d3ac-109">Permissions</span></span>
<span data-ttu-id="9d3ac-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d3ac-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d3ac-112">Permission type</span></span>      | <span data-ttu-id="9d3ac-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d3ac-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3ac-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d3ac-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3ac-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d3ac-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d3ac-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d3ac-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3ac-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-117">Not supported.</span></span>    |
|<span data-ttu-id="9d3ac-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d3ac-118">Application</span></span> | <span data-ttu-id="9d3ac-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3ac-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d3ac-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d3ac-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="9d3ac-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d3ac-121">Request headers</span></span>
| <span data-ttu-id="9d3ac-122">名前</span><span class="sxs-lookup"><span data-stu-id="9d3ac-122">Name</span></span>       | <span data-ttu-id="9d3ac-123">型</span><span class="sxs-lookup"><span data-stu-id="9d3ac-123">Type</span></span> | <span data-ttu-id="9d3ac-124">説明</span><span class="sxs-lookup"><span data-stu-id="9d3ac-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d3ac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d3ac-125">Authorization</span></span>  | <span data-ttu-id="9d3ac-126">string</span><span class="sxs-lookup"><span data-stu-id="9d3ac-126">string</span></span>  | <span data-ttu-id="9d3ac-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d3ac-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d3ac-129">Request body</span></span>
<span data-ttu-id="9d3ac-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d3ac-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d3ac-131">Parameter</span></span>    | <span data-ttu-id="9d3ac-132">型</span><span class="sxs-lookup"><span data-stu-id="9d3ac-132">Type</span></span>   |<span data-ttu-id="9d3ac-133">説明</span><span class="sxs-lookup"><span data-stu-id="9d3ac-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d3ac-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9d3ac-134">securityEnabledOnly</span></span>|<span data-ttu-id="9d3ac-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d3ac-135">Boolean</span></span>|<span data-ttu-id="9d3ac-p105">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="9d3ac-138">応答</span><span class="sxs-lookup"><span data-stu-id="9d3ac-138">Response</span></span>
<span data-ttu-id="9d3ac-139">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="9d3ac-140">例</span><span class="sxs-lookup"><span data-stu-id="9d3ac-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d3ac-141">要求</span><span class="sxs-lookup"><span data-stu-id="9d3ac-141">Request</span></span>
<span data-ttu-id="9d3ac-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d3ac-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9d3ac-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d3ac-144">C#</span><span class="sxs-lookup"><span data-stu-id="9d3ac-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d3ac-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d3ac-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d3ac-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="9d3ac-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9d3ac-147">Java</span><span class="sxs-lookup"><span data-stu-id="9d3ac-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d3ac-148">応答</span><span class="sxs-lookup"><span data-stu-id="9d3ac-148">Response</span></span>
<span data-ttu-id="9d3ac-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-149">The following is an example of the response.</span></span>
><span data-ttu-id="9d3ac-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d3ac-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
