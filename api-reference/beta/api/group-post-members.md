---
title: メンバーを追加する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: db0261b71f6499489b48deb099a572599b482d38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955528"
---
# <a name="add-member"></a><span data-ttu-id="0c2a6-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="0c2a6-103">Add member</span></span>

> <span data-ttu-id="0c2a6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c2a6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c2a6-106">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-106">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="0c2a6-107">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-107">You can add users or other groups.</span></span> <span data-ttu-id="0c2a6-108">重要: Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-108">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c2a6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c2a6-109">Permissions</span></span>
<span data-ttu-id="0c2a6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c2a6-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c2a6-112">Permission type</span></span>      | <span data-ttu-id="0c2a6-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c2a6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c2a6-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c2a6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0c2a6-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c2a6-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c2a6-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c2a6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c2a6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-117">Not supported.</span></span>    |
|<span data-ttu-id="0c2a6-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c2a6-118">Application</span></span> | <span data-ttu-id="0c2a6-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c2a6-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c2a6-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c2a6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0c2a6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c2a6-121">Request headers</span></span>
| <span data-ttu-id="0c2a6-122">名前</span><span class="sxs-lookup"><span data-stu-id="0c2a6-122">Name</span></span>       | <span data-ttu-id="0c2a6-123">型</span><span class="sxs-lookup"><span data-stu-id="0c2a6-123">Type</span></span> | <span data-ttu-id="0c2a6-124">説明</span><span class="sxs-lookup"><span data-stu-id="0c2a6-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c2a6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2a6-125">Authorization</span></span>  | <span data-ttu-id="0c2a6-126">string</span><span class="sxs-lookup"><span data-stu-id="0c2a6-126">string</span></span>  | <span data-ttu-id="0c2a6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c2a6-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c2a6-129">Request body</span></span>
<span data-ttu-id="0c2a6-130">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="0c2a6-131">応答</span><span class="sxs-lookup"><span data-stu-id="0c2a6-131">Response</span></span>
<span data-ttu-id="0c2a6-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c2a6-134">例</span><span class="sxs-lookup"><span data-stu-id="0c2a6-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0c2a6-135">要求</span><span class="sxs-lookup"><span data-stu-id="0c2a6-135">Request</span></span>
<span data-ttu-id="0c2a6-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="0c2a6-137">要求の本文に指定の JSON 表現、`id`の[directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md)、または[グループ](../resources/group.md)のオブジェクトを追加します。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="0c2a6-138">応答</span><span class="sxs-lookup"><span data-stu-id="0c2a6-138">Response</span></span>
<span data-ttu-id="0c2a6-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-139">The following is an example of the response.</span></span>
><span data-ttu-id="0c2a6-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c2a6-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0c2a6-141">All the properties will be returned from an actual call.</span></span>
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
