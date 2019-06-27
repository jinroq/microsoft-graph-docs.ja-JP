---
title: 'outlookUser: supportedLanguages'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 505fb1faf79660153c91ec7d985c9925cb561c79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274285"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="4227b-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="4227b-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="4227b-104">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4227b-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="4227b-105">Outlook クライアントを設定する際は、このサポートされているリストから、優先する言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="4227b-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="4227b-106">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先言語を取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4227b-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="4227b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4227b-107">Permissions</span></span>
<span data-ttu-id="4227b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4227b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4227b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4227b-110">Permission type</span></span>      | <span data-ttu-id="4227b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4227b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4227b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4227b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4227b-113">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4227b-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="4227b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4227b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4227b-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="4227b-115">User.Read</span></span>    |
|<span data-ttu-id="4227b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4227b-116">Application</span></span> | <span data-ttu-id="4227b-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4227b-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4227b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4227b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="4227b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4227b-119">Request headers</span></span>
| <span data-ttu-id="4227b-120">名前</span><span class="sxs-lookup"><span data-stu-id="4227b-120">Name</span></span>       | <span data-ttu-id="4227b-121">型</span><span class="sxs-lookup"><span data-stu-id="4227b-121">Type</span></span> | <span data-ttu-id="4227b-122">説明</span><span class="sxs-lookup"><span data-stu-id="4227b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4227b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4227b-123">Authorization</span></span>  | <span data-ttu-id="4227b-124">string</span><span class="sxs-lookup"><span data-stu-id="4227b-124">string</span></span>  | <span data-ttu-id="4227b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4227b-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4227b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4227b-127">Request body</span></span>
<span data-ttu-id="4227b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4227b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4227b-129">応答</span><span class="sxs-lookup"><span data-stu-id="4227b-129">Response</span></span>
<span data-ttu-id="4227b-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [localeInfo](../resources/localeinfo.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4227b-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4227b-131">例</span><span class="sxs-lookup"><span data-stu-id="4227b-131">Example</span></span>
<span data-ttu-id="4227b-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4227b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4227b-133">要求</span><span class="sxs-lookup"><span data-stu-id="4227b-133">Request</span></span>
<span data-ttu-id="4227b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4227b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="4227b-135">応答</span><span class="sxs-lookup"><span data-stu-id="4227b-135">Response</span></span>
<span data-ttu-id="4227b-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4227b-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4227b-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="4227b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4227b-138">C#</span><span class="sxs-lookup"><span data-stu-id="4227b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4227b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4227b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4227b-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="4227b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
