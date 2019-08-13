---
title: アプリをチームに追加する
description: 指定したチームにアプリをインストールします。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc5f92212d9fbeb6b061f952ff31c76fcf1f2ce8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375500"
---
# <a name="add-app-to-team"></a><span data-ttu-id="c9217-103">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="c9217-103">Add app to team</span></span>

<span data-ttu-id="c9217-104">指定した[チーム](../resources/team.md)に[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="c9217-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9217-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9217-105">Permissions</span></span>

<span data-ttu-id="c9217-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9217-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9217-108">Permission type</span></span>      | <span data-ttu-id="c9217-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9217-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9217-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9217-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c9217-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9217-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9217-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9217-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9217-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9217-113">Not supported.</span></span>    |
|<span data-ttu-id="c9217-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9217-114">Application</span></span> | <span data-ttu-id="c9217-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9217-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9217-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9217-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="c9217-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9217-117">Request headers</span></span>

| <span data-ttu-id="c9217-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9217-118">Header</span></span>       | <span data-ttu-id="c9217-119">値</span><span class="sxs-lookup"><span data-stu-id="c9217-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9217-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9217-120">Authorization</span></span>  | <span data-ttu-id="c9217-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c9217-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9217-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9217-123">Request body</span></span>

| <span data-ttu-id="c9217-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9217-124">Property</span></span>   | <span data-ttu-id="c9217-125">型</span><span class="sxs-lookup"><span data-stu-id="c9217-125">Type</span></span> |<span data-ttu-id="c9217-126">説明</span><span class="sxs-lookup"><span data-stu-id="c9217-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9217-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c9217-127">teamsApp</span></span>| [<span data-ttu-id="c9217-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c9217-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="c9217-129">追加するアプリ。</span><span class="sxs-lookup"><span data-stu-id="c9217-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="c9217-130">応答</span><span class="sxs-lookup"><span data-stu-id="c9217-130">Response</span></span>

<span data-ttu-id="c9217-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c9217-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9217-133">例</span><span class="sxs-lookup"><span data-stu-id="c9217-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9217-134">要求</span><span class="sxs-lookup"><span data-stu-id="c9217-134">Request</span></span>

<span data-ttu-id="c9217-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9217-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9217-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c9217-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9217-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9217-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9217-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9217-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9217-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="c9217-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9217-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9217-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9217-141">応答</span><span class="sxs-lookup"><span data-stu-id="c9217-141">Response</span></span>

<span data-ttu-id="c9217-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9217-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
