---
title: 予定表を作成する
description: この API を使用して、ユーザー用の新しい予定表を作成します。
author: dkershaw10
ms.openlocfilehash: 320a34a22db3e8467af5c30c79ce41c6d18fc05b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339929"
---
# <a name="create-calendar"></a><span data-ttu-id="22173-103">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="22173-103">Create Calendar</span></span>

> <span data-ttu-id="22173-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22173-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22173-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22173-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22173-106">この API を使用して、[ユーザー](../resources/user.md)用の新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="22173-106">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="22173-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22173-107">Permissions</span></span>
<span data-ttu-id="22173-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22173-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22173-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22173-110">Permission type</span></span>      | <span data-ttu-id="22173-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22173-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22173-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22173-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22173-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22173-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="22173-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22173-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22173-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22173-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="22173-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22173-116">Application</span></span> | <span data-ttu-id="22173-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22173-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="22173-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22173-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="22173-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22173-119">Request headers</span></span>
| <span data-ttu-id="22173-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22173-120">Header</span></span>       | <span data-ttu-id="22173-121">値</span><span class="sxs-lookup"><span data-stu-id="22173-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22173-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22173-122">Authorization</span></span>  | <span data-ttu-id="22173-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22173-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22173-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22173-125">Content-Type</span></span>  | <span data-ttu-id="22173-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22173-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22173-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="22173-127">Request body</span></span>
<span data-ttu-id="22173-128">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22173-128">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22173-129">応答</span><span class="sxs-lookup"><span data-stu-id="22173-129">Response</span></span>

<span data-ttu-id="22173-130">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22173-130">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22173-131">例</span><span class="sxs-lookup"><span data-stu-id="22173-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22173-132">要求</span><span class="sxs-lookup"><span data-stu-id="22173-132">Request</span></span>
<span data-ttu-id="22173-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22173-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
<span data-ttu-id="22173-134">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22173-134">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="22173-135">応答</span><span class="sxs-lookup"><span data-stu-id="22173-135">Response</span></span>
<span data-ttu-id="22173-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22173-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->