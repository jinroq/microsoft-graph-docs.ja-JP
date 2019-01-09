---
title: 添付ファイルを一覧表示する
description: イベントに添付された添付ファイル オブジェクトのリストを取得します。
author: angelgolfer-ms
ms.openlocfilehash: 57545b89adc5cbb3c20ab782de04438b7b5ba9bf
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771801"
---
# <a name="list-attachments"></a><span data-ttu-id="2af22-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2af22-103">List attachments</span></span>

> <span data-ttu-id="2af22-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2af22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2af22-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2af22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2af22-106">イベントに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2af22-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="2af22-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2af22-107">Permissions</span></span>

<span data-ttu-id="2af22-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2af22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2af22-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2af22-110">Permission type</span></span>      | <span data-ttu-id="2af22-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2af22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2af22-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2af22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2af22-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af22-113">Calendars.Read</span></span>    |
|<span data-ttu-id="2af22-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2af22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2af22-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af22-115">Calendars.Read</span></span>    |
|<span data-ttu-id="2af22-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2af22-116">Application</span></span> | <span data-ttu-id="2af22-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2af22-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2af22-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2af22-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="2af22-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2af22-119">Optional query parameters</span></span>

<span data-ttu-id="2af22-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2af22-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2af22-121">具体的には、使用することができます、 `$expand` 、イベントの添付ファイルにインライン イベント プロパティの残りの部分のすべてのパラメーターのクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="2af22-121">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="2af22-122">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="2af22-122">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="2af22-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2af22-123">Request headers</span></span>

| <span data-ttu-id="2af22-124">名前</span><span class="sxs-lookup"><span data-stu-id="2af22-124">Name</span></span>       | <span data-ttu-id="2af22-125">型</span><span class="sxs-lookup"><span data-stu-id="2af22-125">Type</span></span> | <span data-ttu-id="2af22-126">説明</span><span class="sxs-lookup"><span data-stu-id="2af22-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2af22-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af22-127">Authorization</span></span>  | <span data-ttu-id="2af22-128">string</span><span class="sxs-lookup"><span data-stu-id="2af22-128">string</span></span>  | <span data-ttu-id="2af22-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2af22-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2af22-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2af22-131">Request body</span></span>

<span data-ttu-id="2af22-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2af22-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2af22-133">応答</span><span class="sxs-lookup"><span data-stu-id="2af22-133">Response</span></span>

<span data-ttu-id="2af22-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2af22-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af22-135">例</span><span class="sxs-lookup"><span data-stu-id="2af22-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="2af22-136">要求</span><span class="sxs-lookup"><span data-stu-id="2af22-136">Request</span></span>

<span data-ttu-id="2af22-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2af22-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="2af22-138">応答</span><span class="sxs-lookup"><span data-stu-id="2af22-138">Response</span></span>

<span data-ttu-id="2af22-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2af22-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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