---
title: 予定表を一覧表示する
description: 予定表グループに属している予定表のリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 55af5ab454b6afe534a1a8d2efa76de7a0e7f9d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862987"
---
# <a name="list-calendars"></a><span data-ttu-id="d1771-103">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1771-103">List calendars</span></span>

<span data-ttu-id="d1771-104">予定表グループに属している予定表のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1771-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1771-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1771-105">Permissions</span></span>

<span data-ttu-id="d1771-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1771-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1771-108">Permission type</span></span>                        | <span data-ttu-id="d1771-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1771-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d1771-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1771-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1771-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1771-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="d1771-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1771-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1771-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1771-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="d1771-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1771-114">Application</span></span>                            | <span data-ttu-id="d1771-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1771-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="d1771-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1771-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d1771-117">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="d1771-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="d1771-118">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="d1771-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1771-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d1771-119">Optional query parameters</span></span>

<span data-ttu-id="d1771-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d1771-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1771-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1771-121">Request headers</span></span>

| <span data-ttu-id="d1771-122">名前</span><span class="sxs-lookup"><span data-stu-id="d1771-122">Name</span></span>          | <span data-ttu-id="d1771-123">種類</span><span class="sxs-lookup"><span data-stu-id="d1771-123">Type</span></span>   | <span data-ttu-id="d1771-124">説明</span><span class="sxs-lookup"><span data-stu-id="d1771-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d1771-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1771-125">Authorization</span></span> | <span data-ttu-id="d1771-126">string</span><span class="sxs-lookup"><span data-stu-id="d1771-126">string</span></span> | <span data-ttu-id="d1771-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1771-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1771-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1771-129">Request body</span></span>

<span data-ttu-id="d1771-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1771-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1771-131">応答</span><span class="sxs-lookup"><span data-stu-id="d1771-131">Response</span></span>

<span data-ttu-id="d1771-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d1771-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1771-133">例</span><span class="sxs-lookup"><span data-stu-id="d1771-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d1771-134">要求</span><span class="sxs-lookup"><span data-stu-id="d1771-134">Request</span></span>

<span data-ttu-id="d1771-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1771-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="d1771-136">応答</span><span class="sxs-lookup"><span data-stu-id="d1771-136">Response</span></span>

<span data-ttu-id="d1771-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1771-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
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
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
