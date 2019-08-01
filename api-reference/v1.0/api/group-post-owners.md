---
title: グループ所有者の追加
description: グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6237c3f82d5154b5f3db602fb0ffa7b0f94cc48f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014866"
---
# <a name="add-group-owner"></a><span data-ttu-id="11851-104">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="11851-104">Add group owner</span></span>
<span data-ttu-id="11851-p102">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="11851-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="11851-107">**Important:** グループの所持者を更新しグループのチームを作成した場合、 Microsoft Teams と所有者が同期するまで最大で 2 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="11851-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="11851-108">また、たとえば Planner プランを作成することによって所有者が Team で変更を加えられるようにしたい場合は、所有者もグループまたはチームのメンバーとして追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="11851-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="11851-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11851-109">Permissions</span></span>
<span data-ttu-id="11851-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11851-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11851-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11851-112">Permission type</span></span>      | <span data-ttu-id="11851-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11851-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11851-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11851-114">Delegated (work or school account)</span></span> | <span data-ttu-id="11851-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11851-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11851-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11851-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11851-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11851-117">Not supported.</span></span>    |
|<span data-ttu-id="11851-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11851-118">Application</span></span> | <span data-ttu-id="11851-119">Group.ReadWrite.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11851-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11851-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11851-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="11851-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11851-121">Request headers</span></span>
| <span data-ttu-id="11851-122">名前</span><span class="sxs-lookup"><span data-stu-id="11851-122">Name</span></span>       | <span data-ttu-id="11851-123">型</span><span class="sxs-lookup"><span data-stu-id="11851-123">Type</span></span> | <span data-ttu-id="11851-124">説明</span><span class="sxs-lookup"><span data-stu-id="11851-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11851-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="11851-125">Authorization</span></span>  | <span data-ttu-id="11851-126">string</span><span class="sxs-lookup"><span data-stu-id="11851-126">string</span></span>  | <span data-ttu-id="11851-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11851-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11851-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="11851-129">Request body</span></span>
<span data-ttu-id="11851-130">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="11851-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="11851-131">応答</span><span class="sxs-lookup"><span data-stu-id="11851-131">Response</span></span>
<span data-ttu-id="11851-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="11851-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11851-134">例</span><span class="sxs-lookup"><span data-stu-id="11851-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="11851-135">要求</span><span class="sxs-lookup"><span data-stu-id="11851-135">Request</span></span>
<span data-ttu-id="11851-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11851-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11851-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="11851-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11851-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="11851-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11851-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11851-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="11851-140">C#</span><span class="sxs-lookup"><span data-stu-id="11851-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="11851-141">Java</span><span class="sxs-lookup"><span data-stu-id="11851-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="11851-142">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="11851-142">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="11851-143">応答</span><span class="sxs-lookup"><span data-stu-id="11851-143">Response</span></span>
<span data-ttu-id="11851-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11851-144">The following is an example of the response.</span></span>
><span data-ttu-id="11851-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="11851-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="11851-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11851-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

