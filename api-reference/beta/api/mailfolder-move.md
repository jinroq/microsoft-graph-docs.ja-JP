---
title: 'mailFolder: 移動'
description: mailFolder とその内容を別の mailFolder に移動します。
ms.openlocfilehash: 8aeef43068bcd2f23df5d726e559d0c8268ae1ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073862"
---
# <a name="mailfolder-move"></a><span data-ttu-id="216c0-103">mailFolder: 移動</span><span class="sxs-lookup"><span data-stu-id="216c0-103">mailFolder: move</span></span>

> <span data-ttu-id="216c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="216c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="216c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="216c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="216c0-106">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="216c0-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="216c0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="216c0-107">Permissions</span></span>

<span data-ttu-id="216c0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="216c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="216c0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="216c0-110">Permission type</span></span> | <span data-ttu-id="216c0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="216c0-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="216c0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="216c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="216c0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="216c0-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="216c0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="216c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="216c0-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="216c0-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="216c0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="216c0-116">Application</span></span> | <span data-ttu-id="216c0-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="216c0-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="216c0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="216c0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="216c0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="216c0-119">Request headers</span></span>

| <span data-ttu-id="216c0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="216c0-120">Header</span></span> | <span data-ttu-id="216c0-121">値</span><span class="sxs-lookup"><span data-stu-id="216c0-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="216c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="216c0-122">Authorization</span></span> | <span data-ttu-id="216c0-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="216c0-123"></span></span> <span data-ttu-id="216c0-124">必須。</span><span class="sxs-lookup"><span data-stu-id="216c0-124">Required.</span></span> |
| <span data-ttu-id="216c0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="216c0-125">Content-Type</span></span> | <span data-ttu-id="216c0-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="216c0-126"></span></span> <span data-ttu-id="216c0-127">必須。</span><span class="sxs-lookup"><span data-stu-id="216c0-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="216c0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="216c0-128">Request body</span></span>

<span data-ttu-id="216c0-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="216c0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="216c0-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="216c0-130">Parameter</span></span> | <span data-ttu-id="216c0-131">型</span><span class="sxs-lookup"><span data-stu-id="216c0-131">Type</span></span> | <span data-ttu-id="216c0-132">説明</span><span class="sxs-lookup"><span data-stu-id="216c0-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="216c0-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="216c0-133">destinationId</span></span>|<span data-ttu-id="216c0-134">String</span><span class="sxs-lookup"><span data-stu-id="216c0-134">String</span></span>|<span data-ttu-id="216c0-135">フォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="216c0-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="216c0-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="216c0-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="216c0-137">応答</span><span class="sxs-lookup"><span data-stu-id="216c0-137">Response</span></span>

<span data-ttu-id="216c0-138">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[mailFolder](../resources/mailfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="216c0-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="216c0-139">例</span><span class="sxs-lookup"><span data-stu-id="216c0-139">Example</span></span>

<span data-ttu-id="216c0-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="216c0-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="216c0-141">要求</span><span class="sxs-lookup"><span data-stu-id="216c0-141">Request</span></span>

<span data-ttu-id="216c0-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="216c0-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="216c0-143">応答</span><span class="sxs-lookup"><span data-stu-id="216c0-143">Response</span></span>

<span data-ttu-id="216c0-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="216c0-144">Here is an example of the response.</span></span>

> <span data-ttu-id="216c0-145">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="216c0-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="216c0-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="216c0-146">All the properties will be returned from an actual call.</span></span>
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
