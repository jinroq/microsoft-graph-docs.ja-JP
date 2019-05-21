---
title: 予定表を作成する
description: この API を使って、ユーザー用の予定表グループに新しい予定表を作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0cc926decb28603ad99af3306016f5eed97c7890
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/21/2019
ms.locfileid: "34311008"
---
# <a name="create-calendar"></a><span data-ttu-id="57fab-103">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="57fab-103">Create Calendar</span></span>

<span data-ttu-id="57fab-104">この API を使って、[ユーザー](../resources/user.md)用の予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="57fab-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57fab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57fab-105">Permissions</span></span>

<span data-ttu-id="57fab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57fab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57fab-108">Permission type</span></span>                        | <span data-ttu-id="57fab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="57fab-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="57fab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57fab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="57fab-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fab-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="57fab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57fab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57fab-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fab-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="57fab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57fab-114">Application</span></span>                            | <span data-ttu-id="57fab-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fab-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="57fab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57fab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="57fab-117">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="57fab-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="57fab-118">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="57fab-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="57fab-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57fab-119">Request headers</span></span>

| <span data-ttu-id="57fab-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57fab-120">Header</span></span>        | <span data-ttu-id="57fab-121">値</span><span class="sxs-lookup"><span data-stu-id="57fab-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="57fab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57fab-122">Authorization</span></span> | <span data-ttu-id="57fab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="57fab-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="57fab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57fab-125">Content-Type</span></span>  | <span data-ttu-id="57fab-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="57fab-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57fab-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="57fab-128">Request body</span></span>

<span data-ttu-id="57fab-129">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57fab-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57fab-130">応答</span><span class="sxs-lookup"><span data-stu-id="57fab-130">Response</span></span>

<span data-ttu-id="57fab-131">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="57fab-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fab-132">例</span><span class="sxs-lookup"><span data-stu-id="57fab-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57fab-133">要求</span><span class="sxs-lookup"><span data-stu-id="57fab-133">Request</span></span>

<span data-ttu-id="57fab-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57fab-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars

Content-type: application/json

{
  "name": "Marketing calendar"
}
```

<span data-ttu-id="57fab-135">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57fab-135">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="57fab-136">応答</span><span class="sxs-lookup"><span data-stu-id="57fab-136">Response</span></span>

<span data-ttu-id="57fab-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57fab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="57fab-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="57fab-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="57fab-141">C#</span><span class="sxs-lookup"><span data-stu-id="57fab-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_calendar_from_calendargroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57fab-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="57fab-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_calendar_from_calendargroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-post-calendars.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-post-calendars.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
