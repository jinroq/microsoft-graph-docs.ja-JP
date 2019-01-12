---
title: CalendarGroup を更新する　
description: calendargroup オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f488594778c1e80e725cb2587bf5d0c41cb570e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961303"
---
# <a name="update-calendargroup"></a><span data-ttu-id="5cc37-103">CalendarGroup を更新する　</span><span class="sxs-lookup"><span data-stu-id="5cc37-103">Update calendargroup</span></span>

> <span data-ttu-id="5cc37-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5cc37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cc37-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cc37-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cc37-106">calendargroup オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5cc37-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cc37-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5cc37-107">Permissions</span></span>

<span data-ttu-id="5cc37-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cc37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cc37-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5cc37-110">Permission type</span></span>                        | <span data-ttu-id="5cc37-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5cc37-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5cc37-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5cc37-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cc37-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cc37-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5cc37-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cc37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cc37-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cc37-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5cc37-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5cc37-116">Application</span></span>                            | <span data-ttu-id="5cc37-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cc37-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5cc37-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cc37-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5cc37-119">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="5cc37-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5cc37-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cc37-120">Request headers</span></span>

| <span data-ttu-id="5cc37-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cc37-121">Header</span></span>        | <span data-ttu-id="5cc37-122">値</span><span class="sxs-lookup"><span data-stu-id="5cc37-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="5cc37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc37-123">Authorization</span></span> | <span data-ttu-id="5cc37-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5cc37-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5cc37-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cc37-126">Content-Type</span></span>  | <span data-ttu-id="5cc37-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5cc37-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cc37-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5cc37-129">Request body</span></span>

<span data-ttu-id="5cc37-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5cc37-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5cc37-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cc37-133">Property</span></span> | <span data-ttu-id="5cc37-134">種類</span><span class="sxs-lookup"><span data-stu-id="5cc37-134">Type</span></span>   | <span data-ttu-id="5cc37-135">説明</span><span class="sxs-lookup"><span data-stu-id="5cc37-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="5cc37-136">名前</span><span class="sxs-lookup"><span data-stu-id="5cc37-136">name</span></span>     | <span data-ttu-id="5cc37-137">String</span><span class="sxs-lookup"><span data-stu-id="5cc37-137">String</span></span> | <span data-ttu-id="5cc37-138">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="5cc37-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="5cc37-139">応答</span><span class="sxs-lookup"><span data-stu-id="5cc37-139">Response</span></span>

<span data-ttu-id="5cc37-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表グループ](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5cc37-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc37-141">例</span><span class="sxs-lookup"><span data-stu-id="5cc37-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5cc37-142">要求</span><span class="sxs-lookup"><span data-stu-id="5cc37-142">Request</span></span>

<span data-ttu-id="5cc37-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5cc37-143">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5cc37-144">応答</span><span class="sxs-lookup"><span data-stu-id="5cc37-144">Response</span></span>

<span data-ttu-id="5cc37-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5cc37-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
