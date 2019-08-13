---
title: Create mailFolder
description: この API を使用して、新しい子 mailFolder を作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7690d79c8745fc1b0ed54f7053af89c0c5d3d4fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347074"
---
# <a name="create-mailfolder"></a><span data-ttu-id="0aeb8-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="0aeb8-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aeb8-104">この API を使用して、新しい子[Mailfolder](../resources/mailfolder.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0aeb8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0aeb8-105">Permissions</span></span>

<span data-ttu-id="0aeb8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0aeb8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0aeb8-108">Permission type</span></span> | <span data-ttu-id="0aeb8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0aeb8-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="0aeb8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0aeb8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0aeb8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeb8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0aeb8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0aeb8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aeb8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeb8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0aeb8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0aeb8-114">Application</span></span> | <span data-ttu-id="0aeb8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeb8-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aeb8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0aeb8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="0aeb8-117">クエリの URL 内の親フォルダーをフォルダー ID または既知のフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="0aeb8-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0aeb8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aeb8-119">Request headers</span></span>

| <span data-ttu-id="0aeb8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aeb8-120">Header</span></span> | <span data-ttu-id="0aeb8-121">値</span><span class="sxs-lookup"><span data-stu-id="0aeb8-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="0aeb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aeb8-122">Authorization</span></span> | <span data-ttu-id="0aeb8-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="0aeb8-123"></span></span> <span data-ttu-id="0aeb8-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-124">Required.</span></span> |
| <span data-ttu-id="0aeb8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0aeb8-125">Content-Type</span></span> | <span data-ttu-id="0aeb8-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="0aeb8-126"></span></span> <span data-ttu-id="0aeb8-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aeb8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0aeb8-128">Request body</span></span>

<span data-ttu-id="0aeb8-p105">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="0aeb8-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0aeb8-131">Parameter</span></span> | <span data-ttu-id="0aeb8-132">型</span><span class="sxs-lookup"><span data-stu-id="0aeb8-132">Type</span></span> | <span data-ttu-id="0aeb8-133">説明</span><span class="sxs-lookup"><span data-stu-id="0aeb8-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="0aeb8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0aeb8-134">displayName</span></span>|<span data-ttu-id="0aeb8-135">String</span><span class="sxs-lookup"><span data-stu-id="0aeb8-135">String</span></span>|<span data-ttu-id="0aeb8-136">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="0aeb8-137">応答</span><span class="sxs-lookup"><span data-stu-id="0aeb8-137">Response</span></span>

<span data-ttu-id="0aeb8-138">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aeb8-139">例</span><span class="sxs-lookup"><span data-stu-id="0aeb8-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0aeb8-140">要求</span><span class="sxs-lookup"><span data-stu-id="0aeb8-140">Request</span></span>

<span data-ttu-id="0aeb8-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0aeb8-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0aeb8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0aeb8-143">C#</span><span class="sxs-lookup"><span data-stu-id="0aeb8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0aeb8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aeb8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0aeb8-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="0aeb8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0aeb8-146">Java</span><span class="sxs-lookup"><span data-stu-id="0aeb8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0aeb8-147">応答</span><span class="sxs-lookup"><span data-stu-id="0aeb8-147">Response</span></span>

<span data-ttu-id="0aeb8-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0aeb8-149">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0aeb8-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0aeb8-150">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
