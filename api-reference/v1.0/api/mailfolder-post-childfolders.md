---
title: MailFolder を作成する
description: この API を使用して、新しい子 mailFolder を作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a52574cdddbccec0654ddc11fa0a1cbf467ae6f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856419"
---
# <a name="create-mailfolder"></a><span data-ttu-id="d6890-103">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="d6890-103">Create MailFolder</span></span>

<span data-ttu-id="d6890-104">この API を使用して、新しい子 mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="d6890-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6890-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6890-105">Permissions</span></span>

<span data-ttu-id="d6890-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6890-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6890-108">Permission type</span></span> | <span data-ttu-id="d6890-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6890-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d6890-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6890-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6890-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6890-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6890-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6890-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6890-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6890-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6890-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6890-114">Application</span></span> | <span data-ttu-id="d6890-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6890-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6890-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6890-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="d6890-117">クエリの URL 内の親フォルダーをフォルダー ID または既知のフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="d6890-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d6890-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6890-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6890-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6890-119">Request headers</span></span>

| <span data-ttu-id="d6890-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6890-120">Header</span></span> | <span data-ttu-id="d6890-121">値</span><span class="sxs-lookup"><span data-stu-id="d6890-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d6890-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6890-122">Authorization</span></span> | <span data-ttu-id="d6890-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d6890-123"></span></span> <span data-ttu-id="d6890-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="d6890-124">Required.</span></span> |
| <span data-ttu-id="d6890-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6890-125">Content-Type</span></span> | <span data-ttu-id="d6890-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d6890-126"></span></span> <span data-ttu-id="d6890-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="d6890-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6890-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6890-128">Request body</span></span>

<span data-ttu-id="d6890-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d6890-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="d6890-130">**displayName**は、 [mailfolder](../resources/mailfolder.md)オブジェクトの唯一の書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="d6890-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="d6890-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6890-131">Parameter</span></span> | <span data-ttu-id="d6890-132">型</span><span class="sxs-lookup"><span data-stu-id="d6890-132">Type</span></span> | <span data-ttu-id="d6890-133">説明</span><span class="sxs-lookup"><span data-stu-id="d6890-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="d6890-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d6890-134">displayName</span></span>|<span data-ttu-id="d6890-135">String</span><span class="sxs-lookup"><span data-stu-id="d6890-135">String</span></span>|<span data-ttu-id="d6890-136">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="d6890-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="d6890-137">応答</span><span class="sxs-lookup"><span data-stu-id="d6890-137">Response</span></span>

<span data-ttu-id="d6890-138">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d6890-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6890-139">例</span><span class="sxs-lookup"><span data-stu-id="d6890-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6890-140">要求</span><span class="sxs-lookup"><span data-stu-id="d6890-140">Request</span></span>

<span data-ttu-id="d6890-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6890-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6890-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d6890-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6890-143">C#</span><span class="sxs-lookup"><span data-stu-id="d6890-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6890-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6890-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6890-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="d6890-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6890-146">Java</span><span class="sxs-lookup"><span data-stu-id="d6890-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6890-147">応答</span><span class="sxs-lookup"><span data-stu-id="d6890-147">Response</span></span>
<span data-ttu-id="d6890-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d6890-148">Here is an example of the response.</span></span>

> <span data-ttu-id="d6890-149">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6890-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d6890-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6890-150">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
