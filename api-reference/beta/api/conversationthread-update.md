---
title: Update conversationthread
description: スレッドに以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 38e79a96b9d7d41d36188db0a51f8626dd73d1d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943065"
---
# <a name="update-conversationthread"></a><span data-ttu-id="1a2a8-103">Update conversationthread</span><span class="sxs-lookup"><span data-stu-id="1a2a8-103">Update conversationthread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a2a8-104">スレッドに以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a2a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a2a8-105">Permissions</span></span>
<span data-ttu-id="1a2a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a2a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a2a8-108">Permission type</span></span>      | <span data-ttu-id="1a2a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a2a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a2a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a2a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a2a8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2a8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a2a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a2a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a2a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-113">Not supported.</span></span>    |
|<span data-ttu-id="1a2a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a2a8-114">Application</span></span> | <span data-ttu-id="1a2a8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2a8-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a2a8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a2a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1a2a8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a2a8-117">Request headers</span></span>
| <span data-ttu-id="1a2a8-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a2a8-118">Header</span></span>       | <span data-ttu-id="1a2a8-119">値</span><span class="sxs-lookup"><span data-stu-id="1a2a8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a2a8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a2a8-120">Authorization</span></span>  | <span data-ttu-id="1a2a8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1a2a8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a2a8-123">Content-Type</span></span>  | <span data-ttu-id="1a2a8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a2a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a2a8-126">Request body</span></span>
<span data-ttu-id="1a2a8-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1a2a8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a2a8-130">Property</span></span>     | <span data-ttu-id="1a2a8-131">型</span><span class="sxs-lookup"><span data-stu-id="1a2a8-131">Type</span></span>   |<span data-ttu-id="1a2a8-132">説明</span><span class="sxs-lookup"><span data-stu-id="1a2a8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a2a8-133">Resource.islocked</span><span class="sxs-lookup"><span data-stu-id="1a2a8-133">isLocked</span></span>|<span data-ttu-id="1a2a8-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="1a2a8-134">Boolean</span></span>|<span data-ttu-id="1a2a8-p105">スレッドがロックされているかどうかを示します。転記を禁止するために `true` に設定します。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="1a2a8-137">応答</span><span class="sxs-lookup"><span data-stu-id="1a2a8-137">Response</span></span>

<span data-ttu-id="1a2a8-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a2a8-139">例</span><span class="sxs-lookup"><span data-stu-id="1a2a8-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a2a8-140">要求</span><span class="sxs-lookup"><span data-stu-id="1a2a8-140">Request</span></span>
<span data-ttu-id="1a2a8-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a2a8-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1a2a8-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a2a8-143">C#</span><span class="sxs-lookup"><span data-stu-id="1a2a8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a2a8-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a2a8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a2a8-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="1a2a8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a2a8-146">Java</span><span class="sxs-lookup"><span data-stu-id="1a2a8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a2a8-147">応答</span><span class="sxs-lookup"><span data-stu-id="1a2a8-147">Response</span></span>
<span data-ttu-id="1a2a8-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a2a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
