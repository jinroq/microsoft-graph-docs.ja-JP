---
title: >
  List messages
description: サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0e04715d011d2cb4217c73b7dc234d48f38d56cb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612513"
---
# <a name="list-messages"></a><span data-ttu-id="c638d-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c638d-103">List messages</span></span>

<span data-ttu-id="c638d-104">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="c638d-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="c638d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c638d-105">Permissions</span></span>
<span data-ttu-id="c638d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c638d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c638d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c638d-108">Permission type</span></span>      | <span data-ttu-id="c638d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c638d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c638d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c638d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c638d-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c638d-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c638d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c638d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c638d-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c638d-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c638d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c638d-114">Application</span></span> | <span data-ttu-id="c638d-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c638d-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c638d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c638d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c638d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c638d-117">Optional query parameters</span></span>
<span data-ttu-id="c638d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c638d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c638d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c638d-119">Request headers</span></span>
| <span data-ttu-id="c638d-120">名前</span><span class="sxs-lookup"><span data-stu-id="c638d-120">Name</span></span>       | <span data-ttu-id="c638d-121">型</span><span class="sxs-lookup"><span data-stu-id="c638d-121">Type</span></span> | <span data-ttu-id="c638d-122">説明</span><span class="sxs-lookup"><span data-stu-id="c638d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c638d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c638d-123">Authorization</span></span>  | <span data-ttu-id="c638d-124">string</span><span class="sxs-lookup"><span data-stu-id="c638d-124">string</span></span>  | <span data-ttu-id="c638d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c638d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c638d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c638d-127">Request body</span></span>
<span data-ttu-id="c638d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c638d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c638d-129">応答</span><span class="sxs-lookup"><span data-stu-id="c638d-129">Response</span></span>

<span data-ttu-id="c638d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c638d-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c638d-131">例</span><span class="sxs-lookup"><span data-stu-id="c638d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c638d-132">要求</span><span class="sxs-lookup"><span data-stu-id="c638d-132">Request</span></span>
<span data-ttu-id="c638d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c638d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="c638d-134">応答</span><span class="sxs-lookup"><span data-stu-id="c638d-134">Response</span></span>
<span data-ttu-id="c638d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c638d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c638d-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c638d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c638d-139">C#</span><span class="sxs-lookup"><span data-stu-id="c638d-139">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c638d-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c638d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
