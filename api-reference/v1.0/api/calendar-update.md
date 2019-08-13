---
title: 予定表を更新する
description: '予定表オブジェクトのプロパティを更新します。 予定表はユーザー用にすることができます。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3365f5bba057c1bb46c7475b661de02ddc36cafe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369137"
---
# <a name="update-calendar"></a><span data-ttu-id="bff48-104">予定表を更新する</span><span class="sxs-lookup"><span data-stu-id="bff48-104">Update calendar</span></span>

<span data-ttu-id="bff48-105">[予定表](../resources/calendar.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bff48-105">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="bff48-106">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="bff48-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bff48-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bff48-107">Permissions</span></span>
<span data-ttu-id="bff48-108">この API を呼び出すには、イベントが含まれる予定表の種類と、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次のいずれかのアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="bff48-108">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="bff48-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bff48-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bff48-110">カレンダー</span><span class="sxs-lookup"><span data-stu-id="bff48-110">Calendar</span></span> | <span data-ttu-id="bff48-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bff48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bff48-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bff48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bff48-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bff48-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="bff48-114">ユーザーの予定表</span><span class="sxs-lookup"><span data-stu-id="bff48-114">user calendar</span></span> | <span data-ttu-id="bff48-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff48-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="bff48-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff48-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="bff48-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff48-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="bff48-118">グループ calendar</span><span class="sxs-lookup"><span data-stu-id="bff48-118">group calendar</span></span> | <span data-ttu-id="bff48-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff48-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="bff48-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bff48-120">Not supported.</span></span> | <span data-ttu-id="bff48-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bff48-121">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="bff48-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bff48-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="bff48-123">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bff48-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="bff48-124">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bff48-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="bff48-125">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bff48-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bff48-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bff48-126">Request headers</span></span>
| <span data-ttu-id="bff48-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bff48-127">Header</span></span>       | <span data-ttu-id="bff48-128">値</span><span class="sxs-lookup"><span data-stu-id="bff48-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bff48-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="bff48-129">Authorization</span></span>  | <span data-ttu-id="bff48-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bff48-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bff48-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bff48-132">Content-Type</span></span>  | <span data-ttu-id="bff48-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bff48-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bff48-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="bff48-135">Request body</span></span>
<span data-ttu-id="bff48-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bff48-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bff48-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff48-139">Property</span></span>     | <span data-ttu-id="bff48-140">型</span><span class="sxs-lookup"><span data-stu-id="bff48-140">Type</span></span>   |<span data-ttu-id="bff48-141">説明</span><span class="sxs-lookup"><span data-stu-id="bff48-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bff48-142">color</span><span class="sxs-lookup"><span data-stu-id="bff48-142">color</span></span>|<span data-ttu-id="bff48-143">String</span><span class="sxs-lookup"><span data-stu-id="bff48-143">String</span></span>|<span data-ttu-id="bff48-p107">UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1</span><span class="sxs-lookup"><span data-stu-id="bff48-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="bff48-146">name</span><span class="sxs-lookup"><span data-stu-id="bff48-146">name</span></span>|<span data-ttu-id="bff48-147">String</span><span class="sxs-lookup"><span data-stu-id="bff48-147">String</span></span>|<span data-ttu-id="bff48-148">予定表の名前。</span><span class="sxs-lookup"><span data-stu-id="bff48-148">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="bff48-149">応答</span><span class="sxs-lookup"><span data-stu-id="bff48-149">Response</span></span>

<span data-ttu-id="bff48-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bff48-150">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bff48-151">例</span><span class="sxs-lookup"><span data-stu-id="bff48-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bff48-152">要求</span><span class="sxs-lookup"><span data-stu-id="bff48-152">Request</span></span>
<span data-ttu-id="bff48-153">次の例では、サインインしているユーザーの既定の予定表の名前を更新します。</span><span class="sxs-lookup"><span data-stu-id="bff48-153">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bff48-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bff48-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bff48-155">C#</span><span class="sxs-lookup"><span data-stu-id="bff48-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bff48-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bff48-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bff48-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="bff48-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bff48-158">Java</span><span class="sxs-lookup"><span data-stu-id="bff48-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bff48-159">応答</span><span class="sxs-lookup"><span data-stu-id="bff48-159">Response</span></span>
<span data-ttu-id="bff48-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bff48-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
