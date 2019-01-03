---
title: 予定表を一覧表示する
description: 予定表グループに属している予定表のリストを取得します。
author: angelgolfer-ms
ms.openlocfilehash: a6cf89b6c5670659d5864496118d125d3c60a903
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336681"
---
# <a name="list-calendars"></a><span data-ttu-id="bcf94-103">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bcf94-103">List calendars</span></span>

> <span data-ttu-id="bcf94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bcf94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcf94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcf94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcf94-106">予定表グループに属している予定表のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bcf94-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf94-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bcf94-107">Permissions</span></span>

<span data-ttu-id="bcf94-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcf94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcf94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcf94-110">Permission type</span></span>                        | <span data-ttu-id="bcf94-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcf94-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bcf94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcf94-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcf94-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcf94-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="bcf94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcf94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf94-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcf94-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="bcf94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcf94-116">Application</span></span>                            | <span data-ttu-id="bcf94-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcf94-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="bcf94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcf94-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="bcf94-119">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="bcf94-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="bcf94-120">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="bcf94-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcf94-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bcf94-121">Optional query parameters</span></span>

<span data-ttu-id="bcf94-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bcf94-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf94-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcf94-123">Request headers</span></span>

| <span data-ttu-id="bcf94-124">名前</span><span class="sxs-lookup"><span data-stu-id="bcf94-124">Name</span></span>          | <span data-ttu-id="bcf94-125">種類</span><span class="sxs-lookup"><span data-stu-id="bcf94-125">Type</span></span>   | <span data-ttu-id="bcf94-126">説明</span><span class="sxs-lookup"><span data-stu-id="bcf94-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="bcf94-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcf94-127">Authorization</span></span> | <span data-ttu-id="bcf94-128">string</span><span class="sxs-lookup"><span data-stu-id="bcf94-128">string</span></span> | <span data-ttu-id="bcf94-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bcf94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf94-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcf94-131">Request body</span></span>

<span data-ttu-id="bcf94-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bcf94-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcf94-133">応答</span><span class="sxs-lookup"><span data-stu-id="bcf94-133">Response</span></span>

<span data-ttu-id="bcf94-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bcf94-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf94-135">例</span><span class="sxs-lookup"><span data-stu-id="bcf94-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bcf94-136">要求</span><span class="sxs-lookup"><span data-stu-id="bcf94-136">Request</span></span>

<span data-ttu-id="bcf94-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bcf94-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="bcf94-138">応答</span><span class="sxs-lookup"><span data-stu-id="bcf94-138">Response</span></span>

<span data-ttu-id="bcf94-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bcf94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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