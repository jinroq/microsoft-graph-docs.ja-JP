---
title: グループ所有者の追加
description: グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
ms.openlocfilehash: 903c659722877263038860c7d2ff47b301b6d5c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308898"
---
# <a name="add-group-owner"></a><span data-ttu-id="e03bb-104">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="e03bb-104">Add group owner</span></span>

> <span data-ttu-id="e03bb-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e03bb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e03bb-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e03bb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e03bb-p103">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="e03bb-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="e03bb-109">**重要な:** グループの所有者を更新すると、グループのチームを作成した、マイクロソフトのチームとの同期に所有者には、最大で 2 時間がかかります。</span><span class="sxs-lookup"><span data-stu-id="e03bb-109">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="e03bb-110">また、- たとえば、プランナーの計画を作成するので、チームで変更を加えることができる所有者所有者も必要があります、グループまたはチームのメンバーとして追加します。</span><span class="sxs-lookup"><span data-stu-id="e03bb-110">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e03bb-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e03bb-111">Permissions</span></span>
<span data-ttu-id="e03bb-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e03bb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e03bb-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e03bb-114">Permission type</span></span>      | <span data-ttu-id="e03bb-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e03bb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e03bb-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e03bb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e03bb-117">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e03bb-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e03bb-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e03bb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e03bb-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e03bb-119">Not supported.</span></span>    |
|<span data-ttu-id="e03bb-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e03bb-120">Application</span></span> | <span data-ttu-id="e03bb-121">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e03bb-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e03bb-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e03bb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e03bb-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e03bb-123">Request headers</span></span>
| <span data-ttu-id="e03bb-124">名前</span><span class="sxs-lookup"><span data-stu-id="e03bb-124">Name</span></span>       | <span data-ttu-id="e03bb-125">種類</span><span class="sxs-lookup"><span data-stu-id="e03bb-125">Type</span></span> | <span data-ttu-id="e03bb-126">説明</span><span class="sxs-lookup"><span data-stu-id="e03bb-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e03bb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e03bb-127">Authorization</span></span>  | <span data-ttu-id="e03bb-128">string</span><span class="sxs-lookup"><span data-stu-id="e03bb-128">string</span></span>  | <span data-ttu-id="e03bb-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e03bb-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e03bb-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e03bb-131">Request body</span></span>
<span data-ttu-id="e03bb-132">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e03bb-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e03bb-133">応答</span><span class="sxs-lookup"><span data-stu-id="e03bb-133">Response</span></span>
<span data-ttu-id="e03bb-p107">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e03bb-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e03bb-136">例</span><span class="sxs-lookup"><span data-stu-id="e03bb-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e03bb-137">要求</span><span class="sxs-lookup"><span data-stu-id="e03bb-137">Request</span></span>
<span data-ttu-id="e03bb-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e03bb-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
<span data-ttu-id="e03bb-139">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e03bb-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="e03bb-140">応答</span><span class="sxs-lookup"><span data-stu-id="e03bb-140">Response</span></span>
<span data-ttu-id="e03bb-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e03bb-141">The following is an example of the response.</span></span>
><span data-ttu-id="e03bb-142">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e03bb-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e03bb-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e03bb-143">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
