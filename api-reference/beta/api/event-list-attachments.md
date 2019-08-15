---
title: 添付ファイルを一覧表示する
description: イベントに添付された Attachment オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 877bf30d5b715b6155edc1cb1eec4ec9d8438531
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420458"
---
# <a name="list-attachments"></a><span data-ttu-id="d54c0-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d54c0-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d54c0-104">イベントに添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d54c0-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="d54c0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d54c0-105">Permissions</span></span>

<span data-ttu-id="d54c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d54c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d54c0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d54c0-108">Permission type</span></span>      | <span data-ttu-id="d54c0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d54c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d54c0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d54c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d54c0-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d54c0-111">Calendars.Read</span></span>    |
|<span data-ttu-id="d54c0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d54c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d54c0-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d54c0-113">Calendars.Read</span></span>    |
|<span data-ttu-id="d54c0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d54c0-114">Application</span></span> | <span data-ttu-id="d54c0-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d54c0-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d54c0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d54c0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="d54c0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d54c0-117">Optional query parameters</span></span>

<span data-ttu-id="d54c0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d54c0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d54c0-119">特に、 `$expand`クエリパラメーターを使用して、イベントのすべての添付ファイルを、他のイベントプロパティと共にインラインに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d54c0-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="d54c0-120">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="d54c0-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="d54c0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d54c0-121">Request headers</span></span>

| <span data-ttu-id="d54c0-122">名前</span><span class="sxs-lookup"><span data-stu-id="d54c0-122">Name</span></span>       | <span data-ttu-id="d54c0-123">型</span><span class="sxs-lookup"><span data-stu-id="d54c0-123">Type</span></span> | <span data-ttu-id="d54c0-124">説明</span><span class="sxs-lookup"><span data-stu-id="d54c0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d54c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d54c0-125">Authorization</span></span>  | <span data-ttu-id="d54c0-126">string</span><span class="sxs-lookup"><span data-stu-id="d54c0-126">string</span></span>  | <span data-ttu-id="d54c0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d54c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d54c0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d54c0-129">Request body</span></span>

<span data-ttu-id="d54c0-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d54c0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d54c0-131">応答</span><span class="sxs-lookup"><span data-stu-id="d54c0-131">Response</span></span>

<span data-ttu-id="d54c0-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d54c0-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d54c0-133">例</span><span class="sxs-lookup"><span data-stu-id="d54c0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d54c0-134">要求</span><span class="sxs-lookup"><span data-stu-id="d54c0-134">Request</span></span>

<span data-ttu-id="d54c0-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d54c0-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d54c0-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d54c0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d54c0-137">C#</span><span class="sxs-lookup"><span data-stu-id="d54c0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d54c0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d54c0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d54c0-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="d54c0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d54c0-140">応答</span><span class="sxs-lookup"><span data-stu-id="d54c0-140">Response</span></span>

<span data-ttu-id="d54c0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d54c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
