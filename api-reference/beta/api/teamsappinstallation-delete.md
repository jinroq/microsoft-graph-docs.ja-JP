---
title: チームからアプリを削除する
description: 指定したチームからアプリをアンインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a970b8e14386ca8c7039a3df3fd1082d39ff750b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931818"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="67235-103">チームからアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="67235-103">Remove app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67235-104">指定した[チーム](../resources/team.md)から[アプリ](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="67235-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67235-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67235-105">Permissions</span></span>

<span data-ttu-id="67235-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67235-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67235-108">Permission type</span></span>      | <span data-ttu-id="67235-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67235-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67235-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67235-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67235-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="67235-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67235-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67235-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67235-113">Not supported.</span></span>    |
|<span data-ttu-id="67235-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67235-114">Application</span></span> | <span data-ttu-id="67235-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67235-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67235-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67235-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="67235-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67235-117">Request headers</span></span>

| <span data-ttu-id="67235-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67235-118">Header</span></span>       | <span data-ttu-id="67235-119">値</span><span class="sxs-lookup"><span data-stu-id="67235-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67235-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="67235-120">Authorization</span></span>  | <span data-ttu-id="67235-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67235-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67235-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="67235-123">Request body</span></span>

<span data-ttu-id="67235-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67235-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67235-125">応答</span><span class="sxs-lookup"><span data-stu-id="67235-125">Response</span></span>

<span data-ttu-id="67235-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="67235-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67235-128">例</span><span class="sxs-lookup"><span data-stu-id="67235-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="67235-129">要求</span><span class="sxs-lookup"><span data-stu-id="67235-129">Request</span></span>

<span data-ttu-id="67235-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67235-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67235-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="67235-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67235-132">C#</span><span class="sxs-lookup"><span data-stu-id="67235-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67235-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="67235-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67235-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="67235-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67235-135">Java</span><span class="sxs-lookup"><span data-stu-id="67235-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67235-136">応答</span><span class="sxs-lookup"><span data-stu-id="67235-136">Response</span></span>

<span data-ttu-id="67235-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67235-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
