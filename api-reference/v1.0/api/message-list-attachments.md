---
title: 添付ファイルを一覧表示する
description: メッセージに添付された添付ファイル オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 2e37e863d4b050a07b756b91f1e98a4349239154
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918122"
---
# <a name="list-attachments"></a><span data-ttu-id="12911-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="12911-103">List attachments</span></span>

<span data-ttu-id="12911-104">メッセージに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="12911-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="12911-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12911-105">Permissions</span></span>
<span data-ttu-id="12911-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12911-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12911-108">Permission type</span></span>      | <span data-ttu-id="12911-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12911-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12911-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12911-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12911-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12911-111">Mail.Read</span></span>    |
|<span data-ttu-id="12911-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12911-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12911-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12911-113">Mail.Read</span></span>    |
|<span data-ttu-id="12911-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12911-114">Application</span></span> | <span data-ttu-id="12911-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12911-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="12911-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12911-116">HTTP request</span></span>
<span data-ttu-id="12911-117"><!-- { "blockType": "ignored" } -->ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="12911-117"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="12911-118">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="12911-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="12911-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="12911-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12911-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="12911-121">Optional query parameters</span></span>
<span data-ttu-id="12911-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="12911-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12911-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12911-123">Request headers</span></span>
| <span data-ttu-id="12911-124">名前</span><span class="sxs-lookup"><span data-stu-id="12911-124">Name</span></span>       | <span data-ttu-id="12911-125">型</span><span class="sxs-lookup"><span data-stu-id="12911-125">Type</span></span> | <span data-ttu-id="12911-126">説明</span><span class="sxs-lookup"><span data-stu-id="12911-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="12911-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="12911-127">Authorization</span></span>  | <span data-ttu-id="12911-128">string</span><span class="sxs-lookup"><span data-stu-id="12911-128">string</span></span>  | <span data-ttu-id="12911-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12911-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12911-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="12911-131">Request body</span></span>
<span data-ttu-id="12911-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12911-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12911-133">応答</span><span class="sxs-lookup"><span data-stu-id="12911-133">Response</span></span>

<span data-ttu-id="12911-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="12911-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12911-135">例</span><span class="sxs-lookup"><span data-stu-id="12911-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12911-136">要求</span><span class="sxs-lookup"><span data-stu-id="12911-136">Request</span></span>
<span data-ttu-id="12911-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12911-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="12911-138">応答</span><span class="sxs-lookup"><span data-stu-id="12911-138">Response</span></span>
<span data-ttu-id="12911-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12911-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
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
