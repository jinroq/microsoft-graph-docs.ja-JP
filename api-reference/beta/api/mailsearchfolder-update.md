---
title: MailSearchFolder を更新する
description: MailSearchFolder オブジェクトの書き込み可能なプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0bc0d18954e4a0c00c7e9e46be8a2ed03718acf8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266613"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="3ca84-103">MailSearchFolder を更新する</span><span class="sxs-lookup"><span data-stu-id="3ca84-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca84-104">[Mailsearchfolder](../resources/mailsearchfolder.md)オブジェクトの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-104">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ca84-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ca84-105">Permissions</span></span>
<span data-ttu-id="3ca84-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ca84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ca84-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ca84-108">Permission type</span></span>      | <span data-ttu-id="3ca84-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ca84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ca84-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ca84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ca84-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ca84-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3ca84-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ca84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ca84-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ca84-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3ca84-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ca84-114">Application</span></span> | <span data-ttu-id="3ca84-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ca84-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ca84-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ca84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ca84-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ca84-117">Request headers</span></span>
| <span data-ttu-id="3ca84-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ca84-118">Header</span></span>       | <span data-ttu-id="3ca84-119">値</span><span class="sxs-lookup"><span data-stu-id="3ca84-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ca84-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ca84-120">Authorization</span></span>  | <span data-ttu-id="3ca84-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ca84-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ca84-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ca84-123">Content-Type</span></span>  | <span data-ttu-id="3ca84-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3ca84-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ca84-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ca84-126">Request body</span></span>
<span data-ttu-id="3ca84-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3ca84-128">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="3ca84-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3ca84-129">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3ca84-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3ca84-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ca84-130">Property</span></span>     | <span data-ttu-id="3ca84-131">型</span><span class="sxs-lookup"><span data-stu-id="3ca84-131">Type</span></span>   |<span data-ttu-id="3ca84-132">説明</span><span class="sxs-lookup"><span data-stu-id="3ca84-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ca84-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3ca84-133">displayName</span></span> | <span data-ttu-id="3ca84-134">String</span><span class="sxs-lookup"><span data-stu-id="3ca84-134">String</span></span> | <span data-ttu-id="3ca84-135">[Mailfolder](../resources/mailfolder.md)の表示名。</span><span class="sxs-lookup"><span data-stu-id="3ca84-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="3ca84-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="3ca84-136">includeNestedFolders</span></span> | <span data-ttu-id="3ca84-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ca84-137">Boolean</span></span> | <span data-ttu-id="3ca84-138">メールボックスフォルダー階層をスキャンする方法。</span><span class="sxs-lookup"><span data-stu-id="3ca84-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="3ca84-139">`true`詳細検索を実行`false`する必要がある場合は、その代わりに浅い検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="3ca84-140">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="3ca84-140">sourceFolderIds</span></span> | <span data-ttu-id="3ca84-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3ca84-141">String collection</span></span> | <span data-ttu-id="3ca84-142">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="3ca84-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="3ca84-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="3ca84-143">filterQuery</span></span> | <span data-ttu-id="3ca84-144">String</span><span class="sxs-lookup"><span data-stu-id="3ca84-144">String</span></span> | <span data-ttu-id="3ca84-145">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="3ca84-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="3ca84-146">応答</span><span class="sxs-lookup"><span data-stu-id="3ca84-146">Response</span></span>
<span data-ttu-id="3ca84-147">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mailfolder](../resources/mailfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-147">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ca84-148">例</span><span class="sxs-lookup"><span data-stu-id="3ca84-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3ca84-149">要求</span><span class="sxs-lookup"><span data-stu-id="3ca84-149">Request</span></span>
<span data-ttu-id="3ca84-150">次に、検索フォルダーの**Filterquery**プロパティを更新する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-150">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```

#### <a name="response"></a><span data-ttu-id="3ca84-151">応答</span><span class="sxs-lookup"><span data-stu-id="3ca84-151">Response</span></span>
<span data-ttu-id="3ca84-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3ca84-152">The following is an example of the response.</span></span>
><span data-ttu-id="3ca84-153">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3ca84-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ca84-154">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ca84-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ca84-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3ca84-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ca84-156">C#</span><span class="sxs-lookup"><span data-stu-id="3ca84-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ca84-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ca84-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3ca84-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="3ca84-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
