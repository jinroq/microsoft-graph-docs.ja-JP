---
title: MailSearchFolder を作成します。
description: 指定されたユーザーのメールボックスに新しい mailSearchFolder を作成するのにには、この API を使用します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517730"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="5ede2-103">MailSearchFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ede2-104">指定されたユーザーのメールボックスに新しい[mailSearchFolder](../resources/mailsearchfolder.md)を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ede2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ede2-105">Permissions</span></span>

<span data-ttu-id="5ede2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ede2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ede2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ede2-108">Permission type</span></span> | <span data-ttu-id="5ede2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ede2-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5ede2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ede2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ede2-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ede2-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5ede2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ede2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ede2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ede2-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5ede2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ede2-114">Application</span></span> | <span data-ttu-id="5ede2-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ede2-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ede2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ede2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="5ede2-117">フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5ede2-118">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ede2-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ede2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ede2-119">Request headers</span></span>

| <span data-ttu-id="5ede2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ede2-120">Header</span></span> | <span data-ttu-id="5ede2-121">値</span><span class="sxs-lookup"><span data-stu-id="5ede2-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5ede2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ede2-122">Authorization</span></span> | <span data-ttu-id="5ede2-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5ede2-123"></span></span> <span data-ttu-id="5ede2-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="5ede2-124">Required.</span></span> |
| <span data-ttu-id="5ede2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ede2-125">Content-Type</span></span> | <span data-ttu-id="5ede2-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5ede2-126"></span></span> <span data-ttu-id="5ede2-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="5ede2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ede2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ede2-128">Request body</span></span>

<span data-ttu-id="5ede2-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ede2-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ede2-130">Parameter</span></span> | <span data-ttu-id="5ede2-131">型</span><span class="sxs-lookup"><span data-stu-id="5ede2-131">Type</span></span> | <span data-ttu-id="5ede2-132">説明</span><span class="sxs-lookup"><span data-stu-id="5ede2-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="5ede2-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="5ede2-133">@odata.type</span></span> | <span data-ttu-id="5ede2-134">String</span><span class="sxs-lookup"><span data-stu-id="5ede2-134">String</span></span> | <span data-ttu-id="5ede2-135">作成するフォルダーの種類。</span><span class="sxs-lookup"><span data-stu-id="5ede2-135">The type of folder to be created.</span></span> <span data-ttu-id="5ede2-136">"Microsoft.graph.mailSearchFolder"に設定します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="5ede2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5ede2-137">displayName</span></span> | <span data-ttu-id="5ede2-138">String</span><span class="sxs-lookup"><span data-stu-id="5ede2-138">String</span></span> | <span data-ttu-id="5ede2-139">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="5ede2-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="5ede2-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="5ede2-140">includeNestedFolders</span></span> | <span data-ttu-id="5ede2-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="5ede2-141">Boolean</span></span> | <span data-ttu-id="5ede2-142">どのメールボックス フォルダー階層を走査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ede2-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="5ede2-143">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="5ede2-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="5ede2-144">sourceFolderIDs</span></span> | <span data-ttu-id="5ede2-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5ede2-145">String collection</span></span> | <span data-ttu-id="5ede2-146">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ede2-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5ede2-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="5ede2-147">filterQuery</span></span> | <span data-ttu-id="5ede2-148">String</span><span class="sxs-lookup"><span data-stu-id="5ede2-148">String</span></span> | <span data-ttu-id="5ede2-149">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="5ede2-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="5ede2-150">応答</span><span class="sxs-lookup"><span data-stu-id="5ede2-150">Response</span></span>

<span data-ttu-id="5ede2-151">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[mailSearchFolder](../resources/mailsearchfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5ede2-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ede2-152">例</span><span class="sxs-lookup"><span data-stu-id="5ede2-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5ede2-153">要求</span><span class="sxs-lookup"><span data-stu-id="5ede2-153">Request</span></span>

<span data-ttu-id="5ede2-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-154">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5ede2-155">応答</span><span class="sxs-lookup"><span data-stu-id="5ede2-155">Response</span></span>

<span data-ttu-id="5ede2-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ede2-156">The following is an example of the response.</span></span>

><span data-ttu-id="5ede2-157">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5ede2-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5ede2-158">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ede2-158">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
