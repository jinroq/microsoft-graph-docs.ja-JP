---
title: CalendarGroup を更新する
description: calendargroup オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4f6e99f7217e3eb702886cba05053f8c9a12e5f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419035"
---
# <a name="update-calendargroup"></a><span data-ttu-id="35fbc-103">CalendarGroup を更新する</span><span class="sxs-lookup"><span data-stu-id="35fbc-103">Update calendargroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35fbc-104">calendargroup オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35fbc-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35fbc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35fbc-105">Permissions</span></span>

<span data-ttu-id="35fbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35fbc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35fbc-108">Permission type</span></span>                        | <span data-ttu-id="35fbc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35fbc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="35fbc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35fbc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="35fbc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35fbc-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="35fbc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35fbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35fbc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35fbc-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="35fbc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35fbc-114">Application</span></span>                            | <span data-ttu-id="35fbc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35fbc-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="35fbc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35fbc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="35fbc-117">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="35fbc-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35fbc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35fbc-118">Request headers</span></span>

| <span data-ttu-id="35fbc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35fbc-119">Header</span></span>        | <span data-ttu-id="35fbc-120">値</span><span class="sxs-lookup"><span data-stu-id="35fbc-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="35fbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35fbc-121">Authorization</span></span> | <span data-ttu-id="35fbc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="35fbc-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="35fbc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35fbc-124">Content-Type</span></span>  | <span data-ttu-id="35fbc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="35fbc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35fbc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="35fbc-127">Request body</span></span>

<span data-ttu-id="35fbc-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="35fbc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="35fbc-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35fbc-131">Property</span></span> | <span data-ttu-id="35fbc-132">型</span><span class="sxs-lookup"><span data-stu-id="35fbc-132">Type</span></span>   | <span data-ttu-id="35fbc-133">説明</span><span class="sxs-lookup"><span data-stu-id="35fbc-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="35fbc-134">name</span><span class="sxs-lookup"><span data-stu-id="35fbc-134">name</span></span>     | <span data-ttu-id="35fbc-135">String</span><span class="sxs-lookup"><span data-stu-id="35fbc-135">String</span></span> | <span data-ttu-id="35fbc-136">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="35fbc-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="35fbc-137">応答</span><span class="sxs-lookup"><span data-stu-id="35fbc-137">Response</span></span>

<span data-ttu-id="35fbc-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表グループ](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35fbc-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35fbc-139">例</span><span class="sxs-lookup"><span data-stu-id="35fbc-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35fbc-140">要求</span><span class="sxs-lookup"><span data-stu-id="35fbc-140">Request</span></span>

<span data-ttu-id="35fbc-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35fbc-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35fbc-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="35fbc-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35fbc-143">C#</span><span class="sxs-lookup"><span data-stu-id="35fbc-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35fbc-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35fbc-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35fbc-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="35fbc-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35fbc-146">応答</span><span class="sxs-lookup"><span data-stu-id="35fbc-146">Response</span></span>

<span data-ttu-id="35fbc-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="35fbc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
