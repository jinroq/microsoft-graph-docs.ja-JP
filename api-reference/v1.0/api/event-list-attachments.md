---
title: 添付ファイルを一覧表示する
description: イベントに添付された Attachment オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3ebb8c1f1395d20ac3bcbe80bff9b1fd166f98b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372011"
---
# <a name="list-attachments"></a><span data-ttu-id="25b3a-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="25b3a-103">List attachments</span></span>

<span data-ttu-id="25b3a-104">イベントに添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="25b3a-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="25b3a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="25b3a-105">Permissions</span></span>
<span data-ttu-id="25b3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b3a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="25b3a-108">Permission type</span></span>      | <span data-ttu-id="25b3a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="25b3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25b3a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="25b3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25b3a-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25b3a-111">Calendars.Read</span></span>    |
|<span data-ttu-id="25b3a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="25b3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25b3a-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25b3a-113">Calendars.Read</span></span>    |
|<span data-ttu-id="25b3a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="25b3a-114">Application</span></span> | <span data-ttu-id="25b3a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25b3a-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="25b3a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="25b3a-116">HTTP request</span></span>
<span data-ttu-id="25b3a-117">ユーザーの既定の[予定表](../resources/calendar.md)にある[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="25b3a-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="25b3a-118">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="25b3a-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="25b3a-119">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="25b3a-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25b3a-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="25b3a-120">Optional query parameters</span></span>
<span data-ttu-id="25b3a-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="25b3a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="25b3a-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="25b3a-122">Request headers</span></span>
| <span data-ttu-id="25b3a-123">名前</span><span class="sxs-lookup"><span data-stu-id="25b3a-123">Name</span></span>       | <span data-ttu-id="25b3a-124">型</span><span class="sxs-lookup"><span data-stu-id="25b3a-124">Type</span></span> | <span data-ttu-id="25b3a-125">説明</span><span class="sxs-lookup"><span data-stu-id="25b3a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25b3a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b3a-126">Authorization</span></span>  | <span data-ttu-id="25b3a-127">string</span><span class="sxs-lookup"><span data-stu-id="25b3a-127">string</span></span>  | <span data-ttu-id="25b3a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="25b3a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25b3a-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="25b3a-130">Request body</span></span>
<span data-ttu-id="25b3a-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="25b3a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b3a-132">応答</span><span class="sxs-lookup"><span data-stu-id="25b3a-132">Response</span></span>

<span data-ttu-id="25b3a-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="25b3a-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25b3a-134">例</span><span class="sxs-lookup"><span data-stu-id="25b3a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25b3a-135">要求</span><span class="sxs-lookup"><span data-stu-id="25b3a-135">Request</span></span>
<span data-ttu-id="25b3a-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="25b3a-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25b3a-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="25b3a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25b3a-138">C#</span><span class="sxs-lookup"><span data-stu-id="25b3a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25b3a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25b3a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25b3a-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="25b3a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="25b3a-141">Java</span><span class="sxs-lookup"><span data-stu-id="25b3a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="25b3a-142">応答</span><span class="sxs-lookup"><span data-stu-id="25b3a-142">Response</span></span>
<span data-ttu-id="25b3a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="25b3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
