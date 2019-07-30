---
title: 'teamsAppInstallation: アップグレード'
description: ユーザーの個人スコープでアプリのインストールをアップグレードする
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 07a35e03b28787016f2aa90a2921b3922be4a257
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931214"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="1e4a2-103">teamsAppInstallation: アップグレード</span><span class="sxs-lookup"><span data-stu-id="1e4a2-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e4a2-104">指定した[ユーザー](../resources/user.md)の個人用スコープ内の[アプリのインストール](../resources/teamsappinstallation.md)をアプリの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e4a2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e4a2-105">Permissions</span></span>

<span data-ttu-id="1e4a2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4a2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e4a2-108">Permission type</span></span>      | <span data-ttu-id="1e4a2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e4a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e4a2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e4a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e4a2-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4a2-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="1e4a2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e4a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4a2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-113">Not supported.</span></span>    |
|<span data-ttu-id="1e4a2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e4a2-114">Application</span></span> | <span data-ttu-id="1e4a2-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4a2-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e4a2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e4a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="1e4a2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e4a2-117">Request headers</span></span>

| <span data-ttu-id="1e4a2-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e4a2-118">Header</span></span>       | <span data-ttu-id="1e4a2-119">値</span><span class="sxs-lookup"><span data-stu-id="1e4a2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e4a2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e4a2-120">Authorization</span></span>  | <span data-ttu-id="1e4a2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e4a2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e4a2-123">Request body</span></span>

<span data-ttu-id="1e4a2-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e4a2-125">応答</span><span class="sxs-lookup"><span data-stu-id="1e4a2-125">Response</span></span>

<span data-ttu-id="1e4a2-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4a2-128">例</span><span class="sxs-lookup"><span data-stu-id="1e4a2-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e4a2-129">要求</span><span class="sxs-lookup"><span data-stu-id="1e4a2-129">Request</span></span>

<span data-ttu-id="1e4a2-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1e4a2-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e4a2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e4a2-132">C#</span><span class="sxs-lookup"><span data-stu-id="1e4a2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e4a2-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e4a2-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e4a2-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e4a2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e4a2-135">Java</span><span class="sxs-lookup"><span data-stu-id="1e4a2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e4a2-136">応答</span><span class="sxs-lookup"><span data-stu-id="1e4a2-136">Response</span></span>

<span data-ttu-id="1e4a2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e4a2-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
