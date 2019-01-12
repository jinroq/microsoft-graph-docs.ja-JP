---
title: MailSearchFolder を作成します。
description: 指定されたユーザーのメールボックスに新しい mailSearchFolder を作成するのにには、この API を使用します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 626bf3a2e8bc77ba929895eed74ac0bb803aa5d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912877"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="a6147-103">MailSearchFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6147-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="a6147-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6147-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6147-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6147-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6147-106">指定されたユーザーのメールボックスに新しい[mailSearchFolder](../resources/mailsearchfolder.md)を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="a6147-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6147-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6147-107">Permissions</span></span>

<span data-ttu-id="a6147-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6147-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6147-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6147-110">Permission type</span></span> | <span data-ttu-id="a6147-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6147-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a6147-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6147-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6147-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6147-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a6147-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6147-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6147-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6147-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a6147-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6147-116">Application</span></span> | <span data-ttu-id="a6147-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6147-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6147-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6147-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="a6147-119">フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6147-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="a6147-120">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6147-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6147-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6147-121">Request headers</span></span>

| <span data-ttu-id="a6147-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6147-122">Header</span></span> | <span data-ttu-id="a6147-123">値</span><span class="sxs-lookup"><span data-stu-id="a6147-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a6147-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6147-124">Authorization</span></span> | <span data-ttu-id="a6147-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a6147-125"></span></span> <span data-ttu-id="a6147-126">必須。</span><span class="sxs-lookup"><span data-stu-id="a6147-126">Required.</span></span> |
| <span data-ttu-id="a6147-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6147-127">Content-Type</span></span> | <span data-ttu-id="a6147-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a6147-128"></span></span> <span data-ttu-id="a6147-129">必須。</span><span class="sxs-lookup"><span data-stu-id="a6147-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6147-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6147-130">Request body</span></span>

<span data-ttu-id="a6147-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6147-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6147-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6147-132">Parameter</span></span> | <span data-ttu-id="a6147-133">Type</span><span class="sxs-lookup"><span data-stu-id="a6147-133">Type</span></span> | <span data-ttu-id="a6147-134">説明</span><span class="sxs-lookup"><span data-stu-id="a6147-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a6147-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="a6147-135">@odata.type</span></span> | <span data-ttu-id="a6147-136">String</span><span class="sxs-lookup"><span data-stu-id="a6147-136">String</span></span> | <span data-ttu-id="a6147-137">作成するフォルダーの種類。</span><span class="sxs-lookup"><span data-stu-id="a6147-137">The type of folder to be created.</span></span> <span data-ttu-id="a6147-138">"Microsoft.graph.mailSearchFolder"に設定します。</span><span class="sxs-lookup"><span data-stu-id="a6147-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="a6147-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a6147-139">displayName</span></span> | <span data-ttu-id="a6147-140">String</span><span class="sxs-lookup"><span data-stu-id="a6147-140">String</span></span> | <span data-ttu-id="a6147-141">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="a6147-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="a6147-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="a6147-142">includeNestedFolders</span></span> | <span data-ttu-id="a6147-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="a6147-143">Boolean</span></span> | <span data-ttu-id="a6147-144">どのメールボックス フォルダー階層を走査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6147-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="a6147-145">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="a6147-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="a6147-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="a6147-146">sourceFolderIDs</span></span> | <span data-ttu-id="a6147-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6147-147">String collection</span></span> | <span data-ttu-id="a6147-148">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6147-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="a6147-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="a6147-149">filterQuery</span></span> | <span data-ttu-id="a6147-150">String</span><span class="sxs-lookup"><span data-stu-id="a6147-150">String</span></span> | <span data-ttu-id="a6147-151">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="a6147-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="a6147-152">応答</span><span class="sxs-lookup"><span data-stu-id="a6147-152">Response</span></span>

<span data-ttu-id="a6147-153">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[mailSearchFolder](../resources/mailsearchfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6147-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6147-154">例</span><span class="sxs-lookup"><span data-stu-id="a6147-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a6147-155">要求</span><span class="sxs-lookup"><span data-stu-id="a6147-155">Request</span></span>

<span data-ttu-id="a6147-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6147-156">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a6147-157">応答</span><span class="sxs-lookup"><span data-stu-id="a6147-157">Response</span></span>

<span data-ttu-id="a6147-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6147-158">The following is an example of the response.</span></span>

><span data-ttu-id="a6147-159">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a6147-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6147-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6147-160">All the properties will be returned from an actual call.</span></span>
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
