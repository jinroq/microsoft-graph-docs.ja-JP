---
title: メンバー グループを取得する
description: 指定したユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。この関数は、推移的です。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a74031d0d4f91d26b5bf0c67a28854ff54b8957d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890146"
---
# <a name="get-member-groups"></a><span data-ttu-id="924a7-104">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="924a7-104">Get member groups</span></span>

<span data-ttu-id="924a7-p102">指定したユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="924a7-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="924a7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="924a7-107">Permissions</span></span>
<span data-ttu-id="924a7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="924a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="924a7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="924a7-110">Permission type</span></span>      | <span data-ttu-id="924a7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="924a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="924a7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="924a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="924a7-113">すべてのユーザーとグループを取得します。すべて、そして、すべてを読み取ります。すべてのユーザーとグループ。</span><span class="sxs-lookup"><span data-stu-id="924a7-113">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="924a7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="924a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="924a7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="924a7-115">Not supported.</span></span>    |
|<span data-ttu-id="924a7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="924a7-116">Application</span></span> | <span data-ttu-id="924a7-117">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="924a7-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="924a7-118">使用するアクセス許可の種類を決定するには、次のシナリオのガイダンスを使用します。</span><span class="sxs-lookup"><span data-stu-id="924a7-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="924a7-119">ユーザーを使用して、サインインしているユーザーのグループメンバーシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="924a7-119">Use User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="924a7-120">すべてのユーザーとグループのアクセス許可を使用して、すべての権限を取得します。すべて、またはすべてのアクセス許可を取得します。すべてのユーザーのグループメンバーシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="924a7-120">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="924a7-121">グループのグループメンバーシップを取得するには、すべてのアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="924a7-121">Use Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="924a7-122">ディレクトリオブジェクトのグループメンバーシップを取得するには、すべてのアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="924a7-122">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>


## <a name="http-request"></a><span data-ttu-id="924a7-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="924a7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="924a7-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="924a7-124">Request headers</span></span>
| <span data-ttu-id="924a7-125">名前</span><span class="sxs-lookup"><span data-stu-id="924a7-125">Name</span></span>       | <span data-ttu-id="924a7-126">型</span><span class="sxs-lookup"><span data-stu-id="924a7-126">Type</span></span> | <span data-ttu-id="924a7-127">説明</span><span class="sxs-lookup"><span data-stu-id="924a7-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="924a7-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="924a7-128">Authorization</span></span>  | <span data-ttu-id="924a7-129">string</span><span class="sxs-lookup"><span data-stu-id="924a7-129">string</span></span>  | <span data-ttu-id="924a7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="924a7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="924a7-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="924a7-132">Content-Type</span></span>   | <span data-ttu-id="924a7-133">string</span><span class="sxs-lookup"><span data-stu-id="924a7-133">string</span></span>  | <span data-ttu-id="924a7-134">application/json</span><span class="sxs-lookup"><span data-stu-id="924a7-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="924a7-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="924a7-135">Request body</span></span>
<span data-ttu-id="924a7-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="924a7-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="924a7-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="924a7-137">Parameter</span></span>    | <span data-ttu-id="924a7-138">型</span><span class="sxs-lookup"><span data-stu-id="924a7-138">Type</span></span>   |<span data-ttu-id="924a7-139">説明</span><span class="sxs-lookup"><span data-stu-id="924a7-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="924a7-140">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="924a7-140">securityEnabledOnly</span></span>|<span data-ttu-id="924a7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="924a7-141">Boolean</span></span>| <span data-ttu-id="924a7-p105">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="924a7-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="924a7-144">応答</span><span class="sxs-lookup"><span data-stu-id="924a7-144">Response</span></span>

<span data-ttu-id="924a7-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="924a7-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="924a7-146">例</span><span class="sxs-lookup"><span data-stu-id="924a7-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="924a7-147">要求</span><span class="sxs-lookup"><span data-stu-id="924a7-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="924a7-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="924a7-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="924a7-149">C#</span><span class="sxs-lookup"><span data-stu-id="924a7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="924a7-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="924a7-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="924a7-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="924a7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="924a7-152">Java</span><span class="sxs-lookup"><span data-stu-id="924a7-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="924a7-153">応答</span><span class="sxs-lookup"><span data-stu-id="924a7-153">Response</span></span>
<span data-ttu-id="924a7-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="924a7-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
