---
title: 添付ファイルを一覧表示する
description: メッセージに添付された添付ファイル オブジェクトのリストを取得します。
author: angelgolfer-ms
ms.openlocfilehash: 9f083af679335eb0bf54fa9bd0eadfaa7a5a1250
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350867"
---
# <a name="list-attachments"></a><span data-ttu-id="54091-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="54091-103">List attachments</span></span>

> <span data-ttu-id="54091-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54091-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54091-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54091-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54091-106">メッセージに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="54091-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="54091-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54091-107">Permissions</span></span>
<span data-ttu-id="54091-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54091-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54091-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54091-110">Permission type</span></span>      | <span data-ttu-id="54091-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54091-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54091-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54091-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54091-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="54091-113">Mail.Read</span></span>    |
|<span data-ttu-id="54091-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54091-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54091-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="54091-115">Mail.Read</span></span>    |
|<span data-ttu-id="54091-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54091-116">Application</span></span> | <span data-ttu-id="54091-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="54091-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="54091-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54091-118">HTTP request</span></span>
<span data-ttu-id="54091-119"><!-- { "blockType": "ignored" } -->ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="54091-119"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="54091-120">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="54091-120">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="54091-p103">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="54091-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54091-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="54091-123">Optional query parameters</span></span>
<span data-ttu-id="54091-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="54091-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="54091-125">$ を使用する具体的には、メッセージのプロパティの残りの部分にインラインでメッセージの添付ファイルをすべてのクエリ パラメーターを展開します。</span><span class="sxs-lookup"><span data-stu-id="54091-125">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="54091-126">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="54091-126">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="54091-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54091-127">Request headers</span></span>
| <span data-ttu-id="54091-128">名前</span><span class="sxs-lookup"><span data-stu-id="54091-128">Name</span></span>       | <span data-ttu-id="54091-129">種類</span><span class="sxs-lookup"><span data-stu-id="54091-129">Type</span></span> | <span data-ttu-id="54091-130">説明</span><span class="sxs-lookup"><span data-stu-id="54091-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54091-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="54091-131">Authorization</span></span>  | <span data-ttu-id="54091-132">string</span><span class="sxs-lookup"><span data-stu-id="54091-132">string</span></span>  | <span data-ttu-id="54091-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54091-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54091-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="54091-135">Request body</span></span>
<span data-ttu-id="54091-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54091-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54091-137">応答</span><span class="sxs-lookup"><span data-stu-id="54091-137">Response</span></span>

<span data-ttu-id="54091-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="54091-138">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54091-139">例</span><span class="sxs-lookup"><span data-stu-id="54091-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54091-140">要求</span><span class="sxs-lookup"><span data-stu-id="54091-140">Request</span></span>
<span data-ttu-id="54091-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54091-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="54091-142">応答</span><span class="sxs-lookup"><span data-stu-id="54091-142">Response</span></span>
<span data-ttu-id="54091-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54091-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->