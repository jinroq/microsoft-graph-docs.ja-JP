---
title: >
  List messages
description: サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d1e77130a6181d6b32b832312568c7005eb4b37f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856469"
---
# <a name="list-messages"></a><span data-ttu-id="21266-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="21266-103">List messages</span></span>

<span data-ttu-id="21266-104">指定したユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="21266-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="21266-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="21266-105">Permissions</span></span>
<span data-ttu-id="21266-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21266-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21266-108">Permission type</span></span>      | <span data-ttu-id="21266-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="21266-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21266-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21266-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21266-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21266-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="21266-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21266-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21266-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21266-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="21266-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21266-114">Application</span></span> | <span data-ttu-id="21266-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21266-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21266-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21266-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21266-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="21266-117">Optional query parameters</span></span>
<span data-ttu-id="21266-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="21266-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="21266-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21266-119">Request headers</span></span>
| <span data-ttu-id="21266-120">名前</span><span class="sxs-lookup"><span data-stu-id="21266-120">Name</span></span>       | <span data-ttu-id="21266-121">型</span><span class="sxs-lookup"><span data-stu-id="21266-121">Type</span></span> | <span data-ttu-id="21266-122">説明</span><span class="sxs-lookup"><span data-stu-id="21266-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21266-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21266-123">Authorization</span></span>  | <span data-ttu-id="21266-124">string</span><span class="sxs-lookup"><span data-stu-id="21266-124">string</span></span>  | <span data-ttu-id="21266-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="21266-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21266-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="21266-127">Request body</span></span>
<span data-ttu-id="21266-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="21266-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21266-129">応答</span><span class="sxs-lookup"><span data-stu-id="21266-129">Response</span></span>

<span data-ttu-id="21266-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="21266-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21266-131">例</span><span class="sxs-lookup"><span data-stu-id="21266-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21266-132">要求</span><span class="sxs-lookup"><span data-stu-id="21266-132">Request</span></span>
<span data-ttu-id="21266-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21266-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21266-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="21266-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21266-135">C#</span><span class="sxs-lookup"><span data-stu-id="21266-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21266-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="21266-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21266-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21266-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21266-138">Java</span><span class="sxs-lookup"><span data-stu-id="21266-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21266-139">応答</span><span class="sxs-lookup"><span data-stu-id="21266-139">Response</span></span>
<span data-ttu-id="21266-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21266-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
