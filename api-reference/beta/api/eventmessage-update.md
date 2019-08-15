---
title: eventMessage の更新
description: eventMessage オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 29a3d9e97f08a77f58a7abbd268dc82dcb47bbcc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419791"
---
# <a name="update-eventmessage"></a><span data-ttu-id="b67ef-103">eventMessage の更新</span><span class="sxs-lookup"><span data-stu-id="b67ef-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b67ef-104">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b67ef-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b67ef-105">Permissions</span></span>
<span data-ttu-id="b67ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b67ef-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b67ef-108">Permission type</span></span>      | <span data-ttu-id="b67ef-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b67ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b67ef-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b67ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b67ef-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b67ef-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b67ef-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b67ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b67ef-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b67ef-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b67ef-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b67ef-114">Application</span></span> | <span data-ttu-id="b67ef-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b67ef-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b67ef-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b67ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b67ef-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b67ef-117">Request headers</span></span>
| <span data-ttu-id="b67ef-118">名前</span><span class="sxs-lookup"><span data-stu-id="b67ef-118">Name</span></span>       | <span data-ttu-id="b67ef-119">型</span><span class="sxs-lookup"><span data-stu-id="b67ef-119">Type</span></span> | <span data-ttu-id="b67ef-120">説明</span><span class="sxs-lookup"><span data-stu-id="b67ef-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b67ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b67ef-121">Authorization</span></span>  | <span data-ttu-id="b67ef-122">string</span><span class="sxs-lookup"><span data-stu-id="b67ef-122">string</span></span>  | <span data-ttu-id="b67ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b67ef-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b67ef-125">Content-Type</span></span> | <span data-ttu-id="b67ef-126">string</span><span class="sxs-lookup"><span data-stu-id="b67ef-126">string</span></span>  | <span data-ttu-id="b67ef-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="b67ef-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b67ef-129">Request body</span></span>
<span data-ttu-id="b67ef-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="b67ef-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b67ef-134">Property</span></span>     | <span data-ttu-id="b67ef-135">型</span><span class="sxs-lookup"><span data-stu-id="b67ef-135">Type</span></span>   |<span data-ttu-id="b67ef-136">説明</span><span class="sxs-lookup"><span data-stu-id="b67ef-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b67ef-137">categories</span><span class="sxs-lookup"><span data-stu-id="b67ef-137">categories</span></span>|<span data-ttu-id="b67ef-138">String</span><span class="sxs-lookup"><span data-stu-id="b67ef-138">String</span></span>|<span data-ttu-id="b67ef-139">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="b67ef-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="b67ef-140">importance</span><span class="sxs-lookup"><span data-stu-id="b67ef-140">importance</span></span>|<span data-ttu-id="b67ef-141">String</span><span class="sxs-lookup"><span data-stu-id="b67ef-141">String</span></span>|<span data-ttu-id="b67ef-p105">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="b67ef-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="b67ef-144">isAllDay</span></span> |<span data-ttu-id="b67ef-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b67ef-145">Boolean</span></span>|<span data-ttu-id="b67ef-146">イベントが 1 日中続くかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="b67ef-147">このプロパティを調整するには、イベントの**startDateTime**および**enddatetime**プロパティの調整も必要です。</span><span class="sxs-lookup"><span data-stu-id="b67ef-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="b67ef-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b67ef-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="b67ef-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="b67ef-149">Boolean</span></span>|<span data-ttu-id="b67ef-150">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b67ef-151">isRead</span><span class="sxs-lookup"><span data-stu-id="b67ef-151">isRead</span></span>|<span data-ttu-id="b67ef-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="b67ef-152">Boolean</span></span>|<span data-ttu-id="b67ef-153">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="b67ef-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b67ef-154">isReadReceiptRequested</span></span>|<span data-ttu-id="b67ef-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="b67ef-155">Boolean</span></span>|<span data-ttu-id="b67ef-156">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="b67ef-157">応答</span><span class="sxs-lookup"><span data-stu-id="b67ef-157">Response</span></span>

<span data-ttu-id="b67ef-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b67ef-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b67ef-159">例</span><span class="sxs-lookup"><span data-stu-id="b67ef-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b67ef-160">要求</span><span class="sxs-lookup"><span data-stu-id="b67ef-160">Request</span></span>
<span data-ttu-id="b67ef-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b67ef-161">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b67ef-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b67ef-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b67ef-163">C#</span><span class="sxs-lookup"><span data-stu-id="b67ef-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b67ef-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b67ef-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b67ef-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="b67ef-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b67ef-166">応答</span><span class="sxs-lookup"><span data-stu-id="b67ef-166">Response</span></span>
<span data-ttu-id="b67ef-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b67ef-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
