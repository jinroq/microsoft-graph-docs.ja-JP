---
title: リスト privilegedRoleAssignmentRequests
description: 'PrivilegedRoleAssignmentRequest のコレクションを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 4bae072caeb54c513e9146fe36dfd100ce1b4360
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838704"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="e1417-103">リスト privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e1417-103">List privilegedRoleAssignmentRequests</span></span>

> <span data-ttu-id="e1417-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1417-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1417-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1417-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1417-106">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1417-106">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="e1417-107">**注:** この依頼者、リソースの 1 つ以上のロールの割り当てが必要です。</span><span class="sxs-lookup"><span data-stu-id="e1417-107">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1417-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1417-108">Permissions</span></span>
<span data-ttu-id="e1417-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1417-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1417-111">Permission type</span></span>                        | <span data-ttu-id="e1417-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1417-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1417-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1417-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1417-114">PrivilegedAccess.ReadWrite.AzureAD、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1417-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1417-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1417-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1417-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1417-116">Not supported.</span></span> |
|<span data-ttu-id="e1417-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1417-117">Application</span></span>                            | <span data-ttu-id="e1417-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1417-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1417-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1417-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1417-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e1417-120">Optional query parameters</span></span>
<span data-ttu-id="e1417-121">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e1417-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1417-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1417-122">Request headers</span></span>
| <span data-ttu-id="e1417-123">名前</span><span class="sxs-lookup"><span data-stu-id="e1417-123">Name</span></span>      |<span data-ttu-id="e1417-124">説明</span><span class="sxs-lookup"><span data-stu-id="e1417-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1417-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1417-125">Authorization</span></span>  | <span data-ttu-id="e1417-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1417-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1417-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1417-128">Request body</span></span>
<span data-ttu-id="e1417-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1417-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1417-130">応答</span><span class="sxs-lookup"><span data-stu-id="e1417-130">Response</span></span>
<span data-ttu-id="e1417-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e1417-131">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1417-132">例</span><span class="sxs-lookup"><span data-stu-id="e1417-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1417-133">要求</span><span class="sxs-lookup"><span data-stu-id="e1417-133">Request</span></span>
<span data-ttu-id="e1417-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1417-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="e1417-135">応答</span><span class="sxs-lookup"><span data-stu-id="e1417-135">Response</span></span>
<span data-ttu-id="e1417-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1417-136">The following is an example of the response.</span></span> <span data-ttu-id="e1417-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e1417-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1417-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e1417-138">All of the properties will be returned from an actual call.</span></span>
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
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
