---
title: 'outlookUser: supportedLanguages'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 83b21c7e81078f82e2b9023153b711d080ed07cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877222"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="bb787-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="bb787-103">outlookUser: supportedLanguages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb787-104">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bb787-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="bb787-105">Outlook クライアントを設定する際は、このサポートされているリストから、優先する言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="bb787-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="bb787-106">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先言語を取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="bb787-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="bb787-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb787-107">Permissions</span></span>
<span data-ttu-id="bb787-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb787-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb787-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb787-110">Permission type</span></span>      | <span data-ttu-id="bb787-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb787-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb787-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb787-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb787-113">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="bb787-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="bb787-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb787-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb787-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="bb787-115">User.Read</span></span>    |
|<span data-ttu-id="bb787-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb787-116">Application</span></span> | <span data-ttu-id="bb787-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb787-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb787-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb787-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="bb787-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb787-119">Request headers</span></span>
| <span data-ttu-id="bb787-120">名前</span><span class="sxs-lookup"><span data-stu-id="bb787-120">Name</span></span>       | <span data-ttu-id="bb787-121">型</span><span class="sxs-lookup"><span data-stu-id="bb787-121">Type</span></span> | <span data-ttu-id="bb787-122">説明</span><span class="sxs-lookup"><span data-stu-id="bb787-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb787-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb787-123">Authorization</span></span>  | <span data-ttu-id="bb787-124">string</span><span class="sxs-lookup"><span data-stu-id="bb787-124">string</span></span>  | <span data-ttu-id="bb787-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb787-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bb787-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb787-127">Request body</span></span>
<span data-ttu-id="bb787-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bb787-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb787-129">応答</span><span class="sxs-lookup"><span data-stu-id="bb787-129">Response</span></span>
<span data-ttu-id="bb787-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [localeInfo](../resources/localeinfo.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bb787-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb787-131">例</span><span class="sxs-lookup"><span data-stu-id="bb787-131">Example</span></span>
<span data-ttu-id="bb787-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bb787-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb787-133">要求</span><span class="sxs-lookup"><span data-stu-id="bb787-133">Request</span></span>
<span data-ttu-id="bb787-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb787-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb787-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bb787-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb787-136">C#</span><span class="sxs-lookup"><span data-stu-id="bb787-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb787-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb787-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb787-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="bb787-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb787-139">Java</span><span class="sxs-lookup"><span data-stu-id="bb787-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedlanguages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb787-140">応答</span><span class="sxs-lookup"><span data-stu-id="bb787-140">Response</span></span>
<span data-ttu-id="bb787-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bb787-141">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
