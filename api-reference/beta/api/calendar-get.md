---
title: 予定表を取得する
description: '予定表オブジェクトのプロパティと関係を取得します。 カレンダーには、ユーザーのいずれかを指定できます。 '
ms.openlocfilehash: b4dd218e25d154fa1641a7a62d3b79790a15f7da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066442"
---
# <a name="get-calendar"></a><span data-ttu-id="d821e-104">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="d821e-104">Get calendar</span></span>

> <span data-ttu-id="d821e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d821e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d821e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d821e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d821e-107">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d821e-107">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="d821e-108">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d821e-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="d821e-109">アプリケーションが別のユーザーの予定表を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="d821e-109">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="d821e-110">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="d821e-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d821e-111">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="d821e-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d821e-112">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d821e-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="d821e-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d821e-113">Permissions</span></span>
<span data-ttu-id="d821e-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d821e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d821e-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d821e-116">Permission type</span></span>      | <span data-ttu-id="d821e-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d821e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d821e-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d821e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d821e-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d821e-119">Calendars.Read</span></span>    |
|<span data-ttu-id="d821e-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d821e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d821e-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d821e-121">Calendars.Read</span></span>    |
|<span data-ttu-id="d821e-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d821e-122">Application</span></span> | <span data-ttu-id="d821e-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d821e-123">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d821e-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d821e-124">HTTP request</span></span>
<span data-ttu-id="d821e-125"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="d821e-125"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="d821e-126">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d821e-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="d821e-127">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d821e-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d821e-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d821e-128">Optional query parameters</span></span>
<span data-ttu-id="d821e-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d821e-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d821e-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d821e-130">Request headers</span></span>
| <span data-ttu-id="d821e-131">名前</span><span class="sxs-lookup"><span data-stu-id="d821e-131">Name</span></span>       | <span data-ttu-id="d821e-132">型</span><span class="sxs-lookup"><span data-stu-id="d821e-132">Type</span></span> | <span data-ttu-id="d821e-133">説明</span><span class="sxs-lookup"><span data-stu-id="d821e-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d821e-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d821e-134">Authorization</span></span>  | <span data-ttu-id="d821e-135">string</span><span class="sxs-lookup"><span data-stu-id="d821e-135">string</span></span>  | <span data-ttu-id="d821e-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d821e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d821e-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="d821e-138">Request body</span></span>
<span data-ttu-id="d821e-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d821e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d821e-140">応答</span><span class="sxs-lookup"><span data-stu-id="d821e-140">Response</span></span>

<span data-ttu-id="d821e-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d821e-141">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d821e-142">例</span><span class="sxs-lookup"><span data-stu-id="d821e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d821e-143">要求</span><span class="sxs-lookup"><span data-stu-id="d821e-143">Request</span></span>
<span data-ttu-id="d821e-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d821e-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="d821e-145">応答</span><span class="sxs-lookup"><span data-stu-id="d821e-145">Response</span></span>
<span data-ttu-id="d821e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d821e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
