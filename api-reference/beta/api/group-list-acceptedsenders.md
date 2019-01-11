---
title: acceptedSenders のリスト化
description: このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b073ea0a6173c86b298628c7e78baaaf0512eaac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892401"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="02f32-103">acceptedSenders のリスト化</span><span class="sxs-lookup"><span data-stu-id="02f32-103">List acceptedSenders</span></span>

> <span data-ttu-id="02f32-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02f32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02f32-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02f32-106">このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="02f32-106">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="02f32-p102">承諾済み送信者リスト内のユーザーは、グループの会話を投稿することができます (要求取得 URL で識別)。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="02f32-p102">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="02f32-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02f32-109">Permissions</span></span>
<span data-ttu-id="02f32-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02f32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f32-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02f32-112">Permission type</span></span>      | <span data-ttu-id="02f32-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02f32-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02f32-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02f32-114">Delegated (work or school account)</span></span> | <span data-ttu-id="02f32-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f32-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02f32-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02f32-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02f32-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f32-117">Not supported.</span></span>    |
|<span data-ttu-id="02f32-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02f32-118">Application</span></span> | <span data-ttu-id="02f32-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f32-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02f32-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02f32-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02f32-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02f32-121">Optional query parameters</span></span>
<span data-ttu-id="02f32-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02f32-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02f32-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f32-123">Request headers</span></span>
| <span data-ttu-id="02f32-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f32-124">Header</span></span>       | <span data-ttu-id="02f32-125">値</span><span class="sxs-lookup"><span data-stu-id="02f32-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02f32-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f32-126">Authorization</span></span>  | <span data-ttu-id="02f32-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02f32-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02f32-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="02f32-129">Request body</span></span>
<span data-ttu-id="02f32-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02f32-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02f32-131">応答</span><span class="sxs-lookup"><span data-stu-id="02f32-131">Response</span></span>
<span data-ttu-id="02f32-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="02f32-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02f32-133">例</span><span class="sxs-lookup"><span data-stu-id="02f32-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="02f32-134">要求</span><span class="sxs-lookup"><span data-stu-id="02f32-134">Request</span></span>
<span data-ttu-id="02f32-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02f32-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="02f32-136">応答</span><span class="sxs-lookup"><span data-stu-id="02f32-136">Response</span></span>
<span data-ttu-id="02f32-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02f32-137">The following is an example of the response.</span></span>
><span data-ttu-id="02f32-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="02f32-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="02f32-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="02f32-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
