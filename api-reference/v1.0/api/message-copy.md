---
title: 'メッセージ: copy'
description: メッセージをフォルダーにコピーします。
ms.openlocfilehash: 0883c847030eaf72f96a0ca4665bf002feba8ca2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024231"
---
# <a name="message-copy"></a><span data-ttu-id="332fb-103">メッセージ: copy</span><span class="sxs-lookup"><span data-stu-id="332fb-103">message: copy</span></span>

<span data-ttu-id="332fb-104">メッセージをフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="332fb-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="332fb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="332fb-105">Permissions</span></span>

<span data-ttu-id="332fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="332fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="332fb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="332fb-108">Permission type</span></span> | <span data-ttu-id="332fb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="332fb-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="332fb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="332fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="332fb-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="332fb-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="332fb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="332fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="332fb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="332fb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="332fb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="332fb-114">Application</span></span> | <span data-ttu-id="332fb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="332fb-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="332fb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="332fb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="332fb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="332fb-117">Request headers</span></span>

| <span data-ttu-id="332fb-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="332fb-118">Header</span></span> | <span data-ttu-id="332fb-119">値</span><span class="sxs-lookup"><span data-stu-id="332fb-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="332fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="332fb-120">Authorization</span></span> | <span data-ttu-id="332fb-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="332fb-121"></span></span> <span data-ttu-id="332fb-122">必須。</span><span class="sxs-lookup"><span data-stu-id="332fb-122">Required.</span></span> |
| <span data-ttu-id="332fb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="332fb-123">Content-Type</span></span> | <span data-ttu-id="332fb-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="332fb-124"></span></span> <span data-ttu-id="332fb-125">必須。</span><span class="sxs-lookup"><span data-stu-id="332fb-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="332fb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="332fb-126">Request body</span></span>

<span data-ttu-id="332fb-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="332fb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="332fb-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="332fb-128">Parameter</span></span> | <span data-ttu-id="332fb-129">型</span><span class="sxs-lookup"><span data-stu-id="332fb-129">Type</span></span> | <span data-ttu-id="332fb-130">説明</span><span class="sxs-lookup"><span data-stu-id="332fb-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="332fb-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="332fb-131">destinationId</span></span>|<span data-ttu-id="332fb-132">String</span><span class="sxs-lookup"><span data-stu-id="332fb-132">String</span></span>|<span data-ttu-id="332fb-133">移動先のフォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="332fb-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="332fb-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="332fb-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="332fb-135">応答</span><span class="sxs-lookup"><span data-stu-id="332fb-135">Response</span></span>

<span data-ttu-id="332fb-136">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[メッセージ](../resources/message.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="332fb-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="332fb-137">例</span><span class="sxs-lookup"><span data-stu-id="332fb-137">Example</span></span>

<span data-ttu-id="332fb-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="332fb-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="332fb-139">要求</span><span class="sxs-lookup"><span data-stu-id="332fb-139">Request</span></span>
<span data-ttu-id="332fb-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="332fb-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="332fb-141">応答</span><span class="sxs-lookup"><span data-stu-id="332fb-141">Response</span></span>

<span data-ttu-id="332fb-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="332fb-142">Here is an example of the response.</span></span>

> <span data-ttu-id="332fb-143">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="332fb-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="332fb-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="332fb-144">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
