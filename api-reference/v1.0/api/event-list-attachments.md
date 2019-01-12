---
title: 添付ファイルを一覧表示する
description: イベントに添付された添付ファイル オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2323cc525af1c01c674ac088c65938186749b051
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965930"
---
# <a name="list-attachments"></a><span data-ttu-id="7baaa-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7baaa-103">List attachments</span></span>

<span data-ttu-id="7baaa-104">イベントに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7baaa-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="7baaa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7baaa-105">Permissions</span></span>
<span data-ttu-id="7baaa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7baaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7baaa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7baaa-108">Permission type</span></span>      | <span data-ttu-id="7baaa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7baaa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7baaa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7baaa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7baaa-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7baaa-111">Calendars.Read</span></span>    |
|<span data-ttu-id="7baaa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7baaa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7baaa-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7baaa-113">Calendars.Read</span></span>    |
|<span data-ttu-id="7baaa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7baaa-114">Application</span></span> | <span data-ttu-id="7baaa-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7baaa-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7baaa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7baaa-116">HTTP request</span></span>
<span data-ttu-id="7baaa-117">ユーザーの既定の[予定表](../resources/calendar.md)に[イベント](../resources/event.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="7baaa-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="7baaa-118">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="7baaa-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="7baaa-119">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="7baaa-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7baaa-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7baaa-120">Optional query parameters</span></span>
<span data-ttu-id="7baaa-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7baaa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7baaa-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7baaa-122">Request headers</span></span>
| <span data-ttu-id="7baaa-123">名前</span><span class="sxs-lookup"><span data-stu-id="7baaa-123">Name</span></span>       | <span data-ttu-id="7baaa-124">種類</span><span class="sxs-lookup"><span data-stu-id="7baaa-124">Type</span></span> | <span data-ttu-id="7baaa-125">説明</span><span class="sxs-lookup"><span data-stu-id="7baaa-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7baaa-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7baaa-126">Authorization</span></span>  | <span data-ttu-id="7baaa-127">string</span><span class="sxs-lookup"><span data-stu-id="7baaa-127">string</span></span>  | <span data-ttu-id="7baaa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7baaa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7baaa-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="7baaa-130">Request body</span></span>
<span data-ttu-id="7baaa-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7baaa-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7baaa-132">応答</span><span class="sxs-lookup"><span data-stu-id="7baaa-132">Response</span></span>

<span data-ttu-id="7baaa-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7baaa-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7baaa-134">例</span><span class="sxs-lookup"><span data-stu-id="7baaa-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7baaa-135">要求</span><span class="sxs-lookup"><span data-stu-id="7baaa-135">Request</span></span>
<span data-ttu-id="7baaa-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7baaa-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="7baaa-137">応答</span><span class="sxs-lookup"><span data-stu-id="7baaa-137">Response</span></span>
<span data-ttu-id="7baaa-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7baaa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
