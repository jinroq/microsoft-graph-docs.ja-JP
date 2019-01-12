---
title: rejectedSenders の一覧表示
description: 'このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: fbe4fd06bb12200326e8648a2736a40de5c8e288
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936285"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="7ffd8-103">rejectedSenders の一覧表示</span><span class="sxs-lookup"><span data-stu-id="7ffd8-103">List rejectedSenders</span></span>

> <span data-ttu-id="7ffd8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ffd8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ffd8-106">このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-106">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="7ffd8-p102">拒否送信者リスト内のユーザーは、グループの会話に投稿できません (取得要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-p102">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ffd8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ffd8-109">Permissions</span></span>
<span data-ttu-id="7ffd8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ffd8-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ffd8-112">Permission type</span></span>      | <span data-ttu-id="7ffd8-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ffd8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ffd8-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ffd8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7ffd8-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffd8-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ffd8-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ffd8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ffd8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-117">Not supported.</span></span>    |
|<span data-ttu-id="7ffd8-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ffd8-118">Application</span></span> | <span data-ttu-id="7ffd8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ffd8-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ffd8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ffd8-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ffd8-121">Optional query parameters</span></span>
<span data-ttu-id="7ffd8-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ffd8-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ffd8-123">Request headers</span></span>
| <span data-ttu-id="7ffd8-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ffd8-124">Header</span></span>       | <span data-ttu-id="7ffd8-125">値</span><span class="sxs-lookup"><span data-stu-id="7ffd8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ffd8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ffd8-126">Authorization</span></span>  | <span data-ttu-id="7ffd8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ffd8-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ffd8-129">Request body</span></span>
<span data-ttu-id="7ffd8-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ffd8-131">応答</span><span class="sxs-lookup"><span data-stu-id="7ffd8-131">Response</span></span>
<span data-ttu-id="7ffd8-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ffd8-133">例</span><span class="sxs-lookup"><span data-stu-id="7ffd8-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7ffd8-134">要求</span><span class="sxs-lookup"><span data-stu-id="7ffd8-134">Request</span></span>
<span data-ttu-id="7ffd8-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="7ffd8-136">応答</span><span class="sxs-lookup"><span data-stu-id="7ffd8-136">Response</span></span>
<span data-ttu-id="7ffd8-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-137">The following is an example of the response.</span></span>
><span data-ttu-id="7ffd8-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ffd8-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7ffd8-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
