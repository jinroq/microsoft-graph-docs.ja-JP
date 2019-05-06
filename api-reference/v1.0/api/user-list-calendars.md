---
title: 予定表を一覧表示する
description: 'すべてのユーザーの予定表を取得します (`/calendars` ナビゲーション プロパティ)。また既定の予定表グループまたは特定の予定表グループから予定表を取得します。 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 762a8ffeaacbc294587e88bf14290cc985c8b2d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567852"
---
# <a name="list-calendars"></a><span data-ttu-id="72e62-103">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="72e62-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e62-104">すべてのユーザーの予定表を取得します (`/calendars` ナビゲーション プロパティ)。また既定の予定表グループまたは特定の予定表グループから予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="72e62-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="72e62-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72e62-105">Permissions</span></span>
<span data-ttu-id="72e62-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e62-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72e62-108">Permission type</span></span>      | <span data-ttu-id="72e62-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72e62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72e62-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72e62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72e62-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72e62-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="72e62-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72e62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72e62-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72e62-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="72e62-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72e62-114">Application</span></span> | <span data-ttu-id="72e62-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72e62-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="72e62-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72e62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="72e62-117">すべてのユーザーの予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="72e62-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="72e62-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="72e62-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="72e62-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="72e62-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72e62-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="72e62-120">Optional query parameters</span></span>
<span data-ttu-id="72e62-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="72e62-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="72e62-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72e62-122">Request headers</span></span>
| <span data-ttu-id="72e62-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72e62-123">Header</span></span>       | <span data-ttu-id="72e62-124">値</span><span class="sxs-lookup"><span data-stu-id="72e62-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72e62-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e62-125">Authorization</span></span>  | <span data-ttu-id="72e62-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72e62-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72e62-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72e62-128">Content-Type</span></span>   | <span data-ttu-id="72e62-129">application/json</span><span class="sxs-lookup"><span data-stu-id="72e62-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="72e62-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="72e62-130">Request body</span></span>
<span data-ttu-id="72e62-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="72e62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72e62-132">応答</span><span class="sxs-lookup"><span data-stu-id="72e62-132">Response</span></span>

<span data-ttu-id="72e62-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="72e62-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72e62-134">例</span><span class="sxs-lookup"><span data-stu-id="72e62-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72e62-135">要求</span><span class="sxs-lookup"><span data-stu-id="72e62-135">Request</span></span>
<span data-ttu-id="72e62-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72e62-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="72e62-137">応答</span><span class="sxs-lookup"><span data-stu-id="72e62-137">Response</span></span>
<span data-ttu-id="72e62-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72e62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
