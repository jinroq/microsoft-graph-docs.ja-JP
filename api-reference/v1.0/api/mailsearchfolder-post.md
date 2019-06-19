---
title: MailSearchFolder を作成する
description: この API を使用して、指定したユーザーのメールボックスに新しい mailSearchFolder を作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 55cd832b5fb6a90e919890fb05553384e58807db
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818681"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="3bfea-103">MailSearchFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="3bfea-103">Create mailSearchFolder</span></span>

<span data-ttu-id="3bfea-104">指定したユーザーのメールボックスに新しい[Mailsearchfolder](../resources/mailsearchfolder.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-104">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bfea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bfea-105">Permissions</span></span>

<span data-ttu-id="3bfea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bfea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bfea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bfea-108">Permission type</span></span> | <span data-ttu-id="3bfea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bfea-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="3bfea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bfea-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bfea-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3bfea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bfea-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bfea-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3bfea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bfea-114">Application</span></span> | <span data-ttu-id="3bfea-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bfea-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bfea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bfea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="3bfea-117">クエリの URL 内の親フォルダーをフォルダー ID または既知のフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="3bfea-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bfea-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bfea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bfea-119">Request headers</span></span>

| <span data-ttu-id="3bfea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bfea-120">Header</span></span> | <span data-ttu-id="3bfea-121">値</span><span class="sxs-lookup"><span data-stu-id="3bfea-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="3bfea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bfea-122">Authorization</span></span> | <span data-ttu-id="3bfea-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="3bfea-123"></span></span> <span data-ttu-id="3bfea-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="3bfea-124">Required.</span></span> |
| <span data-ttu-id="3bfea-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bfea-125">Content-Type</span></span> | <span data-ttu-id="3bfea-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="3bfea-126"></span></span> <span data-ttu-id="3bfea-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="3bfea-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bfea-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bfea-128">Request body</span></span>

<span data-ttu-id="3bfea-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3bfea-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3bfea-130">Parameter</span></span> | <span data-ttu-id="3bfea-131">型</span><span class="sxs-lookup"><span data-stu-id="3bfea-131">Type</span></span> | <span data-ttu-id="3bfea-132">説明</span><span class="sxs-lookup"><span data-stu-id="3bfea-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="3bfea-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="3bfea-133">@odata.type</span></span> | <span data-ttu-id="3bfea-134">String</span><span class="sxs-lookup"><span data-stu-id="3bfea-134">String</span></span> | <span data-ttu-id="3bfea-135">作成するフォルダーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-135">The type of folder to be created.</span></span> <span data-ttu-id="3bfea-136">"..." フォルダーに設定します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="3bfea-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3bfea-137">displayName</span></span> | <span data-ttu-id="3bfea-138">String</span><span class="sxs-lookup"><span data-stu-id="3bfea-138">String</span></span> | <span data-ttu-id="3bfea-139">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="3bfea-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="3bfea-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="3bfea-140">includeNestedFolders</span></span> | <span data-ttu-id="3bfea-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bfea-141">Boolean</span></span> | <span data-ttu-id="3bfea-142">検索でメールボックスフォルダー階層をスキャンする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-142">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="3bfea-143">`true`**sourceFolderIds**で明示的に指定された各フォルダーの階層内に子フォルダーを含めるには、詳細検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-143">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="3bfea-144">`false`は、 **sourceFolderIds**で明示的に指定された各フォルダーの浅い検索を意味します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-144">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="3bfea-145">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="3bfea-145">sourceFolderIds</span></span> | <span data-ttu-id="3bfea-146">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3bfea-146">String collection</span></span> | <span data-ttu-id="3bfea-147">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="3bfea-147">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="3bfea-148">filterQuery</span><span class="sxs-lookup"><span data-stu-id="3bfea-148">filterQuery</span></span> | <span data-ttu-id="3bfea-149">String</span><span class="sxs-lookup"><span data-stu-id="3bfea-149">String</span></span> | <span data-ttu-id="3bfea-150">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="3bfea-150">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="3bfea-151">応答</span><span class="sxs-lookup"><span data-stu-id="3bfea-151">Response</span></span>

<span data-ttu-id="3bfea-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[mailsearchfolder](../resources/mailsearchfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-152">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bfea-153">例</span><span class="sxs-lookup"><span data-stu-id="3bfea-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3bfea-154">要求</span><span class="sxs-lookup"><span data-stu-id="3bfea-154">Request</span></span>

<span data-ttu-id="3bfea-155">要求の例を次に示します。件名に "weekly digest" という文字列が含まれているメッセージの検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-155">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="3bfea-156">検索フォルダーは、指定されたフィルタークエリが適用されるのと同じフォルダーにあります。</span><span class="sxs-lookup"><span data-stu-id="3bfea-156">The search folder is under the same folder on which the specified filter query applies.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```

#### <a name="response"></a><span data-ttu-id="3bfea-157">応答</span><span class="sxs-lookup"><span data-stu-id="3bfea-157">Response</span></span>

<span data-ttu-id="3bfea-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3bfea-158">The following is an example of the response.</span></span>

><span data-ttu-id="3bfea-159">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3bfea-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3bfea-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3bfea-160">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "wellKnownName": null,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
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
  "suppressions": [
  
  ]
}
-->