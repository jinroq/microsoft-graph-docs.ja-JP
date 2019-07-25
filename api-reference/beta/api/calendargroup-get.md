---
title: Get calendarGroup
description: 予定表グループ オブジェクトのプロパティと関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ffb416dbced448791e22ed158cb05d63499f8ef7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864995"
---
# <a name="get-calendargroup"></a><span data-ttu-id="09011-103">Get calendarGroup</span><span class="sxs-lookup"><span data-stu-id="09011-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09011-104">予定表グループ オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="09011-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09011-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09011-105">Permissions</span></span>

<span data-ttu-id="09011-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09011-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09011-108">Permission type</span></span>                        | <span data-ttu-id="09011-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09011-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="09011-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09011-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09011-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09011-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="09011-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09011-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09011-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09011-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="09011-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09011-114">Application</span></span>                            | <span data-ttu-id="09011-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09011-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="09011-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09011-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="09011-117">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="09011-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09011-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="09011-118">Optional query parameters</span></span>

<span data-ttu-id="09011-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="09011-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09011-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09011-120">Request headers</span></span>

| <span data-ttu-id="09011-121">名前</span><span class="sxs-lookup"><span data-stu-id="09011-121">Name</span></span>          | <span data-ttu-id="09011-122">型</span><span class="sxs-lookup"><span data-stu-id="09011-122">Type</span></span>   | <span data-ttu-id="09011-123">説明</span><span class="sxs-lookup"><span data-stu-id="09011-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="09011-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09011-124">Authorization</span></span> | <span data-ttu-id="09011-125">string</span><span class="sxs-lookup"><span data-stu-id="09011-125">string</span></span> | <span data-ttu-id="09011-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09011-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09011-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="09011-128">Request body</span></span>

<span data-ttu-id="09011-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09011-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09011-130">応答</span><span class="sxs-lookup"><span data-stu-id="09011-130">Response</span></span>

<span data-ttu-id="09011-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09011-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09011-132">例</span><span class="sxs-lookup"><span data-stu-id="09011-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="09011-133">要求</span><span class="sxs-lookup"><span data-stu-id="09011-133">Request</span></span>

<span data-ttu-id="09011-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09011-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="09011-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="09011-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09011-136">C#</span><span class="sxs-lookup"><span data-stu-id="09011-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09011-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="09011-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09011-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="09011-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="09011-139">Java</span><span class="sxs-lookup"><span data-stu-id="09011-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09011-140">応答</span><span class="sxs-lookup"><span data-stu-id="09011-140">Response</span></span>

<span data-ttu-id="09011-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09011-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
