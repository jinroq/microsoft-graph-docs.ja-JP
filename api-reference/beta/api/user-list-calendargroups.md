---
title: List calendarGroups
description: ユーザーの予定表グループを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 706bb810b0dcd9615443c477437350a020166be5
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869345"
---
# <a name="list-calendargroups"></a><span data-ttu-id="8c398-103">List calendarGroups</span><span class="sxs-lookup"><span data-stu-id="8c398-103">List calendarGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c398-104">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c398-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c398-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c398-105">Permissions</span></span>
<span data-ttu-id="8c398-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c398-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c398-108">Permission type</span></span>      | <span data-ttu-id="8c398-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c398-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c398-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c398-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c398-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c398-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c398-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c398-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c398-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c398-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c398-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c398-114">Application</span></span> | <span data-ttu-id="8c398-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c398-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c398-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c398-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c398-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c398-117">Optional query parameters</span></span>
<span data-ttu-id="8c398-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c398-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c398-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c398-119">Request headers</span></span>
| <span data-ttu-id="8c398-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c398-120">Header</span></span>       | <span data-ttu-id="8c398-121">値</span><span class="sxs-lookup"><span data-stu-id="8c398-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c398-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c398-122">Authorization</span></span>  | <span data-ttu-id="8c398-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c398-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c398-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c398-125">Content-Type</span></span>  | <span data-ttu-id="8c398-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c398-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c398-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c398-127">Request body</span></span>
<span data-ttu-id="8c398-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c398-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c398-129">応答</span><span class="sxs-lookup"><span data-stu-id="8c398-129">Response</span></span>

<span data-ttu-id="8c398-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8c398-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c398-131">例</span><span class="sxs-lookup"><span data-stu-id="8c398-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c398-132">要求</span><span class="sxs-lookup"><span data-stu-id="8c398-132">Request</span></span>
<span data-ttu-id="8c398-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c398-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="8c398-134">応答</span><span class="sxs-lookup"><span data-stu-id="8c398-134">Response</span></span>
<span data-ttu-id="8c398-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c398-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-calendargroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
