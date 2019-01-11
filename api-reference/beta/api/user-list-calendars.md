---
title: 予定表を一覧表示する
description: 'すべてのユーザーの予定表を取得します (`/calendars` ナビゲーション プロパティ)。また既定の予定表グループまたは特定の予定表グループから予定表を取得します。 '
localization_priority: Normal
ms.openlocfilehash: c59ee99c900aa39221530473c9323dfcaab721b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886515"
---
# <a name="list-calendars"></a><span data-ttu-id="14e60-103">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14e60-103">List calendars</span></span>

> <span data-ttu-id="14e60-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14e60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14e60-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14e60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14e60-106">すべてのユーザーの予定表を取得します (`/calendars` ナビゲーション プロパティ)。また既定の予定表グループまたは特定の予定表グループから予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="14e60-106">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="14e60-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14e60-107">Permissions</span></span>
<span data-ttu-id="14e60-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14e60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e60-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14e60-110">Permission type</span></span>      | <span data-ttu-id="14e60-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14e60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14e60-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14e60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14e60-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14e60-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="14e60-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14e60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14e60-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14e60-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="14e60-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14e60-116">Application</span></span> | <span data-ttu-id="14e60-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14e60-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="14e60-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14e60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="14e60-119">すべてのユーザーの予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="14e60-119">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="14e60-120">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="14e60-120">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="14e60-121">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="14e60-121">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14e60-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14e60-122">Optional query parameters</span></span>
<span data-ttu-id="14e60-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="14e60-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14e60-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14e60-124">Request headers</span></span>
| <span data-ttu-id="14e60-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14e60-125">Header</span></span>       | <span data-ttu-id="14e60-126">値</span><span class="sxs-lookup"><span data-stu-id="14e60-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14e60-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="14e60-127">Authorization</span></span>  | <span data-ttu-id="14e60-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="14e60-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14e60-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14e60-130">Content-Type</span></span>   | <span data-ttu-id="14e60-131">application/json</span><span class="sxs-lookup"><span data-stu-id="14e60-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="14e60-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="14e60-132">Request body</span></span>
<span data-ttu-id="14e60-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14e60-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e60-134">応答</span><span class="sxs-lookup"><span data-stu-id="14e60-134">Response</span></span>

<span data-ttu-id="14e60-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="14e60-135">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14e60-136">例</span><span class="sxs-lookup"><span data-stu-id="14e60-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14e60-137">要求</span><span class="sxs-lookup"><span data-stu-id="14e60-137">Request</span></span>
<span data-ttu-id="14e60-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14e60-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="14e60-139">応答</span><span class="sxs-lookup"><span data-stu-id="14e60-139">Response</span></span>
<span data-ttu-id="14e60-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14e60-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "isDefaultCalendar": true,
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
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
