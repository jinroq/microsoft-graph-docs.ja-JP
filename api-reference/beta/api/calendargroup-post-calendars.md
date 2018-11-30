---
title: 予定表を作成する
description: この API を使って、ユーザー用の予定表グループに新しい予定表を作成します。
ms.openlocfilehash: 220922567eac421479803ad6dd0252a114701c9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068673"
---
# <a name="create-calendar"></a><span data-ttu-id="e5701-103">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="e5701-103">Create Calendar</span></span>

> <span data-ttu-id="e5701-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5701-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5701-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5701-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5701-106">この API を使って、[ユーザー](../resources/user.md)用の予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="e5701-106">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5701-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5701-107">Permissions</span></span>

<span data-ttu-id="e5701-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5701-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5701-110">Permission type</span></span>                        | <span data-ttu-id="e5701-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5701-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e5701-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5701-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5701-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5701-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e5701-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5701-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5701-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5701-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e5701-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5701-116">Application</span></span>                            | <span data-ttu-id="e5701-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5701-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e5701-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5701-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e5701-119">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="e5701-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="e5701-120">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="e5701-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="e5701-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5701-121">Request headers</span></span>

| <span data-ttu-id="e5701-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5701-122">Header</span></span>        | <span data-ttu-id="e5701-123">値</span><span class="sxs-lookup"><span data-stu-id="e5701-123">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="e5701-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5701-124">Authorization</span></span> | <span data-ttu-id="e5701-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5701-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e5701-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5701-127">Content-Type</span></span>  | <span data-ttu-id="e5701-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5701-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5701-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5701-130">Request body</span></span>

<span data-ttu-id="e5701-131">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5701-131">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5701-132">応答</span><span class="sxs-lookup"><span data-stu-id="e5701-132">Response</span></span>

<span data-ttu-id="e5701-133">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5701-133">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5701-134">例</span><span class="sxs-lookup"><span data-stu-id="e5701-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e5701-135">要求</span><span class="sxs-lookup"><span data-stu-id="e5701-135">Request</span></span>

<span data-ttu-id="e5701-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5701-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="e5701-137">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5701-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e5701-138">応答</span><span class="sxs-lookup"><span data-stu-id="e5701-138">Response</span></span>

<span data-ttu-id="e5701-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5701-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
