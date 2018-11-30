---
title: SynchronizationSchema を削除します。
description: カスタマイズされたスキーマを削除し、スキーマがデフォルト設定にリセットします。 テンプレートのコンテキストでは、スキーマが削除されると、リセット、スキーマとテンプレートのいずれかに関連付けられた既定値に`factoryTag`。
ms.openlocfilehash: 81c1a918b10e8f4553b3e99312f20bb538bfbe4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072487"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="e0405-104">SynchronizationSchema を削除します。</span><span class="sxs-lookup"><span data-stu-id="e0405-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="e0405-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0405-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0405-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0405-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0405-107">カスタマイズされたスキーマを削除し、スキーマがデフォルト設定にリセットします。</span><span class="sxs-lookup"><span data-stu-id="e0405-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="e0405-108">テンプレートのコンテキストでは、スキーマが削除されると、リセット、スキーマとテンプレートのいずれかに関連付けられた既定値に`factoryTag`。</span><span class="sxs-lookup"><span data-stu-id="e0405-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0405-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e0405-109">Permissions</span></span>
<span data-ttu-id="e0405-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0405-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0405-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0405-112">Permission type</span></span>                        | <span data-ttu-id="e0405-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0405-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0405-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0405-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="e0405-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0405-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e0405-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0405-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e0405-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0405-117">Not supported.</span></span>|
|<span data-ttu-id="e0405-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0405-118">Application</span></span>                            |<span data-ttu-id="e0405-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0405-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e0405-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0405-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e0405-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0405-121">Request headers</span></span>

| <span data-ttu-id="e0405-122">名前</span><span class="sxs-lookup"><span data-stu-id="e0405-122">Name</span></span>           | <span data-ttu-id="e0405-123">型</span><span class="sxs-lookup"><span data-stu-id="e0405-123">Type</span></span>    | <span data-ttu-id="e0405-124">説明</span><span class="sxs-lookup"><span data-stu-id="e0405-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e0405-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0405-125">Authorization</span></span>  | <span data-ttu-id="e0405-126">string</span><span class="sxs-lookup"><span data-stu-id="e0405-126">string</span></span>  | <span data-ttu-id="e0405-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e0405-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0405-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0405-129">Request body</span></span>

<span data-ttu-id="e0405-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e0405-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0405-131">応答</span><span class="sxs-lookup"><span data-stu-id="e0405-131">Response</span></span>

<span data-ttu-id="e0405-132">成功した場合、このメソッドは `201 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e0405-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="e0405-133">応答の本文に何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="e0405-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0405-134">例</span><span class="sxs-lookup"><span data-stu-id="e0405-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e0405-135">要求</span><span class="sxs-lookup"><span data-stu-id="e0405-135">Request</span></span>
<span data-ttu-id="e0405-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0405-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="e0405-137">応答</span><span class="sxs-lookup"><span data-stu-id="e0405-137">Response</span></span>
<span data-ttu-id="e0405-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0405-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->