---
title: rejectedSenders の一覧表示
description: 'このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 14bf57133ad953d40c3cf39cca4cdf8c4f9f19f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986342"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="2effe-103">rejectedSenders の一覧表示</span><span class="sxs-lookup"><span data-stu-id="2effe-103">List rejectedSenders</span></span>
<span data-ttu-id="2effe-104">このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2effe-104">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="2effe-p101">拒否送信者リスト内のユーザーは、グループの会話に投稿できません (取得要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="2effe-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2effe-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2effe-107">Permissions</span></span>
<span data-ttu-id="2effe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2effe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2effe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2effe-110">Permission type</span></span>      | <span data-ttu-id="2effe-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2effe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2effe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2effe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2effe-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2effe-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2effe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2effe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2effe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2effe-115">Not supported.</span></span>    |
|<span data-ttu-id="2effe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2effe-116">Application</span></span> | <span data-ttu-id="2effe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2effe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2effe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2effe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2effe-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2effe-119">Optional query parameters</span></span>
<span data-ttu-id="2effe-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2effe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2effe-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2effe-121">Request headers</span></span>
| <span data-ttu-id="2effe-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2effe-122">Header</span></span>       | <span data-ttu-id="2effe-123">値</span><span class="sxs-lookup"><span data-stu-id="2effe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2effe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2effe-124">Authorization</span></span>  | <span data-ttu-id="2effe-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2effe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2effe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2effe-127">Request body</span></span>
<span data-ttu-id="2effe-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2effe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2effe-129">応答</span><span class="sxs-lookup"><span data-stu-id="2effe-129">Response</span></span>
<span data-ttu-id="2effe-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2effe-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2effe-131">例</span><span class="sxs-lookup"><span data-stu-id="2effe-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2effe-132">要求</span><span class="sxs-lookup"><span data-stu-id="2effe-132">Request</span></span>
<span data-ttu-id="2effe-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2effe-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="2effe-134">応答</span><span class="sxs-lookup"><span data-stu-id="2effe-134">Response</span></span>
<span data-ttu-id="2effe-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2effe-135">The following is an example of the response.</span></span>
><span data-ttu-id="2effe-136">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2effe-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2effe-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2effe-137">All the properties will be returned from an actual call.</span></span>
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
