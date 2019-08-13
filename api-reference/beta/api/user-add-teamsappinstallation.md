---
title: ユーザー用のアプリをインストールする
description: 指定したユーザーの個人スコープにアプリをインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05d93658f00310f901977f18b79e234275221c10
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362585"
---
# <a name="install-app-for-user"></a><span data-ttu-id="b8674-103">ユーザー用のアプリをインストールする</span><span class="sxs-lookup"><span data-stu-id="b8674-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8674-104">指定した[ユーザー](../resources/user.md)の個人スコープに[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="b8674-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8674-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8674-105">Permissions</span></span>

<span data-ttu-id="b8674-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8674-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8674-108">Permission type</span></span>      | <span data-ttu-id="b8674-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8674-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8674-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8674-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8674-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8674-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="b8674-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8674-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8674-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8674-113">Not supported.</span></span>    |
|<span data-ttu-id="b8674-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8674-114">Application</span></span> | <span data-ttu-id="b8674-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8674-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8674-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8674-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b8674-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8674-117">Request headers</span></span>

| <span data-ttu-id="b8674-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8674-118">Header</span></span>       | <span data-ttu-id="b8674-119">値</span><span class="sxs-lookup"><span data-stu-id="b8674-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8674-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8674-120">Authorization</span></span>  | <span data-ttu-id="b8674-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8674-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8674-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8674-123">Request body</span></span>

<span data-ttu-id="b8674-124">要求本文には、追加する既存のカタログアプリの ID が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8674-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="b8674-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8674-125">Property</span></span>   | <span data-ttu-id="b8674-126">型</span><span class="sxs-lookup"><span data-stu-id="b8674-126">Type</span></span> |<span data-ttu-id="b8674-127">説明</span><span class="sxs-lookup"><span data-stu-id="b8674-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8674-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b8674-128">teamsApp</span></span>|<span data-ttu-id="b8674-129">String</span><span class="sxs-lookup"><span data-stu-id="b8674-129">String</span></span>|<span data-ttu-id="b8674-130">追加するアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="b8674-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="b8674-131">応答</span><span class="sxs-lookup"><span data-stu-id="b8674-131">Response</span></span>

<span data-ttu-id="b8674-p103">成功した場合、このメソッドは `201 Created` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b8674-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8674-134">例</span><span class="sxs-lookup"><span data-stu-id="b8674-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8674-135">要求</span><span class="sxs-lookup"><span data-stu-id="b8674-135">Request</span></span>

<span data-ttu-id="b8674-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8674-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8674-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b8674-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8674-138">C#</span><span class="sxs-lookup"><span data-stu-id="b8674-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8674-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8674-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8674-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="b8674-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8674-141">Java</span><span class="sxs-lookup"><span data-stu-id="b8674-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8674-142">応答</span><span class="sxs-lookup"><span data-stu-id="b8674-142">Response</span></span>

<span data-ttu-id="b8674-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8674-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
