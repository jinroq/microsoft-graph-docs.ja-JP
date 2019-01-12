---
title: Update conversationthread
description: スレッドへの以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 99ed0a7c635fc02bd0b0c6ea485e18a5875d8fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985082"
---
# <a name="update-conversationthread"></a><span data-ttu-id="c2d42-103">Update conversationthread</span><span class="sxs-lookup"><span data-stu-id="c2d42-103">Update conversationthread</span></span>

> <span data-ttu-id="c2d42-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2d42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2d42-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2d42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2d42-106">スレッドへの以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。</span><span class="sxs-lookup"><span data-stu-id="c2d42-106">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2d42-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2d42-107">Permissions</span></span>
<span data-ttu-id="c2d42-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2d42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2d42-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2d42-110">Permission type</span></span>      | <span data-ttu-id="c2d42-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2d42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2d42-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2d42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2d42-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d42-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2d42-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2d42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2d42-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2d42-115">Not supported.</span></span>    |
|<span data-ttu-id="c2d42-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2d42-116">Application</span></span> | <span data-ttu-id="c2d42-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d42-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2d42-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2d42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c2d42-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2d42-119">Request headers</span></span>
| <span data-ttu-id="c2d42-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2d42-120">Header</span></span>       | <span data-ttu-id="c2d42-121">値</span><span class="sxs-lookup"><span data-stu-id="c2d42-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2d42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2d42-122">Authorization</span></span>  | <span data-ttu-id="c2d42-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2d42-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2d42-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2d42-125">Content-Type</span></span>  | <span data-ttu-id="c2d42-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c2d42-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2d42-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2d42-128">Request body</span></span>
<span data-ttu-id="c2d42-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c2d42-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2d42-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2d42-132">Property</span></span>     | <span data-ttu-id="c2d42-133">種類</span><span class="sxs-lookup"><span data-stu-id="c2d42-133">Type</span></span>   |<span data-ttu-id="c2d42-134">説明</span><span class="sxs-lookup"><span data-stu-id="c2d42-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2d42-135">isLocked</span><span class="sxs-lookup"><span data-stu-id="c2d42-135">isLocked</span></span>|<span data-ttu-id="c2d42-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2d42-136">Boolean</span></span>|<span data-ttu-id="c2d42-p106">スレッドがロックされているかどうかを示します。転記を禁止するために `true` に設定します。</span><span class="sxs-lookup"><span data-stu-id="c2d42-p106">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="c2d42-139">応答</span><span class="sxs-lookup"><span data-stu-id="c2d42-139">Response</span></span>

<span data-ttu-id="c2d42-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c2d42-140">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2d42-141">例</span><span class="sxs-lookup"><span data-stu-id="c2d42-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2d42-142">要求</span><span class="sxs-lookup"><span data-stu-id="c2d42-142">Request</span></span>
<span data-ttu-id="c2d42-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2d42-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="c2d42-144">応答</span><span class="sxs-lookup"><span data-stu-id="c2d42-144">Response</span></span>
<span data-ttu-id="c2d42-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2d42-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
