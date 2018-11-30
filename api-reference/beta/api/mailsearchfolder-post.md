---
title: MailSearchFolder を作成します。
description: 指定されたユーザーのメールボックスに新しい mailSearchFolder を作成するのにには、この API を使用します。
ms.openlocfilehash: a35827a6b9164c8d4c1c0fe54a1897b2271fc5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072482"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="dd5b4-103">MailSearchFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="dd5b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd5b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd5b4-106">指定されたユーザーのメールボックスに新しい[mailSearchFolder](../resources/mailsearchfolder.md)を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd5b4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dd5b4-107">Permissions</span></span>

<span data-ttu-id="dd5b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd5b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd5b4-110">Permission type</span></span> | <span data-ttu-id="dd5b4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd5b4-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="dd5b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd5b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd5b4-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd5b4-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd5b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd5b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd5b4-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd5b4-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd5b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd5b4-116">Application</span></span> | <span data-ttu-id="dd5b4-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd5b4-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd5b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd5b4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="dd5b4-119">フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="dd5b4-120">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd5b4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd5b4-121">Request headers</span></span>

| <span data-ttu-id="dd5b4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd5b4-122">Header</span></span> | <span data-ttu-id="dd5b4-123">値</span><span class="sxs-lookup"><span data-stu-id="dd5b4-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="dd5b4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd5b4-124">Authorization</span></span> | <span data-ttu-id="dd5b4-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="dd5b4-125"></span></span> <span data-ttu-id="dd5b4-126">必須。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-126">Required.</span></span> |
| <span data-ttu-id="dd5b4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd5b4-127">Content-Type</span></span> | <span data-ttu-id="dd5b4-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="dd5b4-128"></span></span> <span data-ttu-id="dd5b4-129">必須。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd5b4-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd5b4-130">Request body</span></span>

<span data-ttu-id="dd5b4-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd5b4-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dd5b4-132">Parameter</span></span> | <span data-ttu-id="dd5b4-133">型</span><span class="sxs-lookup"><span data-stu-id="dd5b4-133">Type</span></span> | <span data-ttu-id="dd5b4-134">説明</span><span class="sxs-lookup"><span data-stu-id="dd5b4-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="dd5b4-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="dd5b4-135">@odata.type</span></span> | <span data-ttu-id="dd5b4-136">String</span><span class="sxs-lookup"><span data-stu-id="dd5b4-136">String</span></span> | <span data-ttu-id="dd5b4-137">作成するフォルダーの種類。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-137">The type of folder to be created.</span></span> <span data-ttu-id="dd5b4-138">"Microsoft.graph.mailSearchFolder"に設定します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="dd5b4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dd5b4-139">displayName</span></span> | <span data-ttu-id="dd5b4-140">String</span><span class="sxs-lookup"><span data-stu-id="dd5b4-140">String</span></span> | <span data-ttu-id="dd5b4-141">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="dd5b4-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="dd5b4-142">includeNestedFolders</span></span> | <span data-ttu-id="dd5b4-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="dd5b4-143">Boolean</span></span> | <span data-ttu-id="dd5b4-144">どのメールボックス フォルダー階層を走査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="dd5b4-145">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="dd5b4-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="dd5b4-146">sourceFolderIDs</span></span> | <span data-ttu-id="dd5b4-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dd5b4-147">String collection</span></span> | <span data-ttu-id="dd5b4-148">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="dd5b4-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="dd5b4-149">filterQuery</span></span> | <span data-ttu-id="dd5b4-150">String</span><span class="sxs-lookup"><span data-stu-id="dd5b4-150">String</span></span> | <span data-ttu-id="dd5b4-151">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="dd5b4-152">応答</span><span class="sxs-lookup"><span data-stu-id="dd5b4-152">Response</span></span>

<span data-ttu-id="dd5b4-153">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[mailSearchFolder](../resources/mailsearchfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd5b4-154">例</span><span class="sxs-lookup"><span data-stu-id="dd5b4-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dd5b4-155">要求</span><span class="sxs-lookup"><span data-stu-id="dd5b4-155">Request</span></span>

<span data-ttu-id="dd5b4-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-156">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="dd5b4-157">応答</span><span class="sxs-lookup"><span data-stu-id="dd5b4-157">Response</span></span>

<span data-ttu-id="dd5b4-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-158">The following is an example of the response.</span></span>

><span data-ttu-id="dd5b4-159">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd5b4-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dd5b4-160">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
