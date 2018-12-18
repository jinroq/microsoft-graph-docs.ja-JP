---
title: 予定表を作成する
description: この API を使って、ユーザー用の予定表グループに新しい予定表を作成します。
author: angelgolfer-ms
ms.openlocfilehash: 09b98abeaae5e908046aeac370c791e45a1e894d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306966"
---
# <a name="create-calendar"></a><span data-ttu-id="a86f3-103">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="a86f3-103">Create Calendar</span></span>

<span data-ttu-id="a86f3-104">この API を使って、[ユーザー](../resources/user.md)用の予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="a86f3-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a86f3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a86f3-105">Permissions</span></span>

<span data-ttu-id="a86f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a86f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a86f3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a86f3-108">Permission type</span></span>                        | <span data-ttu-id="a86f3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a86f3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a86f3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a86f3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a86f3-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a86f3-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a86f3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a86f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a86f3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a86f3-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a86f3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a86f3-114">Application</span></span>                            | <span data-ttu-id="a86f3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a86f3-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a86f3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a86f3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a86f3-117">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="a86f3-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="a86f3-118">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="a86f3-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="a86f3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a86f3-119">Request headers</span></span>

| <span data-ttu-id="a86f3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a86f3-120">Header</span></span>        | <span data-ttu-id="a86f3-121">値</span><span class="sxs-lookup"><span data-stu-id="a86f3-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="a86f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a86f3-122">Authorization</span></span> | <span data-ttu-id="a86f3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a86f3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a86f3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a86f3-125">Content-Type</span></span>  | <span data-ttu-id="a86f3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a86f3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a86f3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a86f3-128">Request body</span></span>

<span data-ttu-id="a86f3-129">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a86f3-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a86f3-130">応答</span><span class="sxs-lookup"><span data-stu-id="a86f3-130">Response</span></span>

<span data-ttu-id="a86f3-131">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a86f3-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a86f3-132">例</span><span class="sxs-lookup"><span data-stu-id="a86f3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a86f3-133">要求</span><span class="sxs-lookup"><span data-stu-id="a86f3-133">Request</span></span>

<span data-ttu-id="a86f3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a86f3-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="a86f3-135">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a86f3-135">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a86f3-136">応答</span><span class="sxs-lookup"><span data-stu-id="a86f3-136">Response</span></span>

<span data-ttu-id="a86f3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a86f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
