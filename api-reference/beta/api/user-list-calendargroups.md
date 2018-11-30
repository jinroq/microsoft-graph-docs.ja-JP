---
title: calendarGroups を一覧表示する　
description: ユーザーの予定表グループを取得します。
ms.openlocfilehash: 560dd09d42b59e68b6282d7dec4305f7b10ea9f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074377"
---
# <a name="list-calendargroups"></a><span data-ttu-id="766ee-103">calendarGroups を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="766ee-103">List calendarGroups</span></span>

> <span data-ttu-id="766ee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="766ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="766ee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="766ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="766ee-106">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="766ee-106">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="766ee-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="766ee-107">Permissions</span></span>
<span data-ttu-id="766ee-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="766ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="766ee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="766ee-110">Permission type</span></span>      | <span data-ttu-id="766ee-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="766ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="766ee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="766ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="766ee-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="766ee-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="766ee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="766ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766ee-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="766ee-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="766ee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="766ee-116">Application</span></span> | <span data-ttu-id="766ee-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="766ee-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="766ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="766ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="766ee-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="766ee-119">Optional query parameters</span></span>
<span data-ttu-id="766ee-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="766ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="766ee-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="766ee-121">Request headers</span></span>
| <span data-ttu-id="766ee-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="766ee-122">Header</span></span>       | <span data-ttu-id="766ee-123">値</span><span class="sxs-lookup"><span data-stu-id="766ee-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="766ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="766ee-124">Authorization</span></span>  | <span data-ttu-id="766ee-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="766ee-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="766ee-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="766ee-127">Content-Type</span></span>  | <span data-ttu-id="766ee-128">application/json</span><span class="sxs-lookup"><span data-stu-id="766ee-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="766ee-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="766ee-129">Request body</span></span>
<span data-ttu-id="766ee-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="766ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="766ee-131">応答</span><span class="sxs-lookup"><span data-stu-id="766ee-131">Response</span></span>

<span data-ttu-id="766ee-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="766ee-132">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="766ee-133">例</span><span class="sxs-lookup"><span data-stu-id="766ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="766ee-134">要求</span><span class="sxs-lookup"><span data-stu-id="766ee-134">Request</span></span>
<span data-ttu-id="766ee-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="766ee-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="766ee-136">応答</span><span class="sxs-lookup"><span data-stu-id="766ee-136">Response</span></span>
<span data-ttu-id="766ee-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="766ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
