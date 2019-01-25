---
title: 予定表を取得する
description: '予定表オブジェクトのプロパティと関係を取得します。 カレンダーには、ユーザーのいずれかを指定できます。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4f277fa6cd9621ddcf3a5374594ede7a2417334a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520495"
---
# <a name="get-calendar"></a><span data-ttu-id="32958-104">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="32958-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32958-105">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="32958-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="32958-106">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="32958-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="32958-107">アプリケーションが別のユーザーの予定表を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="32958-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="32958-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="32958-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="32958-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="32958-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="32958-110">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32958-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="32958-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32958-111">Permissions</span></span>
<span data-ttu-id="32958-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32958-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32958-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32958-114">Permission type</span></span>      | <span data-ttu-id="32958-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32958-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32958-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32958-116">Delegated (work or school account)</span></span> | <span data-ttu-id="32958-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="32958-117">Calendars.Read</span></span>    |
|<span data-ttu-id="32958-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32958-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32958-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="32958-119">Calendars.Read</span></span>    |
|<span data-ttu-id="32958-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32958-120">Application</span></span> | <span data-ttu-id="32958-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="32958-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="32958-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32958-122">HTTP request</span></span>
<span data-ttu-id="32958-123"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="32958-123"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="32958-124">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="32958-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="32958-125">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="32958-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32958-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="32958-126">Optional query parameters</span></span>
<span data-ttu-id="32958-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="32958-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32958-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32958-128">Request headers</span></span>
| <span data-ttu-id="32958-129">名前</span><span class="sxs-lookup"><span data-stu-id="32958-129">Name</span></span>       | <span data-ttu-id="32958-130">型</span><span class="sxs-lookup"><span data-stu-id="32958-130">Type</span></span> | <span data-ttu-id="32958-131">説明</span><span class="sxs-lookup"><span data-stu-id="32958-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32958-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="32958-132">Authorization</span></span>  | <span data-ttu-id="32958-133">string</span><span class="sxs-lookup"><span data-stu-id="32958-133">string</span></span>  | <span data-ttu-id="32958-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32958-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32958-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="32958-136">Request body</span></span>
<span data-ttu-id="32958-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="32958-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32958-138">応答</span><span class="sxs-lookup"><span data-stu-id="32958-138">Response</span></span>

<span data-ttu-id="32958-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32958-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32958-140">例</span><span class="sxs-lookup"><span data-stu-id="32958-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32958-141">要求</span><span class="sxs-lookup"><span data-stu-id="32958-141">Request</span></span>
<span data-ttu-id="32958-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32958-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="32958-143">応答</span><span class="sxs-lookup"><span data-stu-id="32958-143">Response</span></span>
<span data-ttu-id="32958-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32958-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
