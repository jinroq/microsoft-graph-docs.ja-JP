---
title: Update conversationthread
description: スレッドに以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a4f09f77c5f11a0933956dd60c9b15ff6be3116f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564093"
---
# <a name="update-conversationthread"></a><span data-ttu-id="ff4a0-103">Update conversationthread</span><span class="sxs-lookup"><span data-stu-id="ff4a0-103">Update conversationthread</span></span>

<span data-ttu-id="ff4a0-104">スレッドに以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff4a0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff4a0-105">Permissions</span></span>
<span data-ttu-id="ff4a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff4a0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff4a0-108">Permission type</span></span>      | <span data-ttu-id="ff4a0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff4a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff4a0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff4a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff4a0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff4a0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff4a0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff4a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff4a0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-113">Not supported.</span></span>    |
|<span data-ttu-id="ff4a0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff4a0-114">Application</span></span> | <span data-ttu-id="ff4a0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff4a0-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff4a0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff4a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ff4a0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff4a0-117">Request headers</span></span>
| <span data-ttu-id="ff4a0-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff4a0-118">Header</span></span>       | <span data-ttu-id="ff4a0-119">値</span><span class="sxs-lookup"><span data-stu-id="ff4a0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff4a0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff4a0-120">Authorization</span></span>  | <span data-ttu-id="ff4a0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff4a0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff4a0-123">Content-Type</span></span>  | <span data-ttu-id="ff4a0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff4a0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff4a0-126">Request body</span></span>
<span data-ttu-id="ff4a0-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff4a0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff4a0-130">Property</span></span>     | <span data-ttu-id="ff4a0-131">型</span><span class="sxs-lookup"><span data-stu-id="ff4a0-131">Type</span></span>   |<span data-ttu-id="ff4a0-132">説明</span><span class="sxs-lookup"><span data-stu-id="ff4a0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff4a0-133">resource.islocked</span><span class="sxs-lookup"><span data-stu-id="ff4a0-133">isLocked</span></span>|<span data-ttu-id="ff4a0-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="ff4a0-134">Boolean</span></span>|<span data-ttu-id="ff4a0-p105">スレッドがロックされているかどうかを示します。転記を禁止するために `true` に設定します。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="ff4a0-137">応答</span><span class="sxs-lookup"><span data-stu-id="ff4a0-137">Response</span></span>

<span data-ttu-id="ff4a0-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff4a0-139">例</span><span class="sxs-lookup"><span data-stu-id="ff4a0-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff4a0-140">要求</span><span class="sxs-lookup"><span data-stu-id="ff4a0-140">Request</span></span>
<span data-ttu-id="ff4a0-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="ff4a0-142">応答</span><span class="sxs-lookup"><span data-stu-id="ff4a0-142">Response</span></span>
<span data-ttu-id="ff4a0-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff4a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
