---
title: 予定表を作成する
description: この API を使用して、ユーザー用の新しい予定表を作成します。
author: dkershaw10
ms.openlocfilehash: ecc86df41dd5d54f07545170ce33f42f782c5dc3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27300869"
---
# <a name="create-calendar"></a><span data-ttu-id="8c48c-103">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="8c48c-103">Create Calendar</span></span>

<span data-ttu-id="8c48c-104">この API を使用して、[ユーザー](../resources/user.md)用の新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="8c48c-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8c48c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c48c-105">Permissions</span></span>
<span data-ttu-id="8c48c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c48c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c48c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c48c-108">Permission type</span></span>      | <span data-ttu-id="8c48c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c48c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c48c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c48c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c48c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c48c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c48c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c48c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c48c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c48c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c48c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c48c-114">Application</span></span> | <span data-ttu-id="8c48c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c48c-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c48c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c48c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="8c48c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c48c-117">Request headers</span></span>
| <span data-ttu-id="8c48c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c48c-118">Header</span></span>       | <span data-ttu-id="8c48c-119">値</span><span class="sxs-lookup"><span data-stu-id="8c48c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c48c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c48c-120">Authorization</span></span>  | <span data-ttu-id="8c48c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c48c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c48c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c48c-123">Content-Type</span></span>  | <span data-ttu-id="8c48c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c48c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c48c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c48c-125">Request body</span></span>
<span data-ttu-id="8c48c-126">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c48c-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8c48c-127">応答</span><span class="sxs-lookup"><span data-stu-id="8c48c-127">Response</span></span>

<span data-ttu-id="8c48c-128">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c48c-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c48c-129">例</span><span class="sxs-lookup"><span data-stu-id="8c48c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c48c-130">要求</span><span class="sxs-lookup"><span data-stu-id="8c48c-130">Request</span></span>
<span data-ttu-id="8c48c-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c48c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="8c48c-132">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c48c-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8c48c-133">応答</span><span class="sxs-lookup"><span data-stu-id="8c48c-133">Response</span></span>
<span data-ttu-id="8c48c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c48c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->