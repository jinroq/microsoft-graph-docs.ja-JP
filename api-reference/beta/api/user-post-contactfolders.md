---
title: ContactFolder を作成する　
description: ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e1da488913703552394b7e2e761151933e10a99
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269532"
---
# <a name="create-contactfolder"></a><span data-ttu-id="64af9-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="64af9-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64af9-104">ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="64af9-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="64af9-105">また、[指定した連絡先フォルダーの子として新しい contactfolder を作成](contactfolder-post-childfolders.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="64af9-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="64af9-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="64af9-106">Permissions</span></span>
<span data-ttu-id="64af9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64af9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64af9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64af9-109">Permission type</span></span>      | <span data-ttu-id="64af9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="64af9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64af9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64af9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64af9-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64af9-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="64af9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64af9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64af9-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64af9-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="64af9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64af9-115">Application</span></span> | <span data-ttu-id="64af9-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64af9-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="64af9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64af9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="64af9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64af9-118">Request headers</span></span>
| <span data-ttu-id="64af9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64af9-119">Header</span></span>       | <span data-ttu-id="64af9-120">値</span><span class="sxs-lookup"><span data-stu-id="64af9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64af9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64af9-121">Authorization</span></span>  | <span data-ttu-id="64af9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="64af9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64af9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64af9-124">Content-Type</span></span>  | <span data-ttu-id="64af9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64af9-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64af9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="64af9-126">Request body</span></span>
<span data-ttu-id="64af9-127">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64af9-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64af9-128">応答</span><span class="sxs-lookup"><span data-stu-id="64af9-128">Response</span></span>

<span data-ttu-id="64af9-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64af9-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64af9-130">例</span><span class="sxs-lookup"><span data-stu-id="64af9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64af9-131">要求</span><span class="sxs-lookup"><span data-stu-id="64af9-131">Request</span></span>
<span data-ttu-id="64af9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64af9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="64af9-133">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64af9-133">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="64af9-134">応答</span><span class="sxs-lookup"><span data-stu-id="64af9-134">Response</span></span>
<span data-ttu-id="64af9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64af9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="64af9-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="64af9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="64af9-139">C#</span><span class="sxs-lookup"><span data-stu-id="64af9-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64af9-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="64af9-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="64af9-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="64af9-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
