---
title: MailSearchFolder を更新する
description: MailSearchFolder オブジェクトの書き込み可能なプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dac2bbb95da7d287ce00503ac4b79cdf52a85968
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536023"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="50b2e-103">MailSearchFolder を更新する</span><span class="sxs-lookup"><span data-stu-id="50b2e-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50b2e-104">[Mailsearchfolder](../resources/mailsearchfolder.md)オブジェクトの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50b2e-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50b2e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50b2e-105">Permissions</span></span>
<span data-ttu-id="50b2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b2e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50b2e-108">Permission type</span></span>      | <span data-ttu-id="50b2e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50b2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50b2e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50b2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50b2e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b2e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50b2e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50b2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50b2e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b2e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50b2e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50b2e-114">Application</span></span> | <span data-ttu-id="50b2e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50b2e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50b2e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50b2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="50b2e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50b2e-117">Request headers</span></span>
| <span data-ttu-id="50b2e-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50b2e-118">Header</span></span>       | <span data-ttu-id="50b2e-119">値</span><span class="sxs-lookup"><span data-stu-id="50b2e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50b2e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b2e-120">Authorization</span></span>  | <span data-ttu-id="50b2e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="50b2e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50b2e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50b2e-123">Content-Type</span></span>  | <span data-ttu-id="50b2e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50b2e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50b2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50b2e-126">Request body</span></span>
<span data-ttu-id="50b2e-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="50b2e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="50b2e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50b2e-130">Property</span></span>     | <span data-ttu-id="50b2e-131">型</span><span class="sxs-lookup"><span data-stu-id="50b2e-131">Type</span></span>   |<span data-ttu-id="50b2e-132">説明</span><span class="sxs-lookup"><span data-stu-id="50b2e-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50b2e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="50b2e-133">displayName</span></span> | <span data-ttu-id="50b2e-134">String</span><span class="sxs-lookup"><span data-stu-id="50b2e-134">String</span></span> | <span data-ttu-id="50b2e-135">[Mailfolder](../resources/mailfolder.md)の表示名。</span><span class="sxs-lookup"><span data-stu-id="50b2e-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="50b2e-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="50b2e-136">includeNestedFolders</span></span> | <span data-ttu-id="50b2e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="50b2e-137">Boolean</span></span> | <span data-ttu-id="50b2e-138">メールボックスフォルダー階層をスキャンする方法。</span><span class="sxs-lookup"><span data-stu-id="50b2e-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="50b2e-139">`true`詳細検索を実行`false`する必要がある場合は、その代わりに浅い検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="50b2e-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="50b2e-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="50b2e-140">sourceFolderIDs</span></span> | <span data-ttu-id="50b2e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="50b2e-141">String collection</span></span> | <span data-ttu-id="50b2e-142">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="50b2e-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="50b2e-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="50b2e-143">filterQuery</span></span> | <span data-ttu-id="50b2e-144">String</span><span class="sxs-lookup"><span data-stu-id="50b2e-144">String</span></span> | <span data-ttu-id="50b2e-145">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="50b2e-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="50b2e-146">応答</span><span class="sxs-lookup"><span data-stu-id="50b2e-146">Response</span></span>
<span data-ttu-id="50b2e-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50b2e-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b2e-148">例</span><span class="sxs-lookup"><span data-stu-id="50b2e-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="50b2e-149">要求</span><span class="sxs-lookup"><span data-stu-id="50b2e-149">Request</span></span>
<span data-ttu-id="50b2e-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50b2e-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="50b2e-151">応答</span><span class="sxs-lookup"><span data-stu-id="50b2e-151">Response</span></span>
<span data-ttu-id="50b2e-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50b2e-152">The following is an example of the response.</span></span>
><span data-ttu-id="50b2e-153">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="50b2e-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50b2e-154">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50b2e-154">All the properties will be returned from an actual call.</span></span>
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
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="50b2e-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="50b2e-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50b2e-156">C#</span><span class="sxs-lookup"><span data-stu-id="50b2e-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50b2e-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="50b2e-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
