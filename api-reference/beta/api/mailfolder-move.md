---
title: 'mailFolder: 移動'
description: mailFolder とその内容を別の mailFolder に移動します。
author: angelgolfer-ms
ms.openlocfilehash: 50c982a9c2277530c884ee2807543f858fd3b696
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348756"
---
# <a name="mailfolder-move"></a><span data-ttu-id="efac3-103">mailFolder: 移動</span><span class="sxs-lookup"><span data-stu-id="efac3-103">mailFolder: move</span></span>

> <span data-ttu-id="efac3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="efac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efac3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efac3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efac3-106">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="efac3-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="efac3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="efac3-107">Permissions</span></span>

<span data-ttu-id="efac3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efac3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="efac3-110">Permission type</span></span> | <span data-ttu-id="efac3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="efac3-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="efac3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="efac3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="efac3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efac3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efac3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="efac3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efac3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efac3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efac3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="efac3-116">Application</span></span> | <span data-ttu-id="efac3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efac3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="efac3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="efac3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="efac3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efac3-119">Request headers</span></span>

| <span data-ttu-id="efac3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efac3-120">Header</span></span> | <span data-ttu-id="efac3-121">値</span><span class="sxs-lookup"><span data-stu-id="efac3-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="efac3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efac3-122">Authorization</span></span> | <span data-ttu-id="efac3-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="efac3-123"></span></span> <span data-ttu-id="efac3-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="efac3-124">Required.</span></span> |
| <span data-ttu-id="efac3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efac3-125">Content-Type</span></span> | <span data-ttu-id="efac3-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="efac3-126"></span></span> <span data-ttu-id="efac3-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="efac3-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efac3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="efac3-128">Request body</span></span>

<span data-ttu-id="efac3-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="efac3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="efac3-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="efac3-130">Parameter</span></span> | <span data-ttu-id="efac3-131">種類</span><span class="sxs-lookup"><span data-stu-id="efac3-131">Type</span></span> | <span data-ttu-id="efac3-132">説明</span><span class="sxs-lookup"><span data-stu-id="efac3-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="efac3-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="efac3-133">destinationId</span></span>|<span data-ttu-id="efac3-134">String</span><span class="sxs-lookup"><span data-stu-id="efac3-134">String</span></span>|<span data-ttu-id="efac3-135">フォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="efac3-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="efac3-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efac3-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="efac3-137">応答</span><span class="sxs-lookup"><span data-stu-id="efac3-137">Response</span></span>

<span data-ttu-id="efac3-138">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[mailFolder](../resources/mailfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="efac3-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efac3-139">例</span><span class="sxs-lookup"><span data-stu-id="efac3-139">Example</span></span>

<span data-ttu-id="efac3-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="efac3-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="efac3-141">要求</span><span class="sxs-lookup"><span data-stu-id="efac3-141">Request</span></span>

<span data-ttu-id="efac3-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="efac3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="efac3-143">応答</span><span class="sxs-lookup"><span data-stu-id="efac3-143">Response</span></span>

<span data-ttu-id="efac3-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="efac3-144">Here is an example of the response.</span></span>

> <span data-ttu-id="efac3-145">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="efac3-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="efac3-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="efac3-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->