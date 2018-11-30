---
title: 'outlookUser: supportedLanguages'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。
ms.openlocfilehash: ac1b9693121f3ba3f180b53532bb6a6c917e2108
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066705"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="4b098-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="4b098-103">outlookUser: supportedLanguages</span></span>

> <span data-ttu-id="4b098-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b098-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b098-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b098-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b098-106">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4b098-106">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="4b098-107">Outlook クライアントを設定する際は、このサポートされているリストから、優先する言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="4b098-107">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="4b098-108">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先言語を取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4b098-108">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="4b098-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4b098-109">Permissions</span></span>
<span data-ttu-id="4b098-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b098-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b098-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b098-112">Permission type</span></span>      | <span data-ttu-id="4b098-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b098-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b098-114">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b098-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4b098-115">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4b098-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="4b098-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b098-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b098-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="4b098-117">User.Read</span></span>    |
|<span data-ttu-id="4b098-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b098-118">Application</span></span> | <span data-ttu-id="4b098-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b098-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b098-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b098-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="4b098-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b098-121">Request headers</span></span>
| <span data-ttu-id="4b098-122">名前</span><span class="sxs-lookup"><span data-stu-id="4b098-122">Name</span></span>       | <span data-ttu-id="4b098-123">型</span><span class="sxs-lookup"><span data-stu-id="4b098-123">Type</span></span> | <span data-ttu-id="4b098-124">説明</span><span class="sxs-lookup"><span data-stu-id="4b098-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b098-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b098-125">Authorization</span></span>  | <span data-ttu-id="4b098-126">string</span><span class="sxs-lookup"><span data-stu-id="4b098-126">string</span></span>  | <span data-ttu-id="4b098-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4b098-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4b098-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b098-129">Request body</span></span>
<span data-ttu-id="4b098-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4b098-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b098-131">応答</span><span class="sxs-lookup"><span data-stu-id="4b098-131">Response</span></span>
<span data-ttu-id="4b098-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [localeInfo](../resources/localeinfo.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4b098-132">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b098-133">例</span><span class="sxs-lookup"><span data-stu-id="4b098-133">Example</span></span>
<span data-ttu-id="4b098-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4b098-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b098-135">要求</span><span class="sxs-lookup"><span data-stu-id="4b098-135">Request</span></span>
<span data-ttu-id="4b098-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b098-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="4b098-137">応答</span><span class="sxs-lookup"><span data-stu-id="4b098-137">Response</span></span>
<span data-ttu-id="4b098-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4b098-138">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->