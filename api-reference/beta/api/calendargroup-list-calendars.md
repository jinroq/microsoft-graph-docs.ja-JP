---
title: 予定表を一覧表示する
description: 予定表グループに属している予定表のリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fcb30ab9c563197635be04995b92f540d0f8a514
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317831"
---
# <a name="list-calendars"></a><span data-ttu-id="befa1-103">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="befa1-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="befa1-104">予定表グループに属している予定表のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="befa1-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="befa1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="befa1-105">Permissions</span></span>

<span data-ttu-id="befa1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="befa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="befa1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="befa1-108">Permission type</span></span>                        | <span data-ttu-id="befa1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="befa1-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="befa1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="befa1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="befa1-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="befa1-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="befa1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="befa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="befa1-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="befa1-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="befa1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="befa1-114">Application</span></span>                            | <span data-ttu-id="befa1-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="befa1-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="befa1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="befa1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="befa1-117">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="befa1-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="befa1-118">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="befa1-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="befa1-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="befa1-119">Optional query parameters</span></span>

<span data-ttu-id="befa1-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="befa1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="befa1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="befa1-121">Request headers</span></span>

| <span data-ttu-id="befa1-122">名前</span><span class="sxs-lookup"><span data-stu-id="befa1-122">Name</span></span>          | <span data-ttu-id="befa1-123">型</span><span class="sxs-lookup"><span data-stu-id="befa1-123">Type</span></span>   | <span data-ttu-id="befa1-124">説明</span><span class="sxs-lookup"><span data-stu-id="befa1-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="befa1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="befa1-125">Authorization</span></span> | <span data-ttu-id="befa1-126">string</span><span class="sxs-lookup"><span data-stu-id="befa1-126">string</span></span> | <span data-ttu-id="befa1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="befa1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="befa1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="befa1-129">Request body</span></span>

<span data-ttu-id="befa1-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="befa1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="befa1-131">応答</span><span class="sxs-lookup"><span data-stu-id="befa1-131">Response</span></span>

<span data-ttu-id="befa1-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="befa1-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="befa1-133">例</span><span class="sxs-lookup"><span data-stu-id="befa1-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="befa1-134">要求</span><span class="sxs-lookup"><span data-stu-id="befa1-134">Request</span></span>

<span data-ttu-id="befa1-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="befa1-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="befa1-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="befa1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="befa1-137">C#</span><span class="sxs-lookup"><span data-stu-id="befa1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="befa1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="befa1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="befa1-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="befa1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="befa1-140">Java</span><span class="sxs-lookup"><span data-stu-id="befa1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="befa1-141">応答</span><span class="sxs-lookup"><span data-stu-id="befa1-141">Response</span></span>

<span data-ttu-id="befa1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="befa1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
