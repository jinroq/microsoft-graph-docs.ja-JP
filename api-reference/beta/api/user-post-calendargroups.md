---
title: CalendarGroup を作成する　
description: この API を使用して、新しい CalendarGroup を作成します。
author: dkershaw10
ms.openlocfilehash: a68be3470489b20667112b67d15f4472a3817d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319049"
---
# <a name="create-calendargroup"></a><span data-ttu-id="374ae-103">CalendarGroup を作成する　</span><span class="sxs-lookup"><span data-stu-id="374ae-103">Create CalendarGroup</span></span>

> <span data-ttu-id="374ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="374ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="374ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="374ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="374ae-106">この API を使用して、新しい CalendarGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="374ae-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="374ae-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="374ae-107">Permissions</span></span>
<span data-ttu-id="374ae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="374ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="374ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="374ae-110">Permission type</span></span>      | <span data-ttu-id="374ae-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="374ae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="374ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="374ae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="374ae-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="374ae-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="374ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="374ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="374ae-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="374ae-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="374ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="374ae-116">Application</span></span> | <span data-ttu-id="374ae-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="374ae-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="374ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="374ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="374ae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="374ae-119">Request headers</span></span>
| <span data-ttu-id="374ae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="374ae-120">Header</span></span>       | <span data-ttu-id="374ae-121">値</span><span class="sxs-lookup"><span data-stu-id="374ae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="374ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="374ae-122">Authorization</span></span>  | <span data-ttu-id="374ae-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="374ae-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="374ae-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="374ae-125">Content-Type</span></span>  | <span data-ttu-id="374ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="374ae-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="374ae-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="374ae-127">Request body</span></span>
<span data-ttu-id="374ae-128">要求本文で、[CalendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="374ae-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="374ae-129">応答</span><span class="sxs-lookup"><span data-stu-id="374ae-129">Response</span></span>

<span data-ttu-id="374ae-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="374ae-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="374ae-131">例</span><span class="sxs-lookup"><span data-stu-id="374ae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="374ae-132">要求</span><span class="sxs-lookup"><span data-stu-id="374ae-132">Request</span></span>
<span data-ttu-id="374ae-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="374ae-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="374ae-134">要求本文で、[calendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="374ae-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="374ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="374ae-135">Response</span></span>
<span data-ttu-id="374ae-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="374ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->