---
title: MailFolder を作成する
description: この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 75ea651237eb0cadd0bd6cfbb1210c2901d1db43
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269966"
---
# <a name="create-mailfolder"></a><span data-ttu-id="daf5c-103">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="daf5c-103">Create MailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daf5c-104">この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="daf5c-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="daf5c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="daf5c-105">Permissions</span></span>
<span data-ttu-id="daf5c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="daf5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daf5c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="daf5c-108">Permission type</span></span>      | <span data-ttu-id="daf5c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="daf5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daf5c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="daf5c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="daf5c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daf5c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="daf5c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="daf5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daf5c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daf5c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="daf5c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="daf5c-114">Application</span></span> | <span data-ttu-id="daf5c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daf5c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="daf5c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="daf5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="daf5c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daf5c-117">Request headers</span></span>
| <span data-ttu-id="daf5c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daf5c-118">Header</span></span>       | <span data-ttu-id="daf5c-119">値</span><span class="sxs-lookup"><span data-stu-id="daf5c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="daf5c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf5c-120">Authorization</span></span>  | <span data-ttu-id="daf5c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="daf5c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="daf5c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daf5c-123">Content-Type</span></span>  | <span data-ttu-id="daf5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="daf5c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="daf5c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="daf5c-125">Request body</span></span>
<span data-ttu-id="daf5c-p103">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="daf5c-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="daf5c-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="daf5c-128">Parameter</span></span>    | <span data-ttu-id="daf5c-129">型</span><span class="sxs-lookup"><span data-stu-id="daf5c-129">Type</span></span>   |<span data-ttu-id="daf5c-130">説明</span><span class="sxs-lookup"><span data-stu-id="daf5c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daf5c-131">displayName</span><span class="sxs-lookup"><span data-stu-id="daf5c-131">displayName</span></span>|<span data-ttu-id="daf5c-132">String</span><span class="sxs-lookup"><span data-stu-id="daf5c-132">String</span></span>|<span data-ttu-id="daf5c-133">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="daf5c-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="daf5c-134">応答</span><span class="sxs-lookup"><span data-stu-id="daf5c-134">Response</span></span>

<span data-ttu-id="daf5c-135">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="daf5c-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf5c-136">例</span><span class="sxs-lookup"><span data-stu-id="daf5c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="daf5c-137">要求</span><span class="sxs-lookup"><span data-stu-id="daf5c-137">Request</span></span>
<span data-ttu-id="daf5c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="daf5c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="daf5c-139">応答</span><span class="sxs-lookup"><span data-stu-id="daf5c-139">Response</span></span>
<span data-ttu-id="daf5c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="daf5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="daf5c-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="daf5c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="daf5c-144">C#</span><span class="sxs-lookup"><span data-stu-id="daf5c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="daf5c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="daf5c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="daf5c-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="daf5c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
