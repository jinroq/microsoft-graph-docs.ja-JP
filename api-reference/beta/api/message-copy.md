---
title: 'メッセージ: copy'
description: メッセージをフォルダーにコピーします。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 02cde8f2854e9a32210534e8c127c7c3d7dc6e86
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879799"
---
# <a name="message-copy"></a><span data-ttu-id="ef47c-103">メッセージ: copy</span><span class="sxs-lookup"><span data-stu-id="ef47c-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef47c-104">メッセージをフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="ef47c-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef47c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ef47c-105">Permissions</span></span>

<span data-ttu-id="ef47c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef47c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef47c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef47c-108">Permission type</span></span> | <span data-ttu-id="ef47c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef47c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ef47c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef47c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef47c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef47c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ef47c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef47c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef47c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef47c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ef47c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef47c-114">Application</span></span> | <span data-ttu-id="ef47c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef47c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef47c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef47c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="ef47c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef47c-117">Request headers</span></span>

| <span data-ttu-id="ef47c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef47c-118">Header</span></span> | <span data-ttu-id="ef47c-119">値</span><span class="sxs-lookup"><span data-stu-id="ef47c-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ef47c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef47c-120">Authorization</span></span> | <span data-ttu-id="ef47c-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ef47c-121"></span></span> <span data-ttu-id="ef47c-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-122">Required.</span></span> |
| <span data-ttu-id="ef47c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef47c-123">Content-Type</span></span> | <span data-ttu-id="ef47c-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ef47c-124"></span></span> <span data-ttu-id="ef47c-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef47c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef47c-126">Request body</span></span>

<span data-ttu-id="ef47c-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ef47c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ef47c-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ef47c-128">Parameter</span></span> | <span data-ttu-id="ef47c-129">型</span><span class="sxs-lookup"><span data-stu-id="ef47c-129">Type</span></span> | <span data-ttu-id="ef47c-130">説明</span><span class="sxs-lookup"><span data-stu-id="ef47c-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ef47c-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="ef47c-131">destinationId</span></span>|<span data-ttu-id="ef47c-132">String</span><span class="sxs-lookup"><span data-stu-id="ef47c-132">String</span></span>|<span data-ttu-id="ef47c-133">宛先フォルダーの ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ef47c-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef47c-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ef47c-135">応答</span><span class="sxs-lookup"><span data-stu-id="ef47c-135">Response</span></span>

<span data-ttu-id="ef47c-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="ef47c-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef47c-137">例</span><span class="sxs-lookup"><span data-stu-id="ef47c-137">Example</span></span>

<span data-ttu-id="ef47c-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ef47c-139">要求</span><span class="sxs-lookup"><span data-stu-id="ef47c-139">Request</span></span>

<span data-ttu-id="ef47c-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef47c-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ef47c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef47c-142">C#</span><span class="sxs-lookup"><span data-stu-id="ef47c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef47c-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef47c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef47c-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="ef47c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef47c-145">Java</span><span class="sxs-lookup"><span data-stu-id="ef47c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef47c-146">応答</span><span class="sxs-lookup"><span data-stu-id="ef47c-146">Response</span></span>

<span data-ttu-id="ef47c-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ef47c-147">Here is an example of the response.</span></span>

> <span data-ttu-id="ef47c-148">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ef47c-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef47c-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ef47c-149">All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
