---
title: メッセージを一覧表示する
description: サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。
localization_priority: Priority
ms.openlocfilehash: a58d6e3c51cf85992129b3ba9c8e3996fa9841f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825369"
---
# <a name="list-messages"></a><span data-ttu-id="1ffb7-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1ffb7-103">List messages</span></span>

<span data-ttu-id="1ffb7-104">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ffb7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ffb7-105">Permissions</span></span>
<span data-ttu-id="1ffb7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ffb7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ffb7-108">Permission type</span></span>      | <span data-ttu-id="1ffb7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ffb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ffb7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ffb7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ffb7-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ffb7-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ffb7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ffb7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ffb7-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ffb7-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ffb7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ffb7-114">Application</span></span> | <span data-ttu-id="1ffb7-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ffb7-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ffb7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ffb7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ffb7-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1ffb7-117">Optional query parameters</span></span>
<span data-ttu-id="1ffb7-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1ffb7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ffb7-119">Request headers</span></span>
| <span data-ttu-id="1ffb7-120">名前</span><span class="sxs-lookup"><span data-stu-id="1ffb7-120">Name</span></span>       | <span data-ttu-id="1ffb7-121">種類</span><span class="sxs-lookup"><span data-stu-id="1ffb7-121">Type</span></span> | <span data-ttu-id="1ffb7-122">説明</span><span class="sxs-lookup"><span data-stu-id="1ffb7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ffb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ffb7-123">Authorization</span></span>  | <span data-ttu-id="1ffb7-124">string</span><span class="sxs-lookup"><span data-stu-id="1ffb7-124">string</span></span>  | <span data-ttu-id="1ffb7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ffb7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ffb7-127">Request body</span></span>
<span data-ttu-id="1ffb7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ffb7-129">応答</span><span class="sxs-lookup"><span data-stu-id="1ffb7-129">Response</span></span>

<span data-ttu-id="1ffb7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ffb7-131">例</span><span class="sxs-lookup"><span data-stu-id="1ffb7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ffb7-132">要求</span><span class="sxs-lookup"><span data-stu-id="1ffb7-132">Request</span></span>
<span data-ttu-id="1ffb7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="1ffb7-134">応答</span><span class="sxs-lookup"><span data-stu-id="1ffb7-134">Response</span></span>
<span data-ttu-id="1ffb7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ffb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
