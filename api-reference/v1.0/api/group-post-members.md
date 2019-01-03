---
title: メンバーを追加する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。
ms.openlocfilehash: 1fe2d5c259b4e1974168df30e282d97d3342e0bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022158"
---
# <a name="add-member"></a><span data-ttu-id="9927c-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="9927c-103">Add member</span></span>
<span data-ttu-id="9927c-104">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="9927c-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="9927c-105">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="9927c-105">You can add users or other groups.</span></span> <span data-ttu-id="9927c-106">重要: Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="9927c-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="9927c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9927c-107">Permissions</span></span>
<span data-ttu-id="9927c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9927c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9927c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9927c-110">Permission type</span></span>      | <span data-ttu-id="9927c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9927c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9927c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9927c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9927c-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9927c-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9927c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9927c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9927c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9927c-115">Not supported.</span></span>    |
|<span data-ttu-id="9927c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9927c-116">Application</span></span> | <span data-ttu-id="9927c-117">Group.ReadWrite.All と Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9927c-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9927c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9927c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9927c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9927c-119">Request headers</span></span>
| <span data-ttu-id="9927c-120">名前</span><span class="sxs-lookup"><span data-stu-id="9927c-120">Name</span></span>       | <span data-ttu-id="9927c-121">型</span><span class="sxs-lookup"><span data-stu-id="9927c-121">Type</span></span> | <span data-ttu-id="9927c-122">説明</span><span class="sxs-lookup"><span data-stu-id="9927c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9927c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9927c-123">Authorization</span></span>  | <span data-ttu-id="9927c-124">string</span><span class="sxs-lookup"><span data-stu-id="9927c-124">string</span></span>  | <span data-ttu-id="9927c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9927c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9927c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9927c-127">Request body</span></span>
<span data-ttu-id="9927c-128">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9927c-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9927c-129">応答</span><span class="sxs-lookup"><span data-stu-id="9927c-129">Response</span></span>
<span data-ttu-id="9927c-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9927c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9927c-132">例</span><span class="sxs-lookup"><span data-stu-id="9927c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9927c-133">要求</span><span class="sxs-lookup"><span data-stu-id="9927c-133">Request</span></span>
<span data-ttu-id="9927c-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9927c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="9927c-135">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9927c-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="9927c-136">応答</span><span class="sxs-lookup"><span data-stu-id="9927c-136">Response</span></span>
<span data-ttu-id="9927c-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9927c-137">The following is an example of the response.</span></span>
><span data-ttu-id="9927c-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9927c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9927c-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9927c-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->