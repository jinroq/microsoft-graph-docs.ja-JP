---
title: eventMessage の更新
description: eventMessage オブジェクトのプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: 20c910ae2d6562a4bb9a593a0fac32269dbd413f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320425"
---
# <a name="update-eventmessage"></a><span data-ttu-id="94247-103">eventMessage の更新</span><span class="sxs-lookup"><span data-stu-id="94247-103">Update eventMessage</span></span>

<span data-ttu-id="94247-104">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94247-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94247-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94247-105">Permissions</span></span>
<span data-ttu-id="94247-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94247-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94247-108">Permission type</span></span>      | <span data-ttu-id="94247-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94247-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94247-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94247-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94247-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94247-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94247-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94247-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94247-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94247-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94247-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94247-114">Application</span></span> | <span data-ttu-id="94247-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94247-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94247-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94247-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94247-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94247-117">Request headers</span></span>
| <span data-ttu-id="94247-118">名前</span><span class="sxs-lookup"><span data-stu-id="94247-118">Name</span></span>       | <span data-ttu-id="94247-119">種類</span><span class="sxs-lookup"><span data-stu-id="94247-119">Type</span></span> | <span data-ttu-id="94247-120">説明</span><span class="sxs-lookup"><span data-stu-id="94247-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94247-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94247-121">Authorization</span></span>  | <span data-ttu-id="94247-122">string</span><span class="sxs-lookup"><span data-stu-id="94247-122">string</span></span>  | <span data-ttu-id="94247-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94247-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94247-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94247-125">Content-Type</span></span> | <span data-ttu-id="94247-126">string</span><span class="sxs-lookup"><span data-stu-id="94247-126">string</span></span>  | <span data-ttu-id="94247-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="94247-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="94247-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="94247-129">Request body</span></span>
<span data-ttu-id="94247-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="94247-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="94247-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94247-134">Property</span></span>     | <span data-ttu-id="94247-135">種類</span><span class="sxs-lookup"><span data-stu-id="94247-135">Type</span></span>   |<span data-ttu-id="94247-136">説明</span><span class="sxs-lookup"><span data-stu-id="94247-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94247-137">categories</span><span class="sxs-lookup"><span data-stu-id="94247-137">categories</span></span>|<span data-ttu-id="94247-138">String</span><span class="sxs-lookup"><span data-stu-id="94247-138">String</span></span>|<span data-ttu-id="94247-139">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="94247-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="94247-140">importance</span><span class="sxs-lookup"><span data-stu-id="94247-140">importance</span></span>|<span data-ttu-id="94247-141">String</span><span class="sxs-lookup"><span data-stu-id="94247-141">String</span></span>|<span data-ttu-id="94247-142">メッセージの重要性。</span><span class="sxs-lookup"><span data-stu-id="94247-142">The importance of the message.</span></span> <span data-ttu-id="94247-143">可能な値: `Low`、 `Normal`、 `High`。</span><span class="sxs-lookup"><span data-stu-id="94247-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="94247-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="94247-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="94247-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="94247-145">Boolean</span></span>|<span data-ttu-id="94247-146">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="94247-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="94247-147">isRead</span><span class="sxs-lookup"><span data-stu-id="94247-147">isRead</span></span>|<span data-ttu-id="94247-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="94247-148">Boolean</span></span>|<span data-ttu-id="94247-149">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="94247-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="94247-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="94247-150">isReadReceiptRequested</span></span>|<span data-ttu-id="94247-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="94247-151">Boolean</span></span>|<span data-ttu-id="94247-152">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="94247-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="94247-153">応答</span><span class="sxs-lookup"><span data-stu-id="94247-153">Response</span></span>

<span data-ttu-id="94247-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94247-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94247-155">例</span><span class="sxs-lookup"><span data-stu-id="94247-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94247-156">要求</span><span class="sxs-lookup"><span data-stu-id="94247-156">Request</span></span>
<span data-ttu-id="94247-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94247-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="94247-158">応答</span><span class="sxs-lookup"><span data-stu-id="94247-158">Response</span></span>
<span data-ttu-id="94247-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94247-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
