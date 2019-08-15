---
title: リスト privilegedRoleAssignmentRequests
description: 'PrivilegedRoleAssignmentRequest のコレクションを取得します。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b014615714ea0535a4683013445deac6684dcfda
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412636"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="b579f-103">リスト privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="b579f-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b579f-104">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b579f-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="b579f-105">**注:** この依頼者は、リソースに対して少なくとも1つのロール割り当てを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b579f-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="b579f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b579f-106">Permissions</span></span>
<span data-ttu-id="b579f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b579f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b579f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b579f-109">Permission type</span></span>                        | <span data-ttu-id="b579f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b579f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b579f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b579f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b579f-112">PrivilegedAccess、AzureAD、Directory.accessasuser.all のいずれかのディレクトリを取得します。</span><span class="sxs-lookup"><span data-stu-id="b579f-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b579f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b579f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b579f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b579f-114">Not supported.</span></span> |
|<span data-ttu-id="b579f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b579f-115">Application</span></span>                            | <span data-ttu-id="b579f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b579f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b579f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b579f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b579f-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b579f-118">Optional query parameters</span></span>
<span data-ttu-id="b579f-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b579f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b579f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b579f-120">Request headers</span></span>
| <span data-ttu-id="b579f-121">名前</span><span class="sxs-lookup"><span data-stu-id="b579f-121">Name</span></span>      |<span data-ttu-id="b579f-122">説明</span><span class="sxs-lookup"><span data-stu-id="b579f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b579f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b579f-123">Authorization</span></span>  | <span data-ttu-id="b579f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b579f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b579f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b579f-126">Request body</span></span>
<span data-ttu-id="b579f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b579f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b579f-128">応答</span><span class="sxs-lookup"><span data-stu-id="b579f-128">Response</span></span>
<span data-ttu-id="b579f-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b579f-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b579f-130">例</span><span class="sxs-lookup"><span data-stu-id="b579f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b579f-131">要求</span><span class="sxs-lookup"><span data-stu-id="b579f-131">Request</span></span>
<span data-ttu-id="b579f-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b579f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b579f-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b579f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b579f-134">C#</span><span class="sxs-lookup"><span data-stu-id="b579f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b579f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b579f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b579f-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="b579f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b579f-137">応答</span><span class="sxs-lookup"><span data-stu-id="b579f-137">Response</span></span>
<span data-ttu-id="b579f-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b579f-138">The following is an example of the response.</span></span> <span data-ttu-id="b579f-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b579f-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b579f-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b579f-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
