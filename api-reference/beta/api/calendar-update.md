---
title: 予定表を更新する
description: '予定表オブジェクトのプロパティを更新します。 カレンダーには、ユーザーのいずれかを指定できます。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a9b9ac65fa5d03b73a7508f6032ebe199118b09c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922495"
---
# <a name="update-calendar"></a><span data-ttu-id="692ff-104">予定表を更新する</span><span class="sxs-lookup"><span data-stu-id="692ff-104">Update calendar</span></span>

> <span data-ttu-id="692ff-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="692ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="692ff-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="692ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="692ff-107">[予定表](../resources/calendar.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="692ff-107">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="692ff-108">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="692ff-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="692ff-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="692ff-109">Permissions</span></span>
<span data-ttu-id="692ff-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="692ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="692ff-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="692ff-112">Permission type</span></span>      | <span data-ttu-id="692ff-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="692ff-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="692ff-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="692ff-114">Delegated (work or school account)</span></span> | <span data-ttu-id="692ff-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="692ff-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="692ff-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="692ff-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="692ff-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="692ff-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="692ff-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="692ff-118">Application</span></span> | <span data-ttu-id="692ff-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="692ff-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="692ff-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="692ff-120">HTTP request</span></span>
<span data-ttu-id="692ff-121"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="692ff-121"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="692ff-122">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="692ff-122">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="692ff-123">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="692ff-123">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="692ff-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="692ff-124">Request headers</span></span>
| <span data-ttu-id="692ff-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="692ff-125">Header</span></span>       | <span data-ttu-id="692ff-126">値</span><span class="sxs-lookup"><span data-stu-id="692ff-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="692ff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="692ff-127">Authorization</span></span>  | <span data-ttu-id="692ff-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="692ff-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="692ff-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="692ff-130">Content-Type</span></span>  | <span data-ttu-id="692ff-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="692ff-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="692ff-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="692ff-133">Request body</span></span>
<span data-ttu-id="692ff-p107">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="692ff-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="692ff-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="692ff-137">Property</span></span>     | <span data-ttu-id="692ff-138">型</span><span class="sxs-lookup"><span data-stu-id="692ff-138">Type</span></span>   |<span data-ttu-id="692ff-139">説明</span><span class="sxs-lookup"><span data-stu-id="692ff-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="692ff-140">color</span><span class="sxs-lookup"><span data-stu-id="692ff-140">color</span></span>|<span data-ttu-id="692ff-141">String</span><span class="sxs-lookup"><span data-stu-id="692ff-141">String</span></span>|<span data-ttu-id="692ff-p108">UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1</span><span class="sxs-lookup"><span data-stu-id="692ff-p108">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="692ff-144">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="692ff-144">isDefaultCalendar</span></span>|<span data-ttu-id="692ff-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="692ff-145">Boolean</span></span>|<span data-ttu-id="692ff-146">この予定表がユーザーの既定の予定表であれば True、そうでなければ False。</span><span class="sxs-lookup"><span data-stu-id="692ff-146">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="692ff-147">名前</span><span class="sxs-lookup"><span data-stu-id="692ff-147">name</span></span>|<span data-ttu-id="692ff-148">String</span><span class="sxs-lookup"><span data-stu-id="692ff-148">String</span></span>|<span data-ttu-id="692ff-149">予定表の名前。</span><span class="sxs-lookup"><span data-stu-id="692ff-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="692ff-150">応答</span><span class="sxs-lookup"><span data-stu-id="692ff-150">Response</span></span>

<span data-ttu-id="692ff-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="692ff-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="692ff-152">例</span><span class="sxs-lookup"><span data-stu-id="692ff-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="692ff-153">要求</span><span class="sxs-lookup"><span data-stu-id="692ff-153">Request</span></span>
<span data-ttu-id="692ff-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="692ff-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
##### <a name="response"></a><span data-ttu-id="692ff-155">応答</span><span class="sxs-lookup"><span data-stu-id="692ff-155">Response</span></span>
<span data-ttu-id="692ff-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="692ff-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "hexColor": "",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
