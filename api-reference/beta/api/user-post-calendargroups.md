---
title: CalendarGroup を作成する　
description: この API を使用して、新しい CalendarGroup を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 477576ab5c944b35ec9e554f8d1bd0da850d380d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867017"
---
# <a name="create-calendargroup"></a><span data-ttu-id="79e3b-103">CalendarGroup を作成する　</span><span class="sxs-lookup"><span data-stu-id="79e3b-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79e3b-104">この API を使用して、新しい CalendarGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="79e3b-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="79e3b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79e3b-105">Permissions</span></span>
<span data-ttu-id="79e3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79e3b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79e3b-108">Permission type</span></span>      | <span data-ttu-id="79e3b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79e3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79e3b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79e3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79e3b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79e3b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="79e3b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79e3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79e3b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79e3b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="79e3b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79e3b-114">Application</span></span> | <span data-ttu-id="79e3b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79e3b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79e3b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79e3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="79e3b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79e3b-117">Request headers</span></span>
| <span data-ttu-id="79e3b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79e3b-118">Header</span></span>       | <span data-ttu-id="79e3b-119">値</span><span class="sxs-lookup"><span data-stu-id="79e3b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79e3b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="79e3b-120">Authorization</span></span>  | <span data-ttu-id="79e3b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79e3b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79e3b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79e3b-123">Content-Type</span></span>  | <span data-ttu-id="79e3b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79e3b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79e3b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="79e3b-125">Request body</span></span>
<span data-ttu-id="79e3b-126">要求本文で、[CalendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79e3b-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79e3b-127">応答</span><span class="sxs-lookup"><span data-stu-id="79e3b-127">Response</span></span>

<span data-ttu-id="79e3b-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79e3b-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79e3b-129">例</span><span class="sxs-lookup"><span data-stu-id="79e3b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79e3b-130">要求</span><span class="sxs-lookup"><span data-stu-id="79e3b-130">Request</span></span>
<span data-ttu-id="79e3b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79e3b-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79e3b-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="79e3b-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79e3b-133">C#</span><span class="sxs-lookup"><span data-stu-id="79e3b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79e3b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="79e3b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79e3b-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="79e3b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79e3b-136">Java</span><span class="sxs-lookup"><span data-stu-id="79e3b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="79e3b-137">要求本文で、[calendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79e3b-137">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="79e3b-138">応答</span><span class="sxs-lookup"><span data-stu-id="79e3b-138">Response</span></span>
<span data-ttu-id="79e3b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79e3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
