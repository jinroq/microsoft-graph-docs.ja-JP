---
title: eventMessage の更新
description: eventMessage オブジェクトのプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: 922f17528b864c8cdfae39a4df475a0a61f40103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302472"
---
# <a name="update-eventmessage"></a><span data-ttu-id="633ef-103">eventMessage の更新</span><span class="sxs-lookup"><span data-stu-id="633ef-103">Update eventMessage</span></span>

> <span data-ttu-id="633ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="633ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="633ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="633ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="633ef-106">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="633ef-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="633ef-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="633ef-107">Permissions</span></span>
<span data-ttu-id="633ef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="633ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="633ef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="633ef-110">Permission type</span></span>      | <span data-ttu-id="633ef-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="633ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="633ef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="633ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="633ef-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="633ef-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="633ef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="633ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="633ef-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="633ef-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="633ef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="633ef-116">Application</span></span> | <span data-ttu-id="633ef-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="633ef-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="633ef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="633ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="633ef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="633ef-119">Request headers</span></span>
| <span data-ttu-id="633ef-120">名前</span><span class="sxs-lookup"><span data-stu-id="633ef-120">Name</span></span>       | <span data-ttu-id="633ef-121">種類</span><span class="sxs-lookup"><span data-stu-id="633ef-121">Type</span></span> | <span data-ttu-id="633ef-122">説明</span><span class="sxs-lookup"><span data-stu-id="633ef-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="633ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="633ef-123">Authorization</span></span>  | <span data-ttu-id="633ef-124">string</span><span class="sxs-lookup"><span data-stu-id="633ef-124">string</span></span>  | <span data-ttu-id="633ef-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="633ef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="633ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="633ef-127">Content-Type</span></span> | <span data-ttu-id="633ef-128">string</span><span class="sxs-lookup"><span data-stu-id="633ef-128">string</span></span>  | <span data-ttu-id="633ef-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="633ef-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="633ef-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="633ef-131">Request body</span></span>
<span data-ttu-id="633ef-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="633ef-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="633ef-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="633ef-136">Property</span></span>     | <span data-ttu-id="633ef-137">種類</span><span class="sxs-lookup"><span data-stu-id="633ef-137">Type</span></span>   |<span data-ttu-id="633ef-138">説明</span><span class="sxs-lookup"><span data-stu-id="633ef-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="633ef-139">categories</span><span class="sxs-lookup"><span data-stu-id="633ef-139">categories</span></span>|<span data-ttu-id="633ef-140">String</span><span class="sxs-lookup"><span data-stu-id="633ef-140">String</span></span>|<span data-ttu-id="633ef-141">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="633ef-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="633ef-142">importance</span><span class="sxs-lookup"><span data-stu-id="633ef-142">importance</span></span>|<span data-ttu-id="633ef-143">String</span><span class="sxs-lookup"><span data-stu-id="633ef-143">String</span></span>|<span data-ttu-id="633ef-p106">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="633ef-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="633ef-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="633ef-146">isAllDay</span></span> |<span data-ttu-id="633ef-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="633ef-147">Boolean</span></span>|<span data-ttu-id="633ef-148">イベントが 1 日中続くかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="633ef-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="633ef-149">このプロパティを調整するには、イベントにも**させる**し、 **endDateTime**プロパティを調整する必要があります。</span><span class="sxs-lookup"><span data-stu-id="633ef-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="633ef-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="633ef-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="633ef-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="633ef-151">Boolean</span></span>|<span data-ttu-id="633ef-152">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="633ef-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="633ef-153">isRead</span><span class="sxs-lookup"><span data-stu-id="633ef-153">isRead</span></span>|<span data-ttu-id="633ef-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="633ef-154">Boolean</span></span>|<span data-ttu-id="633ef-155">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="633ef-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="633ef-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="633ef-156">isReadReceiptRequested</span></span>|<span data-ttu-id="633ef-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="633ef-157">Boolean</span></span>|<span data-ttu-id="633ef-158">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="633ef-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="633ef-159">応答</span><span class="sxs-lookup"><span data-stu-id="633ef-159">Response</span></span>

<span data-ttu-id="633ef-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="633ef-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="633ef-161">例</span><span class="sxs-lookup"><span data-stu-id="633ef-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="633ef-162">要求</span><span class="sxs-lookup"><span data-stu-id="633ef-162">Request</span></span>
<span data-ttu-id="633ef-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="633ef-163">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="633ef-164">応答</span><span class="sxs-lookup"><span data-stu-id="633ef-164">Response</span></span>
<span data-ttu-id="633ef-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="633ef-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
