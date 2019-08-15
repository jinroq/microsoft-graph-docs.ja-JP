---
title: 予定表を取得する
description: '予定表オブジェクトのプロパティと関係を取得します。 予定表はユーザー用にすることができます。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f1510d6009a0a0fe7585ef5c21ce4db2864d3fca
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419161"
---
# <a name="get-calendar"></a><span data-ttu-id="83413-104">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="83413-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83413-105">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="83413-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="83413-106">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="83413-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="83413-107">アプリで別のユーザーの予定表を取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="83413-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="83413-108">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="83413-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="83413-109">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーと予定表を共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="83413-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="83413-110">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83413-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="83413-111">権限</span><span class="sxs-lookup"><span data-stu-id="83413-111">Permissions</span></span>
<span data-ttu-id="83413-112">この API を呼び出すには、イベントが含まれる予定表の種類と、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次のいずれかのアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="83413-112">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="83413-113">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83413-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83413-114">カレンダー</span><span class="sxs-lookup"><span data-stu-id="83413-114">Calendar</span></span> | <span data-ttu-id="83413-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83413-115">Delegated (work or school account)</span></span> | <span data-ttu-id="83413-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83413-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83413-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83413-117">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="83413-118">ユーザーの予定表</span><span class="sxs-lookup"><span data-stu-id="83413-118">user calendar</span></span> | <span data-ttu-id="83413-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83413-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="83413-120">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83413-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="83413-121">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83413-121">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="83413-122">グループ calendar</span><span class="sxs-lookup"><span data-stu-id="83413-122">group calendar</span></span> | <span data-ttu-id="83413-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83413-123">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="83413-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83413-124">Not supported.</span></span> | <span data-ttu-id="83413-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83413-125">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="83413-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83413-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="83413-127">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="83413-127">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="83413-128">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="83413-128">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="83413-129">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="83413-129">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83413-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83413-130">Optional query parameters</span></span>
<span data-ttu-id="83413-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83413-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83413-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83413-132">Request headers</span></span>
| <span data-ttu-id="83413-133">名前</span><span class="sxs-lookup"><span data-stu-id="83413-133">Name</span></span>       | <span data-ttu-id="83413-134">型</span><span class="sxs-lookup"><span data-stu-id="83413-134">Type</span></span> | <span data-ttu-id="83413-135">説明</span><span class="sxs-lookup"><span data-stu-id="83413-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="83413-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="83413-136">Authorization</span></span>  | <span data-ttu-id="83413-137">string</span><span class="sxs-lookup"><span data-stu-id="83413-137">string</span></span>  | <span data-ttu-id="83413-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83413-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83413-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="83413-140">Request body</span></span>
<span data-ttu-id="83413-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83413-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83413-142">応答</span><span class="sxs-lookup"><span data-stu-id="83413-142">Response</span></span>

<span data-ttu-id="83413-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83413-143">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83413-144">例</span><span class="sxs-lookup"><span data-stu-id="83413-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83413-145">要求</span><span class="sxs-lookup"><span data-stu-id="83413-145">Request</span></span>
<span data-ttu-id="83413-146">次の例では、サインインしているユーザーの既定の予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="83413-146">The following example gets the signed-in user's default calendar.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83413-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83413-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83413-148">C#</span><span class="sxs-lookup"><span data-stu-id="83413-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83413-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83413-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83413-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="83413-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83413-151">応答</span><span class="sxs-lookup"><span data-stu-id="83413-151">Response</span></span>
<span data-ttu-id="83413-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83413-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
