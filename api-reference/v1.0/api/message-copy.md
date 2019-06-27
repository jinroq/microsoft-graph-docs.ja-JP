---
title: 'メッセージ: copy'
description: メッセージをフォルダーにコピーします。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2be9d62a8c5b44736612330ebb56fd3f13149e4c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274915"
---
# <a name="message-copy"></a><span data-ttu-id="41e3a-103">メッセージ: copy</span><span class="sxs-lookup"><span data-stu-id="41e3a-103">message: copy</span></span>

<span data-ttu-id="41e3a-104">メッセージをフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="41e3a-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="41e3a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41e3a-105">Permissions</span></span>

<span data-ttu-id="41e3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41e3a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41e3a-108">Permission type</span></span> | <span data-ttu-id="41e3a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41e3a-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="41e3a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41e3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41e3a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41e3a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="41e3a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41e3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e3a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41e3a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="41e3a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41e3a-114">Application</span></span> | <span data-ttu-id="41e3a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41e3a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="41e3a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41e3a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="41e3a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41e3a-117">Request headers</span></span>

| <span data-ttu-id="41e3a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41e3a-118">Header</span></span> | <span data-ttu-id="41e3a-119">値</span><span class="sxs-lookup"><span data-stu-id="41e3a-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="41e3a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e3a-120">Authorization</span></span> | <span data-ttu-id="41e3a-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="41e3a-121"></span></span> <span data-ttu-id="41e3a-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-122">Required.</span></span> |
| <span data-ttu-id="41e3a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41e3a-123">Content-Type</span></span> | <span data-ttu-id="41e3a-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="41e3a-124"></span></span> <span data-ttu-id="41e3a-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41e3a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="41e3a-126">Request body</span></span>

<span data-ttu-id="41e3a-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="41e3a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="41e3a-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="41e3a-128">Parameter</span></span> | <span data-ttu-id="41e3a-129">型</span><span class="sxs-lookup"><span data-stu-id="41e3a-129">Type</span></span> | <span data-ttu-id="41e3a-130">説明</span><span class="sxs-lookup"><span data-stu-id="41e3a-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="41e3a-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="41e3a-131">destinationId</span></span>|<span data-ttu-id="41e3a-132">String</span><span class="sxs-lookup"><span data-stu-id="41e3a-132">String</span></span>|<span data-ttu-id="41e3a-133">宛先フォルダーの ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="41e3a-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e3a-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="41e3a-135">応答</span><span class="sxs-lookup"><span data-stu-id="41e3a-135">Response</span></span>

<span data-ttu-id="41e3a-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="41e3a-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e3a-137">例</span><span class="sxs-lookup"><span data-stu-id="41e3a-137">Example</span></span>

<span data-ttu-id="41e3a-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="41e3a-139">要求</span><span class="sxs-lookup"><span data-stu-id="41e3a-139">Request</span></span>
<span data-ttu-id="41e3a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="41e3a-141">応答</span><span class="sxs-lookup"><span data-stu-id="41e3a-141">Response</span></span>

<span data-ttu-id="41e3a-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="41e3a-142">Here is an example of the response.</span></span>

> <span data-ttu-id="41e3a-143">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="41e3a-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41e3a-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="41e3a-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41e3a-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="41e3a-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41e3a-146">C#</span><span class="sxs-lookup"><span data-stu-id="41e3a-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_copy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41e3a-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="41e3a-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_copy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="41e3a-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="41e3a-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_copy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
