---
title: 添付ファイルを一覧表示する
description: メッセージに添付された添付フィル オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4a5b9130a562ff15b1a9c13106c0528246805ce4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346913"
---
# <a name="list-attachments"></a><span data-ttu-id="b218c-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b218c-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b218c-104">メッセージに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b218c-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="b218c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b218c-105">Permissions</span></span>
<span data-ttu-id="b218c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b218c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b218c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b218c-108">Permission type</span></span>      | <span data-ttu-id="b218c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b218c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b218c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b218c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b218c-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b218c-111">Mail.Read</span></span>    |
|<span data-ttu-id="b218c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b218c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b218c-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b218c-113">Mail.Read</span></span>    |
|<span data-ttu-id="b218c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b218c-114">Application</span></span> | <span data-ttu-id="b218c-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b218c-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b218c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b218c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b218c-117">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b218c-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="b218c-118">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b218c-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="b218c-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="b218c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b218c-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b218c-121">Optional query parameters</span></span>
<span data-ttu-id="b218c-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b218c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b218c-123">特に、$expand クエリパラメーターを使用して、メッセージのすべての添付ファイルを他のメッセージプロパティと共にインラインに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b218c-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="b218c-124">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="b218c-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="b218c-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b218c-125">Request headers</span></span>
| <span data-ttu-id="b218c-126">名前</span><span class="sxs-lookup"><span data-stu-id="b218c-126">Name</span></span>       | <span data-ttu-id="b218c-127">型</span><span class="sxs-lookup"><span data-stu-id="b218c-127">Type</span></span> | <span data-ttu-id="b218c-128">説明</span><span class="sxs-lookup"><span data-stu-id="b218c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b218c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b218c-129">Authorization</span></span>  | <span data-ttu-id="b218c-130">string</span><span class="sxs-lookup"><span data-stu-id="b218c-130">string</span></span>  | <span data-ttu-id="b218c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b218c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b218c-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="b218c-133">Request body</span></span>
<span data-ttu-id="b218c-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b218c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b218c-135">応答</span><span class="sxs-lookup"><span data-stu-id="b218c-135">Response</span></span>

<span data-ttu-id="b218c-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b218c-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b218c-137">例</span><span class="sxs-lookup"><span data-stu-id="b218c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b218c-138">要求</span><span class="sxs-lookup"><span data-stu-id="b218c-138">Request</span></span>
<span data-ttu-id="b218c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b218c-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b218c-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b218c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b218c-141">C#</span><span class="sxs-lookup"><span data-stu-id="b218c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b218c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b218c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b218c-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="b218c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b218c-144">Java</span><span class="sxs-lookup"><span data-stu-id="b218c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b218c-145">応答</span><span class="sxs-lookup"><span data-stu-id="b218c-145">Response</span></span>
<span data-ttu-id="b218c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b218c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
