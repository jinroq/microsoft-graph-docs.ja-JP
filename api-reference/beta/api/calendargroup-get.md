---
title: Get calendarGroup
description: 予定表グループ オブジェクトのプロパティと関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 68f0ffcfa34d0a4a69a7cf49d39594c4da18ce98
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635926"
---
# <a name="get-calendargroup"></a><span data-ttu-id="22a6d-103">Get calendarGroup</span><span class="sxs-lookup"><span data-stu-id="22a6d-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a6d-104">予定表グループ オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="22a6d-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22a6d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22a6d-105">Permissions</span></span>

<span data-ttu-id="22a6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22a6d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22a6d-108">Permission type</span></span>                        | <span data-ttu-id="22a6d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22a6d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="22a6d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22a6d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22a6d-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="22a6d-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="22a6d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22a6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a6d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="22a6d-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="22a6d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22a6d-114">Application</span></span>                            | <span data-ttu-id="22a6d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="22a6d-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="22a6d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22a6d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="22a6d-117">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="22a6d-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22a6d-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="22a6d-118">Optional query parameters</span></span>

<span data-ttu-id="22a6d-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="22a6d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22a6d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22a6d-120">Request headers</span></span>

| <span data-ttu-id="22a6d-121">名前</span><span class="sxs-lookup"><span data-stu-id="22a6d-121">Name</span></span>          | <span data-ttu-id="22a6d-122">型</span><span class="sxs-lookup"><span data-stu-id="22a6d-122">Type</span></span>   | <span data-ttu-id="22a6d-123">説明</span><span class="sxs-lookup"><span data-stu-id="22a6d-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="22a6d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a6d-124">Authorization</span></span> | <span data-ttu-id="22a6d-125">string</span><span class="sxs-lookup"><span data-stu-id="22a6d-125">string</span></span> | <span data-ttu-id="22a6d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22a6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22a6d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="22a6d-128">Request body</span></span>

<span data-ttu-id="22a6d-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22a6d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a6d-130">応答</span><span class="sxs-lookup"><span data-stu-id="22a6d-130">Response</span></span>

<span data-ttu-id="22a6d-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22a6d-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a6d-132">例</span><span class="sxs-lookup"><span data-stu-id="22a6d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22a6d-133">要求</span><span class="sxs-lookup"><span data-stu-id="22a6d-133">Request</span></span>

<span data-ttu-id="22a6d-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22a6d-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="22a6d-135">応答</span><span class="sxs-lookup"><span data-stu-id="22a6d-135">Response</span></span>

<span data-ttu-id="22a6d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22a6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="22a6d-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="22a6d-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="22a6d-140">Visual</span><span class="sxs-lookup"><span data-stu-id="22a6d-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendargroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22a6d-141">Java</span><span class="sxs-lookup"><span data-stu-id="22a6d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendargroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendargroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendargroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
