---
title: 'mailFolder: コピー'
description: mailFolder とその内容を別の mailFolder にコピーします。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c19903977cb90b119e21fbc4cad944afd87ea1fc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598134"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="d5c62-103">mailFolder: コピー</span><span class="sxs-lookup"><span data-stu-id="d5c62-103">mailFolder: copy</span></span>

<span data-ttu-id="d5c62-104">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="d5c62-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c62-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5c62-105">Permissions</span></span>

<span data-ttu-id="d5c62-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5c62-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5c62-108">Permission type</span></span> | <span data-ttu-id="d5c62-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5c62-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d5c62-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5c62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5c62-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c62-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d5c62-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5c62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c62-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c62-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d5c62-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5c62-114">Application</span></span> | <span data-ttu-id="d5c62-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c62-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c62-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5c62-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="d5c62-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5c62-117">Request headers</span></span>
| <span data-ttu-id="d5c62-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5c62-118">Header</span></span> | <span data-ttu-id="d5c62-119">値</span><span class="sxs-lookup"><span data-stu-id="d5c62-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d5c62-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c62-120">Authorization</span></span> | <span data-ttu-id="d5c62-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d5c62-121"></span></span> <span data-ttu-id="d5c62-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="d5c62-122">Required.</span></span> |
| <span data-ttu-id="d5c62-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5c62-123">Content-Type</span></span> | <span data-ttu-id="d5c62-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d5c62-124"></span></span> <span data-ttu-id="d5c62-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="d5c62-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5c62-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5c62-126">Request body</span></span>

<span data-ttu-id="d5c62-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d5c62-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5c62-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d5c62-128">Parameter</span></span> | <span data-ttu-id="d5c62-129">型</span><span class="sxs-lookup"><span data-stu-id="d5c62-129">Type</span></span> | <span data-ttu-id="d5c62-130">説明</span><span class="sxs-lookup"><span data-stu-id="d5c62-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="d5c62-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="d5c62-131">destinationId</span></span>|<span data-ttu-id="d5c62-132">String</span><span class="sxs-lookup"><span data-stu-id="d5c62-132">String</span></span>|<span data-ttu-id="d5c62-133">フォルダー ID、またはよく知られているフォルダー名。</span><span class="sxs-lookup"><span data-stu-id="d5c62-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d5c62-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5c62-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d5c62-135">応答</span><span class="sxs-lookup"><span data-stu-id="d5c62-135">Response</span></span>

<span data-ttu-id="d5c62-136">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d5c62-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c62-137">例</span><span class="sxs-lookup"><span data-stu-id="d5c62-137">Example</span></span>

<span data-ttu-id="d5c62-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d5c62-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d5c62-139">要求</span><span class="sxs-lookup"><span data-stu-id="d5c62-139">Request</span></span>
<span data-ttu-id="d5c62-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5c62-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="d5c62-141">応答</span><span class="sxs-lookup"><span data-stu-id="d5c62-141">Response</span></span>

<span data-ttu-id="d5c62-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d5c62-142">Here is an example of the response.</span></span>

> <span data-ttu-id="d5c62-143">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d5c62-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d5c62-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d5c62-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5c62-145">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d5c62-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5c62-146">Visual</span><span class="sxs-lookup"><span data-stu-id="d5c62-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/mailfolder_copy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5c62-147">Java</span><span class="sxs-lookup"><span data-stu-id="d5c62-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/mailfolder_copy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-copy.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-copy.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
