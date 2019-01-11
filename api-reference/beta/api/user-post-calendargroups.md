---
title: CalendarGroup を作成する　
description: この API を使用して、新しい CalendarGroup を作成します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e2d8d4a00a629fb2dfb7ca811a319a1859758fb1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839432"
---
# <a name="create-calendargroup"></a><span data-ttu-id="2040d-103">CalendarGroup を作成する　</span><span class="sxs-lookup"><span data-stu-id="2040d-103">Create CalendarGroup</span></span>

> <span data-ttu-id="2040d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2040d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2040d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2040d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2040d-106">この API を使用して、新しい CalendarGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="2040d-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="2040d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2040d-107">Permissions</span></span>
<span data-ttu-id="2040d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2040d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2040d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2040d-110">Permission type</span></span>      | <span data-ttu-id="2040d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2040d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2040d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2040d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2040d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2040d-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2040d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2040d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2040d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2040d-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2040d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2040d-116">Application</span></span> | <span data-ttu-id="2040d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2040d-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2040d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2040d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="2040d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2040d-119">Request headers</span></span>
| <span data-ttu-id="2040d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2040d-120">Header</span></span>       | <span data-ttu-id="2040d-121">値</span><span class="sxs-lookup"><span data-stu-id="2040d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2040d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2040d-122">Authorization</span></span>  | <span data-ttu-id="2040d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2040d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2040d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2040d-125">Content-Type</span></span>  | <span data-ttu-id="2040d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2040d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2040d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2040d-127">Request body</span></span>
<span data-ttu-id="2040d-128">要求本文で、[CalendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2040d-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2040d-129">応答</span><span class="sxs-lookup"><span data-stu-id="2040d-129">Response</span></span>

<span data-ttu-id="2040d-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2040d-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2040d-131">例</span><span class="sxs-lookup"><span data-stu-id="2040d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2040d-132">要求</span><span class="sxs-lookup"><span data-stu-id="2040d-132">Request</span></span>
<span data-ttu-id="2040d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2040d-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="2040d-134">要求本文で、[calendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2040d-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2040d-135">応答</span><span class="sxs-lookup"><span data-stu-id="2040d-135">Response</span></span>
<span data-ttu-id="2040d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2040d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
