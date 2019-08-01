---
title: チーム内のアプリをアップグレードする
description: チーム内のアプリのインストールをアップグレードする
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8525ae7afa33f34d3630a8b5fbac53b3d89dedbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027280"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="64249-103">チーム内のアプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="64249-103">Upgrade an app in a team</span></span>

<span data-ttu-id="64249-104">[チーム](../resources/team.md)内の[アプリのインストール](../resources/teamsappinstallation.md)をアプリの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="64249-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="64249-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="64249-105">Permissions</span></span>

<span data-ttu-id="64249-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64249-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64249-108">Permission type</span></span>      | <span data-ttu-id="64249-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="64249-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64249-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64249-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64249-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64249-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64249-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64249-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64249-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64249-113">Not supported.</span></span>    |
|<span data-ttu-id="64249-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64249-114">Application</span></span> | <span data-ttu-id="64249-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64249-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="64249-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64249-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="64249-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64249-117">Request headers</span></span>

| <span data-ttu-id="64249-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64249-118">Header</span></span>       | <span data-ttu-id="64249-119">値</span><span class="sxs-lookup"><span data-stu-id="64249-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64249-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="64249-120">Authorization</span></span>  | <span data-ttu-id="64249-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="64249-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64249-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="64249-123">Request body</span></span>

<span data-ttu-id="64249-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="64249-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64249-125">応答</span><span class="sxs-lookup"><span data-stu-id="64249-125">Response</span></span>

<span data-ttu-id="64249-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="64249-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64249-128">例</span><span class="sxs-lookup"><span data-stu-id="64249-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="64249-129">要求</span><span class="sxs-lookup"><span data-stu-id="64249-129">Request</span></span>

<span data-ttu-id="64249-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64249-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64249-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="64249-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64249-132">C#</span><span class="sxs-lookup"><span data-stu-id="64249-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64249-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="64249-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64249-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="64249-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64249-135">Java</span><span class="sxs-lookup"><span data-stu-id="64249-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64249-136">応答</span><span class="sxs-lookup"><span data-stu-id="64249-136">Response</span></span>

<span data-ttu-id="64249-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64249-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
