---
title: MailFolder を作成する
description: この API を使用して、新しい子 mailFolder を作成します。
author: angelgolfer-ms
ms.openlocfilehash: 717baa63f3bb15355eaf59387b8fc701ab1288b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331522"
---
# <a name="create-mailfolder"></a><span data-ttu-id="ecd22-103">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="ecd22-103">Create MailFolder</span></span>

<span data-ttu-id="ecd22-104">この API を使用して、新しい子 mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="ecd22-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecd22-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ecd22-105">Permissions</span></span>

<span data-ttu-id="ecd22-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecd22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecd22-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecd22-108">Permission type</span></span> | <span data-ttu-id="ecd22-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecd22-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ecd22-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecd22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ecd22-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecd22-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ecd22-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecd22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecd22-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecd22-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ecd22-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecd22-114">Application</span></span> | <span data-ttu-id="ecd22-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecd22-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecd22-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecd22-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="ecd22-117">フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="ecd22-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ecd22-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecd22-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecd22-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecd22-119">Request headers</span></span>

| <span data-ttu-id="ecd22-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecd22-120">Header</span></span> | <span data-ttu-id="ecd22-121">値</span><span class="sxs-lookup"><span data-stu-id="ecd22-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ecd22-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecd22-122">Authorization</span></span> | <span data-ttu-id="ecd22-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ecd22-123"></span></span> <span data-ttu-id="ecd22-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="ecd22-124">Required.</span></span> |
| <span data-ttu-id="ecd22-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecd22-125">Content-Type</span></span> | <span data-ttu-id="ecd22-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ecd22-126"></span></span> <span data-ttu-id="ecd22-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="ecd22-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecd22-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecd22-128">Request body</span></span>

<span data-ttu-id="ecd22-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ecd22-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="ecd22-130">**表示名**は、 [mailFolder](../resources/mailfolder.md)オブジェクトにのみ書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ecd22-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="ecd22-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ecd22-131">Parameter</span></span> | <span data-ttu-id="ecd22-132">種類</span><span class="sxs-lookup"><span data-stu-id="ecd22-132">Type</span></span> | <span data-ttu-id="ecd22-133">説明</span><span class="sxs-lookup"><span data-stu-id="ecd22-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ecd22-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ecd22-134">displayName</span></span>|<span data-ttu-id="ecd22-135">String</span><span class="sxs-lookup"><span data-stu-id="ecd22-135">String</span></span>|<span data-ttu-id="ecd22-136">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="ecd22-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="ecd22-137">応答</span><span class="sxs-lookup"><span data-stu-id="ecd22-137">Response</span></span>

<span data-ttu-id="ecd22-138">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文の[mailFolder](../resources/mailfolder.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="ecd22-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecd22-139">例</span><span class="sxs-lookup"><span data-stu-id="ecd22-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ecd22-140">要求</span><span class="sxs-lookup"><span data-stu-id="ecd22-140">Request</span></span>

<span data-ttu-id="ecd22-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecd22-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ecd22-142">応答</span><span class="sxs-lookup"><span data-stu-id="ecd22-142">Response</span></span>
<span data-ttu-id="ecd22-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ecd22-143">Here is an example of the response.</span></span>

> <span data-ttu-id="ecd22-144">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ecd22-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ecd22-145">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ecd22-145">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->