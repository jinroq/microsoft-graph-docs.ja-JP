# <a name="update-calendar"></a><span data-ttu-id="0d194-101">Update calendar</span><span class="sxs-lookup"><span data-stu-id="0d194-101">Update calendar</span></span>

<span data-ttu-id="0d194-102">予定表オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d194-102">Update the properties of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d194-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d194-103">Permissions</span></span>
<span data-ttu-id="0d194-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d194-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d194-106">Permission type</span></span>      | <span data-ttu-id="0d194-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d194-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d194-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d194-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0d194-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d194-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0d194-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d194-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d194-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d194-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0d194-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d194-112">Application</span></span> | <span data-ttu-id="0d194-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d194-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d194-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d194-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0d194-115">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0d194-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="0d194-116">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0d194-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="0d194-117">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0d194-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d194-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d194-118">Request headers</span></span>
| <span data-ttu-id="0d194-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d194-119">Header</span></span>       | <span data-ttu-id="0d194-120">値</span><span class="sxs-lookup"><span data-stu-id="0d194-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d194-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d194-121">Authorization</span></span>  | <span data-ttu-id="0d194-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0d194-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d194-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d194-124">Content-Type</span></span>  | <span data-ttu-id="0d194-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d194-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d194-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d194-127">Request body</span></span>
<span data-ttu-id="0d194-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0d194-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d194-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d194-131">Property</span></span>     | <span data-ttu-id="0d194-132">型</span><span class="sxs-lookup"><span data-stu-id="0d194-132">Type</span></span>   |<span data-ttu-id="0d194-133">説明</span><span class="sxs-lookup"><span data-stu-id="0d194-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d194-134">color</span><span class="sxs-lookup"><span data-stu-id="0d194-134">color</span></span>|<span data-ttu-id="0d194-135">String</span><span class="sxs-lookup"><span data-stu-id="0d194-135">String</span></span>|<span data-ttu-id="0d194-p105">UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1</span><span class="sxs-lookup"><span data-stu-id="0d194-p105">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="0d194-138">name</span><span class="sxs-lookup"><span data-stu-id="0d194-138">name</span></span>|<span data-ttu-id="0d194-139">String</span><span class="sxs-lookup"><span data-stu-id="0d194-139">String</span></span>|<span data-ttu-id="0d194-140">予定表の名前。</span><span class="sxs-lookup"><span data-stu-id="0d194-140">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="0d194-141">応答</span><span class="sxs-lookup"><span data-stu-id="0d194-141">Response</span></span>

<span data-ttu-id="0d194-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d194-142">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d194-143">例</span><span class="sxs-lookup"><span data-stu-id="0d194-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d194-144">要求</span><span class="sxs-lookup"><span data-stu-id="0d194-144">Request</span></span>
<span data-ttu-id="0d194-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d194-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0d194-146">応答</span><span class="sxs-lookup"><span data-stu-id="0d194-146">Response</span></span>
<span data-ttu-id="0d194-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d194-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
