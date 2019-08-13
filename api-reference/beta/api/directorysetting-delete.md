---
title: ディレクトリ設定を削除する
description: ディレクトリ設定を削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6821861196a923c73d44e3e5c5a70c0eda15d03e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319469"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="c942b-103">ディレクトリ設定を削除する</span><span class="sxs-lookup"><span data-stu-id="c942b-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c942b-104">ディレクトリ設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="c942b-104">Delete a directory setting.</span></span>

> <span data-ttu-id="c942b-105">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="c942b-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="c942b-106">この API の/v1.0 バージョンは、 *groupSettings を削除*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="c942b-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="c942b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c942b-107">Permissions</span></span>
<span data-ttu-id="c942b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c942b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c942b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c942b-110">Permission type</span></span>      | <span data-ttu-id="c942b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c942b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c942b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c942b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c942b-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c942b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c942b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c942b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c942b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c942b-115">Not supported.</span></span>    |
|<span data-ttu-id="c942b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c942b-116">Application</span></span> | <span data-ttu-id="c942b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c942b-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c942b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c942b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c942b-119">特定のテナント全体またはグループ設定を削除する</span><span class="sxs-lookup"><span data-stu-id="c942b-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c942b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c942b-120">Request headers</span></span>
| <span data-ttu-id="c942b-121">名前</span><span class="sxs-lookup"><span data-stu-id="c942b-121">Name</span></span>       | <span data-ttu-id="c942b-122">説明</span><span class="sxs-lookup"><span data-stu-id="c942b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c942b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c942b-123">Authorization</span></span>  | <span data-ttu-id="c942b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c942b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c942b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c942b-126">Request body</span></span>
<span data-ttu-id="c942b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c942b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c942b-128">応答</span><span class="sxs-lookup"><span data-stu-id="c942b-128">Response</span></span>

<span data-ttu-id="c942b-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c942b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c942b-131">例</span><span class="sxs-lookup"><span data-stu-id="c942b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c942b-132">要求</span><span class="sxs-lookup"><span data-stu-id="c942b-132">Request</span></span>
<span data-ttu-id="c942b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c942b-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c942b-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c942b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c942b-135">C#</span><span class="sxs-lookup"><span data-stu-id="c942b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c942b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c942b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c942b-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="c942b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c942b-138">Java</span><span class="sxs-lookup"><span data-stu-id="c942b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c942b-139">応答</span><span class="sxs-lookup"><span data-stu-id="c942b-139">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
