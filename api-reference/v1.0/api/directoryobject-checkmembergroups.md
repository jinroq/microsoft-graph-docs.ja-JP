---
title: メンバー グループをチェックする
description: 指定したグループの一覧のメンバーシップを確認し、それらのグループをリストから返します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4dab149dcf4881ed23c8852f26d89aee43edb123
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016980"
---
# <a name="check-member-groups"></a><span data-ttu-id="5ea6c-103">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="5ea6c-103">Check member groups</span></span>

<span data-ttu-id="5ea6c-p101">指定したグループのリスト内のメンバーシップを確認し、そのリストから指定したユーザー、グループまたはディレクトリ オブジェクトがメンバーであるグループを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea6c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ea6c-106">Permissions</span></span>
<span data-ttu-id="5ea6c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea6c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ea6c-109">Permission type</span></span>      | <span data-ttu-id="5ea6c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ea6c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea6c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ea6c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea6c-112">すべてのユーザーとグループを取得します。すべて、そして、すべてを読み取ります。すべてのユーザーとグループ。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-112">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="5ea6c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ea6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea6c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-114">Not supported.</span></span>    |
|<span data-ttu-id="5ea6c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ea6c-115">Application</span></span> | <span data-ttu-id="5ea6c-116">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea6c-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="5ea6c-117">使用するアクセス許可の種類を決定するには、次のシナリオのガイダンスを使用します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-117">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="5ea6c-118">ユーザーを使用します。すべてのアクセス許可が、サインインしているユーザーのグループメンバーシップを確認します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-118">Use User.Read and Group.Read.All permissions to check group memberships for the signed-in user.</span></span>
- <span data-ttu-id="5ea6c-119">すべてのユーザーとグループのアクセス許可を使用して、すべての権限を取得します。すべて、または、すべてのユーザーのグループメンバーシップを確認します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-119">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to check group memberships for any user.</span></span>
- <span data-ttu-id="5ea6c-120">グループのグループメンバーシップを確認するには、すべてのアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-120">Use Group.Read.All permission to check group memberships for a group.</span></span>
- <span data-ttu-id="5ea6c-121">ディレクトリオブジェクトのグループメンバーシップを確認するには、すべてのアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-121">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ea6c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ea6c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="5ea6c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ea6c-123">Request headers</span></span>
| <span data-ttu-id="5ea6c-124">名前</span><span class="sxs-lookup"><span data-stu-id="5ea6c-124">Name</span></span>       | <span data-ttu-id="5ea6c-125">型</span><span class="sxs-lookup"><span data-stu-id="5ea6c-125">Type</span></span> | <span data-ttu-id="5ea6c-126">説明</span><span class="sxs-lookup"><span data-stu-id="5ea6c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ea6c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea6c-127">Authorization</span></span>  | <span data-ttu-id="5ea6c-128">string</span><span class="sxs-lookup"><span data-stu-id="5ea6c-128">string</span></span>  | <span data-ttu-id="5ea6c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ea6c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ea6c-131">Content-Type</span></span>  | <span data-ttu-id="5ea6c-132">string</span><span class="sxs-lookup"><span data-stu-id="5ea6c-132">string</span></span> | <span data-ttu-id="5ea6c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5ea6c-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ea6c-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ea6c-134">Request body</span></span>
<span data-ttu-id="5ea6c-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ea6c-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ea6c-136">Parameter</span></span>    | <span data-ttu-id="5ea6c-137">型</span><span class="sxs-lookup"><span data-stu-id="5ea6c-137">Type</span></span>   |<span data-ttu-id="5ea6c-138">説明</span><span class="sxs-lookup"><span data-stu-id="5ea6c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ea6c-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="5ea6c-139">groupIds</span></span>|<span data-ttu-id="5ea6c-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="5ea6c-140">String collection</span></span>|<span data-ttu-id="5ea6c-p104">メンバーシップを確認するためのグループのオブジェクト ID を含むコレクションです。最大 20 グループを指定することが可能です。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="5ea6c-143">応答</span><span class="sxs-lookup"><span data-stu-id="5ea6c-143">Response</span></span>

<span data-ttu-id="5ea6c-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea6c-145">例</span><span class="sxs-lookup"><span data-stu-id="5ea6c-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ea6c-146">要求</span><span class="sxs-lookup"><span data-stu-id="5ea6c-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5ea6c-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5ea6c-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ea6c-148">C#</span><span class="sxs-lookup"><span data-stu-id="5ea6c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ea6c-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ea6c-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ea6c-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="5ea6c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5ea6c-151">Java</span><span class="sxs-lookup"><span data-stu-id="5ea6c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ea6c-152">応答</span><span class="sxs-lookup"><span data-stu-id="5ea6c-152">Response</span></span>
<span data-ttu-id="5ea6c-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ea6c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
