---
title: mailsearchfolder を作成する
description: この API を使用して、指定したユーザーのメールボックスに新しい mailsearchfolder を作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bdebbcb9c842d57d4c6ee8d8eb72f45df74a22d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333311"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="0f59d-103">mailsearchfolder を作成する</span><span class="sxs-lookup"><span data-stu-id="0f59d-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f59d-104">この API を使用して、指定したユーザーのメールボックスに新しい[mailsearchfolder](../resources/mailsearchfolder.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f59d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f59d-105">Permissions</span></span>

<span data-ttu-id="0f59d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f59d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f59d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f59d-108">Permission type</span></span> | <span data-ttu-id="0f59d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f59d-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="0f59d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f59d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f59d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f59d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0f59d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f59d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f59d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f59d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0f59d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f59d-114">Application</span></span> | <span data-ttu-id="0f59d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f59d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f59d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f59d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="0f59d-117">クエリの URL 内の親フォルダーをフォルダー ID または既知のフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="0f59d-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f59d-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f59d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f59d-119">Request headers</span></span>

| <span data-ttu-id="0f59d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f59d-120">Header</span></span> | <span data-ttu-id="0f59d-121">値</span><span class="sxs-lookup"><span data-stu-id="0f59d-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="0f59d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f59d-122">Authorization</span></span> | <span data-ttu-id="0f59d-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="0f59d-123"></span></span> <span data-ttu-id="0f59d-124">必須。</span><span class="sxs-lookup"><span data-stu-id="0f59d-124">Required.</span></span> |
| <span data-ttu-id="0f59d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f59d-125">Content-Type</span></span> | <span data-ttu-id="0f59d-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="0f59d-126"></span></span> <span data-ttu-id="0f59d-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="0f59d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f59d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f59d-128">Request body</span></span>

<span data-ttu-id="0f59d-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f59d-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0f59d-130">Parameter</span></span> | <span data-ttu-id="0f59d-131">型</span><span class="sxs-lookup"><span data-stu-id="0f59d-131">Type</span></span> | <span data-ttu-id="0f59d-132">説明</span><span class="sxs-lookup"><span data-stu-id="0f59d-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="0f59d-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="0f59d-133">@odata.type</span></span> | <span data-ttu-id="0f59d-134">String</span><span class="sxs-lookup"><span data-stu-id="0f59d-134">String</span></span> | <span data-ttu-id="0f59d-135">作成するフォルダーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-135">The type of folder to be created.</span></span> <span data-ttu-id="0f59d-136">"..." フォルダーに設定します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="0f59d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0f59d-137">displayName</span></span> | <span data-ttu-id="0f59d-138">String</span><span class="sxs-lookup"><span data-stu-id="0f59d-138">String</span></span> | <span data-ttu-id="0f59d-139">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="0f59d-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="0f59d-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="0f59d-140">includeNestedFolders</span></span> | <span data-ttu-id="0f59d-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f59d-141">Boolean</span></span> | <span data-ttu-id="0f59d-142">メールボックスフォルダー階層をスキャンする方法。</span><span class="sxs-lookup"><span data-stu-id="0f59d-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="0f59d-143">`true`詳細検索を実行`false`する必要がある場合は、その代わりに浅い検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="0f59d-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="0f59d-144">sourceFolderIDs</span></span> | <span data-ttu-id="0f59d-145">String collection</span><span class="sxs-lookup"><span data-stu-id="0f59d-145">String collection</span></span> | <span data-ttu-id="0f59d-146">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="0f59d-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="0f59d-147">filterquery</span><span class="sxs-lookup"><span data-stu-id="0f59d-147">filterQuery</span></span> | <span data-ttu-id="0f59d-148">String</span><span class="sxs-lookup"><span data-stu-id="0f59d-148">String</span></span> | <span data-ttu-id="0f59d-149">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="0f59d-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="0f59d-150">応答</span><span class="sxs-lookup"><span data-stu-id="0f59d-150">Response</span></span>

<span data-ttu-id="0f59d-151">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[mailsearchfolder](../resources/mailsearchfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f59d-152">例</span><span class="sxs-lookup"><span data-stu-id="0f59d-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0f59d-153">要求</span><span class="sxs-lookup"><span data-stu-id="0f59d-153">Request</span></span>

<span data-ttu-id="0f59d-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="0f59d-155">応答</span><span class="sxs-lookup"><span data-stu-id="0f59d-155">Response</span></span>

<span data-ttu-id="0f59d-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f59d-156">The following is an example of the response.</span></span>

><span data-ttu-id="0f59d-157">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0f59d-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f59d-158">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0f59d-158">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
