---
title: グループ所有者の追加
description: グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
ms.openlocfilehash: ac3790ac3a61beb9b5d92916e8dac82f1849cc8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332250"
---
# <a name="add-group-owner"></a><span data-ttu-id="f935f-104">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="f935f-104">Add group owner</span></span>
<span data-ttu-id="f935f-p102">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="f935f-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="f935f-107">**重要な:** グループの所有者を更新すると、グループのチームを作成した、マイクロソフトのチームとの同期に所有者には、最大で 2 時間がかかります。</span><span class="sxs-lookup"><span data-stu-id="f935f-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="f935f-108">また、- たとえば、プランナーの計画を作成するので、チームで変更を加えることができる所有者所有者も必要があります、グループまたはチームのメンバーとして追加します。</span><span class="sxs-lookup"><span data-stu-id="f935f-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f935f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f935f-109">Permissions</span></span>
<span data-ttu-id="f935f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f935f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f935f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f935f-112">Permission type</span></span>      | <span data-ttu-id="f935f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f935f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f935f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f935f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f935f-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f935f-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f935f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f935f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f935f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f935f-117">Not supported.</span></span>    |
|<span data-ttu-id="f935f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f935f-118">Application</span></span> | <span data-ttu-id="f935f-119">Group.ReadWrite.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f935f-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f935f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f935f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f935f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f935f-121">Request headers</span></span>
| <span data-ttu-id="f935f-122">名前</span><span class="sxs-lookup"><span data-stu-id="f935f-122">Name</span></span>       | <span data-ttu-id="f935f-123">種類</span><span class="sxs-lookup"><span data-stu-id="f935f-123">Type</span></span> | <span data-ttu-id="f935f-124">説明</span><span class="sxs-lookup"><span data-stu-id="f935f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f935f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f935f-125">Authorization</span></span>  | <span data-ttu-id="f935f-126">string</span><span class="sxs-lookup"><span data-stu-id="f935f-126">string</span></span>  | <span data-ttu-id="f935f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f935f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f935f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f935f-129">Request body</span></span>
<span data-ttu-id="f935f-130">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f935f-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f935f-131">応答</span><span class="sxs-lookup"><span data-stu-id="f935f-131">Response</span></span>
<span data-ttu-id="f935f-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f935f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f935f-134">例</span><span class="sxs-lookup"><span data-stu-id="f935f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f935f-135">要求</span><span class="sxs-lookup"><span data-stu-id="f935f-135">Request</span></span>
<span data-ttu-id="f935f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f935f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="f935f-137">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f935f-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="f935f-138">応答</span><span class="sxs-lookup"><span data-stu-id="f935f-138">Response</span></span>
<span data-ttu-id="f935f-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f935f-139">The following is an example of the response.</span></span>
><span data-ttu-id="f935f-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f935f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f935f-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f935f-141">All the properties will be returned from an actual call.</span></span>
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

