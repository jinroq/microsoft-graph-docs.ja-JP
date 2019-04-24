---
title: グループ所有者の追加
description: グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 049c860be95e2f4f4b83848d8d8be6b3dd0ed9c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502162"
---
# <a name="add-group-owner"></a><span data-ttu-id="5e3b3-104">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="5e3b3-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e3b3-p102">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="5e3b3-107">**重要:** グループの所有者を更新し、グループのチームを作成した場合、所有者が Microsoft Teams と同期するには最大2時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="5e3b3-108">また、たとえばプランナープランを作成して所有者がチーム内で変更できるようにする場合は、グループ/チームメンバーとして所有者を追加する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5e3b3-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e3b3-109">Permissions</span></span>
<span data-ttu-id="5e3b3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3b3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e3b3-112">Permission type</span></span>      | <span data-ttu-id="5e3b3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e3b3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e3b3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e3b3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5e3b3-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e3b3-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e3b3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e3b3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e3b3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-117">Not supported.</span></span>    |
|<span data-ttu-id="5e3b3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e3b3-118">Application</span></span> | <span data-ttu-id="5e3b3-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3b3-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e3b3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e3b3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5e3b3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e3b3-121">Request headers</span></span>
| <span data-ttu-id="5e3b3-122">名前</span><span class="sxs-lookup"><span data-stu-id="5e3b3-122">Name</span></span>       | <span data-ttu-id="5e3b3-123">型</span><span class="sxs-lookup"><span data-stu-id="5e3b3-123">Type</span></span> | <span data-ttu-id="5e3b3-124">説明</span><span class="sxs-lookup"><span data-stu-id="5e3b3-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e3b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e3b3-125">Authorization</span></span>  | <span data-ttu-id="5e3b3-126">string</span><span class="sxs-lookup"><span data-stu-id="5e3b3-126">string</span></span>  | <span data-ttu-id="5e3b3-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e3b3-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e3b3-129">Request body</span></span>
<span data-ttu-id="5e3b3-130">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5e3b3-131">応答</span><span class="sxs-lookup"><span data-stu-id="5e3b3-131">Response</span></span>
<span data-ttu-id="5e3b3-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3b3-134">例</span><span class="sxs-lookup"><span data-stu-id="5e3b3-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5e3b3-135">要求</span><span class="sxs-lookup"><span data-stu-id="5e3b3-135">Request</span></span>
<span data-ttu-id="5e3b3-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="5e3b3-137">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="5e3b3-138">応答</span><span class="sxs-lookup"><span data-stu-id="5e3b3-138">Response</span></span>
<span data-ttu-id="5e3b3-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-139">The following is an example of the response.</span></span>
><span data-ttu-id="5e3b3-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e3b3-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5e3b3-141">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
