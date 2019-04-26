---
title: acceptedSenders のリスト化
description: このグループの承認済み送信者リストに含まれるユーザーまたはグループの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a29fe42dc7a34939a41120caf03c59cc7662e5b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345667"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="09b40-103">acceptedSenders のリスト化</span><span class="sxs-lookup"><span data-stu-id="09b40-103">List acceptedSenders</span></span>
<span data-ttu-id="09b40-104">このグループの承認済み送信者リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09b40-104">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="09b40-p101">承諾済み送信者リスト内のユーザーは、グループの会話を投稿することができます (要求取得 URL で識別)。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="09b40-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="09b40-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09b40-107">Permissions</span></span>
<span data-ttu-id="09b40-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09b40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b40-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09b40-110">Permission type</span></span>      | <span data-ttu-id="09b40-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09b40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09b40-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09b40-112">Delegated (work or school account)</span></span> | <span data-ttu-id="09b40-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b40-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="09b40-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09b40-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09b40-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09b40-115">Not supported.</span></span>    |
|<span data-ttu-id="09b40-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09b40-116">Application</span></span> | <span data-ttu-id="09b40-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09b40-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09b40-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09b40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09b40-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="09b40-119">Optional query parameters</span></span>
<span data-ttu-id="09b40-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="09b40-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09b40-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09b40-121">Request headers</span></span>
| <span data-ttu-id="09b40-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09b40-122">Header</span></span>       | <span data-ttu-id="09b40-123">値</span><span class="sxs-lookup"><span data-stu-id="09b40-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09b40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09b40-124">Authorization</span></span>  | <span data-ttu-id="09b40-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09b40-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09b40-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="09b40-127">Request body</span></span>
<span data-ttu-id="09b40-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09b40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09b40-129">応答</span><span class="sxs-lookup"><span data-stu-id="09b40-129">Response</span></span>
<span data-ttu-id="09b40-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="09b40-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09b40-131">例</span><span class="sxs-lookup"><span data-stu-id="09b40-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="09b40-132">要求</span><span class="sxs-lookup"><span data-stu-id="09b40-132">Request</span></span>
<span data-ttu-id="09b40-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09b40-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="09b40-134">応答</span><span class="sxs-lookup"><span data-stu-id="09b40-134">Response</span></span>
<span data-ttu-id="09b40-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09b40-135">The following is an example of the response.</span></span>
><span data-ttu-id="09b40-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="09b40-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09b40-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="09b40-137">All the properties will be returned from an actual call.</span></span>
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
