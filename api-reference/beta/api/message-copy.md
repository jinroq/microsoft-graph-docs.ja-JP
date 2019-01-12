---
title: 'メッセージ: copy'
description: メッセージをフォルダーにコピーします。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cacc827079089cf977a28f5bb45bb1ac62884275
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934717"
---
# <a name="message-copy"></a><span data-ttu-id="3a5f2-103">メッセージ: copy</span><span class="sxs-lookup"><span data-stu-id="3a5f2-103">message: copy</span></span>

> <span data-ttu-id="3a5f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a5f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a5f2-106">メッセージをフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a5f2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a5f2-107">Permissions</span></span>

<span data-ttu-id="3a5f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a5f2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a5f2-110">Permission type</span></span> | <span data-ttu-id="3a5f2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a5f2-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="3a5f2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a5f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a5f2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5f2-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a5f2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a5f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a5f2-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5f2-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a5f2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a5f2-116">Application</span></span> | <span data-ttu-id="3a5f2-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5f2-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a5f2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a5f2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="3a5f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a5f2-119">Request headers</span></span>

| <span data-ttu-id="3a5f2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a5f2-120">Header</span></span> | <span data-ttu-id="3a5f2-121">値</span><span class="sxs-lookup"><span data-stu-id="3a5f2-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="3a5f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a5f2-122">Authorization</span></span> | <span data-ttu-id="3a5f2-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="3a5f2-123"></span></span> <span data-ttu-id="3a5f2-124">必須。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-124">Required.</span></span> |
| <span data-ttu-id="3a5f2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a5f2-125">Content-Type</span></span> | <span data-ttu-id="3a5f2-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="3a5f2-126"></span></span> <span data-ttu-id="3a5f2-127">必須。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a5f2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a5f2-128">Request body</span></span>

<span data-ttu-id="3a5f2-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a5f2-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a5f2-130">Parameter</span></span> | <span data-ttu-id="3a5f2-131">型</span><span class="sxs-lookup"><span data-stu-id="3a5f2-131">Type</span></span> | <span data-ttu-id="3a5f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="3a5f2-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="3a5f2-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="3a5f2-133">destinationId</span></span>|<span data-ttu-id="3a5f2-134">String</span><span class="sxs-lookup"><span data-stu-id="3a5f2-134">String</span></span>|<span data-ttu-id="3a5f2-135">移動先のフォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="3a5f2-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3a5f2-137">応答</span><span class="sxs-lookup"><span data-stu-id="3a5f2-137">Response</span></span>

<span data-ttu-id="3a5f2-138">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[メッセージ](../resources/message.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a5f2-139">例</span><span class="sxs-lookup"><span data-stu-id="3a5f2-139">Example</span></span>

<span data-ttu-id="3a5f2-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3a5f2-141">要求</span><span class="sxs-lookup"><span data-stu-id="3a5f2-141">Request</span></span>

<span data-ttu-id="3a5f2-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3a5f2-143">応答</span><span class="sxs-lookup"><span data-stu-id="3a5f2-143">Response</span></span>

<span data-ttu-id="3a5f2-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-144">Here is an example of the response.</span></span>

> <span data-ttu-id="3a5f2-145">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a5f2-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3a5f2-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
