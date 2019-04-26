---
title: Create mailFolder
description: この API を使用して、新しい子 mailfolder を作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 739556fe0f322cad7a36afb58bb78e4e521b374f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338689"
---
# <a name="create-mailfolder"></a><span data-ttu-id="eb9c8-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="eb9c8-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb9c8-104">この API を使用して、新しい子[mailfolder](../resources/mailfolder.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb9c8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb9c8-105">Permissions</span></span>

<span data-ttu-id="eb9c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb9c8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb9c8-108">Permission type</span></span> | <span data-ttu-id="eb9c8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb9c8-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="eb9c8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb9c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb9c8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb9c8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb9c8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb9c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb9c8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb9c8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb9c8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb9c8-114">Application</span></span> | <span data-ttu-id="eb9c8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb9c8-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb9c8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb9c8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="eb9c8-117">クエリの URL 内の親フォルダーをフォルダー ID または既知のフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="eb9c8-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb9c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb9c8-119">Request headers</span></span>

| <span data-ttu-id="eb9c8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb9c8-120">Header</span></span> | <span data-ttu-id="eb9c8-121">値</span><span class="sxs-lookup"><span data-stu-id="eb9c8-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="eb9c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9c8-122">Authorization</span></span> | <span data-ttu-id="eb9c8-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="eb9c8-123"></span></span> <span data-ttu-id="eb9c8-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-124">Required.</span></span> |
| <span data-ttu-id="eb9c8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb9c8-125">Content-Type</span></span> | <span data-ttu-id="eb9c8-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="eb9c8-126"></span></span> <span data-ttu-id="eb9c8-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb9c8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb9c8-128">Request body</span></span>

<span data-ttu-id="eb9c8-p105">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="eb9c8-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb9c8-131">Parameter</span></span> | <span data-ttu-id="eb9c8-132">型</span><span class="sxs-lookup"><span data-stu-id="eb9c8-132">Type</span></span> | <span data-ttu-id="eb9c8-133">説明</span><span class="sxs-lookup"><span data-stu-id="eb9c8-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="eb9c8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="eb9c8-134">displayName</span></span>|<span data-ttu-id="eb9c8-135">String</span><span class="sxs-lookup"><span data-stu-id="eb9c8-135">String</span></span>|<span data-ttu-id="eb9c8-136">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="eb9c8-137">応答</span><span class="sxs-lookup"><span data-stu-id="eb9c8-137">Response</span></span>

<span data-ttu-id="eb9c8-138">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9c8-139">例</span><span class="sxs-lookup"><span data-stu-id="eb9c8-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eb9c8-140">要求</span><span class="sxs-lookup"><span data-stu-id="eb9c8-140">Request</span></span>

<span data-ttu-id="eb9c8-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="eb9c8-142">応答</span><span class="sxs-lookup"><span data-stu-id="eb9c8-142">Response</span></span>

<span data-ttu-id="eb9c8-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-143">The following is an example of the response.</span></span>

> <span data-ttu-id="eb9c8-144">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb9c8-145">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb9c8-145">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
