---
title: ユーザーのアプリをアンインストールする
description: 指定したユーザーの個人スコープからアプリをアンインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c6240cc83575b6f7e0a496d161c424f069634b02
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409078"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="f95a2-103">ユーザーのアプリをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="f95a2-103">Uninstall app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f95a2-104">指定した[ユーザー](../resources/user.md)の個人スコープから[アプリ](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="f95a2-104">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f95a2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f95a2-105">Permissions</span></span>

<span data-ttu-id="f95a2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f95a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f95a2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f95a2-108">Permission type</span></span>      | <span data-ttu-id="f95a2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f95a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f95a2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f95a2-110">Delegated (work or school account)</span></span> |<span data-ttu-id="f95a2-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95a2-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f95a2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f95a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f95a2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95a2-113">Not supported.</span></span>    |
|<span data-ttu-id="f95a2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f95a2-114">Application</span></span> | <span data-ttu-id="f95a2-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95a2-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f95a2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f95a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f95a2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95a2-117">Request headers</span></span>

| <span data-ttu-id="f95a2-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95a2-118">Header</span></span>       | <span data-ttu-id="f95a2-119">値</span><span class="sxs-lookup"><span data-stu-id="f95a2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f95a2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f95a2-120">Authorization</span></span>  | <span data-ttu-id="f95a2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f95a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f95a2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f95a2-123">Request body</span></span>

<span data-ttu-id="f95a2-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f95a2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f95a2-125">応答</span><span class="sxs-lookup"><span data-stu-id="f95a2-125">Response</span></span>

<span data-ttu-id="f95a2-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f95a2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95a2-128">例</span><span class="sxs-lookup"><span data-stu-id="f95a2-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f95a2-129">要求</span><span class="sxs-lookup"><span data-stu-id="f95a2-129">Request</span></span>

<span data-ttu-id="f95a2-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f95a2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f95a2-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f95a2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f95a2-132">C#</span><span class="sxs-lookup"><span data-stu-id="f95a2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f95a2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f95a2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f95a2-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="f95a2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f95a2-135">応答</span><span class="sxs-lookup"><span data-stu-id="f95a2-135">Response</span></span>

<span data-ttu-id="f95a2-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f95a2-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
