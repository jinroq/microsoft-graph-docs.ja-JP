---
title: 予定表を取得する
description: '予定表オブジェクトのプロパティと関係を取得します。 予定表は、ユーザーに対して1つにすることができます。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4f277fa6cd9621ddcf3a5374594ede7a2417334a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462089"
---
# <a name="get-calendar"></a><span data-ttu-id="c6463-104">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="c6463-104">Get calendar</span></span>

<span data-ttu-id="c6463-105">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6463-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="c6463-106">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="c6463-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="c6463-107">アプリが別のユーザーの予定表を取得するには、次の2つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="c6463-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="c6463-108">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="c6463-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c6463-109">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーと予定表を共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="c6463-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c6463-110">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6463-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6463-111">権限</span><span class="sxs-lookup"><span data-stu-id="c6463-111">Permissions</span></span>
<span data-ttu-id="c6463-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6463-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6463-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6463-114">Permission type</span></span>      | <span data-ttu-id="c6463-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6463-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6463-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6463-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c6463-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c6463-117">Calendars.Read</span></span>    |
|<span data-ttu-id="c6463-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6463-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6463-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c6463-119">Calendars.Read</span></span>    |
|<span data-ttu-id="c6463-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6463-120">Application</span></span> | <span data-ttu-id="c6463-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c6463-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6463-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6463-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c6463-123">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="c6463-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="c6463-124">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="c6463-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="c6463-125">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="c6463-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6463-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6463-126">Optional query parameters</span></span>
<span data-ttu-id="c6463-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c6463-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c6463-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6463-128">Request headers</span></span>
| <span data-ttu-id="c6463-129">名前</span><span class="sxs-lookup"><span data-stu-id="c6463-129">Name</span></span>       | <span data-ttu-id="c6463-130">型</span><span class="sxs-lookup"><span data-stu-id="c6463-130">Type</span></span> | <span data-ttu-id="c6463-131">説明</span><span class="sxs-lookup"><span data-stu-id="c6463-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c6463-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6463-132">Authorization</span></span>  | <span data-ttu-id="c6463-133">string</span><span class="sxs-lookup"><span data-stu-id="c6463-133">string</span></span>  | <span data-ttu-id="c6463-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c6463-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6463-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6463-136">Request body</span></span>
<span data-ttu-id="c6463-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c6463-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6463-138">応答</span><span class="sxs-lookup"><span data-stu-id="c6463-138">Response</span></span>

<span data-ttu-id="c6463-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c6463-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6463-140">例</span><span class="sxs-lookup"><span data-stu-id="c6463-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6463-141">要求</span><span class="sxs-lookup"><span data-stu-id="c6463-141">Request</span></span>
<span data-ttu-id="c6463-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6463-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="c6463-143">応答</span><span class="sxs-lookup"><span data-stu-id="c6463-143">Response</span></span>
<span data-ttu-id="c6463-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c6463-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
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
