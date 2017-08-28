# <a name="update-calendargroup"></a><span data-ttu-id="9284b-101">CalendarGroup を更新する　</span><span class="sxs-lookup"><span data-stu-id="9284b-101">Update calendargroup</span></span>

<span data-ttu-id="9284b-102">calendargroup オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9284b-102">Update the properties of calendargroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9284b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9284b-103">Permissions</span></span>
<span data-ttu-id="9284b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9284b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9284b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9284b-106">Permission type</span></span>      | <span data-ttu-id="9284b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9284b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9284b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9284b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9284b-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9284b-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9284b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9284b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9284b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9284b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9284b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9284b-112">Application</span></span> | <span data-ttu-id="9284b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9284b-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9284b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9284b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9284b-115">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="9284b-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9284b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9284b-116">Request headers</span></span>
| <span data-ttu-id="9284b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9284b-117">Header</span></span>       | <span data-ttu-id="9284b-118">値</span><span class="sxs-lookup"><span data-stu-id="9284b-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9284b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9284b-119">Authorization</span></span>  | <span data-ttu-id="9284b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9284b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9284b-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9284b-122">Content-Type</span></span>  | <span data-ttu-id="9284b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9284b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9284b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9284b-125">Request body</span></span>
<span data-ttu-id="9284b-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9284b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9284b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9284b-129">Property</span></span>     | <span data-ttu-id="9284b-130">型</span><span class="sxs-lookup"><span data-stu-id="9284b-130">Type</span></span>   |<span data-ttu-id="9284b-131">説明</span><span class="sxs-lookup"><span data-stu-id="9284b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9284b-132">name</span><span class="sxs-lookup"><span data-stu-id="9284b-132">name</span></span>|<span data-ttu-id="9284b-133">String</span><span class="sxs-lookup"><span data-stu-id="9284b-133">String</span></span>|<span data-ttu-id="9284b-134">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="9284b-134">The group name.</span></span>|

## <a name="response"></a><span data-ttu-id="9284b-135">応答</span><span class="sxs-lookup"><span data-stu-id="9284b-135">Response</span></span>

<span data-ttu-id="9284b-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表グループ](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9284b-136">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9284b-137">例</span><span class="sxs-lookup"><span data-stu-id="9284b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9284b-138">要求</span><span class="sxs-lookup"><span data-stu-id="9284b-138">Request</span></span>
<span data-ttu-id="9284b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9284b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="9284b-140">応答</span><span class="sxs-lookup"><span data-stu-id="9284b-140">Response</span></span>
<span data-ttu-id="9284b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9284b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
