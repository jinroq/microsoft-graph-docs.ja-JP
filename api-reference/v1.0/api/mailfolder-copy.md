---
title: 'mailFolder: コピー'
description: mailFolder とその内容を別の mailFolder にコピーします。
ms.openlocfilehash: 8cee2ad91fe40a9e9ef40c3a4662b76e71be1ccd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020734"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="c44ae-103">mailFolder: コピー</span><span class="sxs-lookup"><span data-stu-id="c44ae-103">mailFolder: copy</span></span>

<span data-ttu-id="c44ae-104">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="c44ae-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c44ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c44ae-105">Permissions</span></span>

<span data-ttu-id="c44ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c44ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c44ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c44ae-108">Permission type</span></span> | <span data-ttu-id="c44ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c44ae-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c44ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c44ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c44ae-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c44ae-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c44ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c44ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c44ae-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c44ae-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c44ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c44ae-114">Application</span></span> | <span data-ttu-id="c44ae-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c44ae-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c44ae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c44ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="c44ae-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c44ae-117">Request headers</span></span>
| <span data-ttu-id="c44ae-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c44ae-118">Header</span></span> | <span data-ttu-id="c44ae-119">値</span><span class="sxs-lookup"><span data-stu-id="c44ae-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c44ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c44ae-120">Authorization</span></span> | <span data-ttu-id="c44ae-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c44ae-121"></span></span> <span data-ttu-id="c44ae-122">必須。</span><span class="sxs-lookup"><span data-stu-id="c44ae-122">Required.</span></span> |
| <span data-ttu-id="c44ae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c44ae-123">Content-Type</span></span> | <span data-ttu-id="c44ae-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c44ae-124"></span></span> <span data-ttu-id="c44ae-125">必須。</span><span class="sxs-lookup"><span data-stu-id="c44ae-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c44ae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c44ae-126">Request body</span></span>

<span data-ttu-id="c44ae-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c44ae-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c44ae-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c44ae-128">Parameter</span></span> | <span data-ttu-id="c44ae-129">型</span><span class="sxs-lookup"><span data-stu-id="c44ae-129">Type</span></span> | <span data-ttu-id="c44ae-130">説明</span><span class="sxs-lookup"><span data-stu-id="c44ae-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c44ae-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="c44ae-131">destinationId</span></span>|<span data-ttu-id="c44ae-132">String</span><span class="sxs-lookup"><span data-stu-id="c44ae-132">String</span></span>|<span data-ttu-id="c44ae-133">フォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="c44ae-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c44ae-134">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c44ae-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c44ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="c44ae-135">Response</span></span>

<span data-ttu-id="c44ae-136">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文の[mailFolder](../resources/mailfolder.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="c44ae-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c44ae-137">例</span><span class="sxs-lookup"><span data-stu-id="c44ae-137">Example</span></span>

<span data-ttu-id="c44ae-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c44ae-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c44ae-139">要求</span><span class="sxs-lookup"><span data-stu-id="c44ae-139">Request</span></span>
<span data-ttu-id="c44ae-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c44ae-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c44ae-141">応答</span><span class="sxs-lookup"><span data-stu-id="c44ae-141">Response</span></span>

<span data-ttu-id="c44ae-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c44ae-142">Here is an example of the response.</span></span>

> <span data-ttu-id="c44ae-143">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c44ae-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c44ae-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c44ae-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
