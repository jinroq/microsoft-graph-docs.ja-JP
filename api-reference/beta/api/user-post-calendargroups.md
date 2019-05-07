---
title: CalendarGroup を作成する　
description: この API を使用して、新しい CalendarGroup を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c8c1fd8b9224dfa789436be80713444bf84c99e6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637144"
---
# <a name="create-calendargroup"></a><span data-ttu-id="32a40-103">CalendarGroup を作成する　</span><span class="sxs-lookup"><span data-stu-id="32a40-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32a40-104">この API を使用して、新しい CalendarGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="32a40-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="32a40-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32a40-105">Permissions</span></span>
<span data-ttu-id="32a40-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a40-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32a40-108">Permission type</span></span>      | <span data-ttu-id="32a40-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32a40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32a40-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32a40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32a40-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32a40-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="32a40-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32a40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32a40-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32a40-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="32a40-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32a40-114">Application</span></span> | <span data-ttu-id="32a40-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32a40-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32a40-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32a40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="32a40-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32a40-117">Request headers</span></span>
| <span data-ttu-id="32a40-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32a40-118">Header</span></span>       | <span data-ttu-id="32a40-119">値</span><span class="sxs-lookup"><span data-stu-id="32a40-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32a40-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32a40-120">Authorization</span></span>  | <span data-ttu-id="32a40-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32a40-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32a40-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32a40-123">Content-Type</span></span>  | <span data-ttu-id="32a40-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32a40-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32a40-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="32a40-125">Request body</span></span>
<span data-ttu-id="32a40-126">要求本文で、[CalendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="32a40-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="32a40-127">応答</span><span class="sxs-lookup"><span data-stu-id="32a40-127">Response</span></span>

<span data-ttu-id="32a40-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32a40-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a40-129">例</span><span class="sxs-lookup"><span data-stu-id="32a40-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32a40-130">要求</span><span class="sxs-lookup"><span data-stu-id="32a40-130">Request</span></span>
<span data-ttu-id="32a40-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32a40-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="32a40-132">要求本文で、[calendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="32a40-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="32a40-133">応答</span><span class="sxs-lookup"><span data-stu-id="32a40-133">Response</span></span>
<span data-ttu-id="32a40-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32a40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="32a40-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="32a40-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="32a40-138">Visual</span><span class="sxs-lookup"><span data-stu-id="32a40-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32a40-139">Java</span><span class="sxs-lookup"><span data-stu-id="32a40-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
