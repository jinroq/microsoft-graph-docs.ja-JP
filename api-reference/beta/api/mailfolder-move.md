---
title: 'mailFolder: 移動'
description: mailFolder とその内容を別の mailFolder に移動します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a654dbfb32539abee990fb8e1cf2da5166163afa
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598670"
---
# <a name="mailfolder-move"></a><span data-ttu-id="50d89-103">mailFolder: 移動</span><span class="sxs-lookup"><span data-stu-id="50d89-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d89-104">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="50d89-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="50d89-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50d89-105">Permissions</span></span>

<span data-ttu-id="50d89-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50d89-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50d89-108">Permission type</span></span> | <span data-ttu-id="50d89-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50d89-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="50d89-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50d89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50d89-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d89-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50d89-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50d89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50d89-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d89-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50d89-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50d89-114">Application</span></span> | <span data-ttu-id="50d89-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d89-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50d89-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50d89-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="50d89-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50d89-117">Request headers</span></span>

| <span data-ttu-id="50d89-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50d89-118">Header</span></span> | <span data-ttu-id="50d89-119">値</span><span class="sxs-lookup"><span data-stu-id="50d89-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="50d89-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d89-120">Authorization</span></span> | <span data-ttu-id="50d89-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="50d89-121"></span></span> <span data-ttu-id="50d89-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="50d89-122">Required.</span></span> |
| <span data-ttu-id="50d89-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50d89-123">Content-Type</span></span> | <span data-ttu-id="50d89-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="50d89-124"></span></span> <span data-ttu-id="50d89-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="50d89-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50d89-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50d89-126">Request body</span></span>

<span data-ttu-id="50d89-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="50d89-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50d89-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="50d89-128">Parameter</span></span> | <span data-ttu-id="50d89-129">型</span><span class="sxs-lookup"><span data-stu-id="50d89-129">Type</span></span> | <span data-ttu-id="50d89-130">説明</span><span class="sxs-lookup"><span data-stu-id="50d89-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="50d89-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="50d89-131">destinationId</span></span>|<span data-ttu-id="50d89-132">String</span><span class="sxs-lookup"><span data-stu-id="50d89-132">String</span></span>|<span data-ttu-id="50d89-133">フォルダー ID、またはよく知られているフォルダー名。</span><span class="sxs-lookup"><span data-stu-id="50d89-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="50d89-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50d89-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="50d89-135">応答</span><span class="sxs-lookup"><span data-stu-id="50d89-135">Response</span></span>

<span data-ttu-id="50d89-136">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50d89-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d89-137">例</span><span class="sxs-lookup"><span data-stu-id="50d89-137">Example</span></span>

<span data-ttu-id="50d89-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="50d89-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50d89-139">要求</span><span class="sxs-lookup"><span data-stu-id="50d89-139">Request</span></span>

<span data-ttu-id="50d89-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50d89-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="50d89-141">応答</span><span class="sxs-lookup"><span data-stu-id="50d89-141">Response</span></span>

<span data-ttu-id="50d89-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="50d89-142">Here is an example of the response.</span></span>

> <span data-ttu-id="50d89-143">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="50d89-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50d89-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50d89-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="50d89-145">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="50d89-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50d89-146">Visual</span><span class="sxs-lookup"><span data-stu-id="50d89-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/mailfolder_move-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50d89-147">Java</span><span class="sxs-lookup"><span data-stu-id="50d89-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/mailfolder_move-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
