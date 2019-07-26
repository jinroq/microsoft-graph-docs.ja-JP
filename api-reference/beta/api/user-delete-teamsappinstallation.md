---
title: ユーザーのアプリをアンインストールする
description: 指定したユーザーの個人スコープからアプリをアンインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 42030378f3d66c11d1d9f8d8856739c54508c302
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908531"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="181f9-103">ユーザーのアプリをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="181f9-103">Uninstall app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="181f9-104">指定した[ユーザー](../resources/user.md)の個人スコープから[アプリ](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="181f9-104">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="181f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="181f9-105">Permissions</span></span>

<span data-ttu-id="181f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="181f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="181f9-108">Permission type</span></span>      | <span data-ttu-id="181f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="181f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="181f9-110">Delegated (work or school account)</span></span> |<span data-ttu-id="181f9-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181f9-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="181f9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="181f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181f9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="181f9-113">Not supported.</span></span>    |
|<span data-ttu-id="181f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="181f9-114">Application</span></span> | <span data-ttu-id="181f9-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181f9-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="181f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="181f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="181f9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="181f9-117">Request headers</span></span>

| <span data-ttu-id="181f9-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="181f9-118">Header</span></span>       | <span data-ttu-id="181f9-119">値</span><span class="sxs-lookup"><span data-stu-id="181f9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="181f9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="181f9-120">Authorization</span></span>  | <span data-ttu-id="181f9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="181f9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="181f9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="181f9-123">Request body</span></span>

<span data-ttu-id="181f9-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="181f9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181f9-125">応答</span><span class="sxs-lookup"><span data-stu-id="181f9-125">Response</span></span>

<span data-ttu-id="181f9-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="181f9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181f9-128">例</span><span class="sxs-lookup"><span data-stu-id="181f9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="181f9-129">要求</span><span class="sxs-lookup"><span data-stu-id="181f9-129">Request</span></span>

<span data-ttu-id="181f9-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="181f9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```

### <a name="response"></a><span data-ttu-id="181f9-131">応答</span><span class="sxs-lookup"><span data-stu-id="181f9-131">Response</span></span>

<span data-ttu-id="181f9-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="181f9-132">The following is an example of the response.</span></span>

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
