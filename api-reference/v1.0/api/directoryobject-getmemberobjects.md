---
title: メンバー オブジェクトを取得する
description: " ユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。この関数は、推移的です。 "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78a2b0d3fe108ff7dc90c1ed878f01e3f84e4f80
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016805"
---
# <a name="get-member-objects"></a><span data-ttu-id="4cea7-104">メンバー オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="4cea7-104">Get member objects</span></span>

 <span data-ttu-id="4cea7-p102">ユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="4cea7-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="4cea7-107">注:ユーザーのみがディレクトリ ロールのメンバーになることができます。</span><span class="sxs-lookup"><span data-stu-id="4cea7-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cea7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4cea7-108">Permissions</span></span>
<span data-ttu-id="4cea7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cea7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cea7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4cea7-111">Permission type</span></span>      | <span data-ttu-id="4cea7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4cea7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cea7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4cea7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4cea7-114">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cea7-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="4cea7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4cea7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cea7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cea7-116">Not supported.</span></span>    |
|<span data-ttu-id="4cea7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4cea7-117">Application</span></span> | <span data-ttu-id="4cea7-118">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cea7-118">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cea7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4cea7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="4cea7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cea7-120">Request headers</span></span>
| <span data-ttu-id="4cea7-121">名前</span><span class="sxs-lookup"><span data-stu-id="4cea7-121">Name</span></span>       | <span data-ttu-id="4cea7-122">型</span><span class="sxs-lookup"><span data-stu-id="4cea7-122">Type</span></span> | <span data-ttu-id="4cea7-123">説明</span><span class="sxs-lookup"><span data-stu-id="4cea7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4cea7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cea7-124">Authorization</span></span>  | <span data-ttu-id="4cea7-125">string</span><span class="sxs-lookup"><span data-stu-id="4cea7-125">string</span></span>  | <span data-ttu-id="4cea7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4cea7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cea7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cea7-128">Content-Type</span></span>   | <span data-ttu-id="4cea7-129">string</span><span class="sxs-lookup"><span data-stu-id="4cea7-129">string</span></span>  | <span data-ttu-id="4cea7-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4cea7-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4cea7-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="4cea7-131">Request body</span></span>
<span data-ttu-id="4cea7-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4cea7-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4cea7-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4cea7-133">Parameter</span></span>    | <span data-ttu-id="4cea7-134">型</span><span class="sxs-lookup"><span data-stu-id="4cea7-134">Type</span></span>   |<span data-ttu-id="4cea7-135">説明</span><span class="sxs-lookup"><span data-stu-id="4cea7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cea7-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4cea7-136">securityEnabledOnly</span></span>|<span data-ttu-id="4cea7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cea7-137">Boolean</span></span>| <span data-ttu-id="4cea7-p105">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="4cea7-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="4cea7-140">応答</span><span class="sxs-lookup"><span data-stu-id="4cea7-140">Response</span></span>

<span data-ttu-id="4cea7-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4cea7-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cea7-142">例</span><span class="sxs-lookup"><span data-stu-id="4cea7-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4cea7-143">要求</span><span class="sxs-lookup"><span data-stu-id="4cea7-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4cea7-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4cea7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4cea7-145">C#</span><span class="sxs-lookup"><span data-stu-id="4cea7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cea7-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="4cea7-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4cea7-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="4cea7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4cea7-148">Java</span><span class="sxs-lookup"><span data-stu-id="4cea7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4cea7-149">応答</span><span class="sxs-lookup"><span data-stu-id="4cea7-149">Response</span></span>
<span data-ttu-id="4cea7-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4cea7-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
