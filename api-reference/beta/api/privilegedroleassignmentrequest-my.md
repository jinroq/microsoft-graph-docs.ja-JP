---
title: 'privilegedRoleAssignmentRequest: マイ'
description: 依頼者の特権を持つ役割の割り当て要求を取得します。
localization_priority: Normal
ms.openlocfilehash: 8f37224dd47be060f1ffc8a3551c537289edf966
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872164"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="c26d8-103">privilegedRoleAssignmentRequest: マイ</span><span class="sxs-lookup"><span data-stu-id="c26d8-103">privilegedRoleAssignmentRequest: my</span></span>

> <span data-ttu-id="c26d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c26d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c26d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c26d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c26d8-106">依頼者の特権を持つ役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="c26d8-106">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c26d8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c26d8-107">Permissions</span></span>
<span data-ttu-id="c26d8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c26d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c26d8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c26d8-110">Permission type</span></span>                        | <span data-ttu-id="c26d8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c26d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c26d8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c26d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c26d8-113">PrivilegedAccess.ReadWrite.AzureAD、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c26d8-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c26d8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c26d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c26d8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c26d8-115">Not supported.</span></span> |
|<span data-ttu-id="c26d8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c26d8-116">Application</span></span>                            | <span data-ttu-id="c26d8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c26d8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c26d8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c26d8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c26d8-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c26d8-119">Optional query parameters</span></span>
<span data-ttu-id="c26d8-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c26d8-120">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c26d8-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c26d8-121">Request headers</span></span>
| <span data-ttu-id="c26d8-122">名前</span><span class="sxs-lookup"><span data-stu-id="c26d8-122">Name</span></span>      |<span data-ttu-id="c26d8-123">説明</span><span class="sxs-lookup"><span data-stu-id="c26d8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c26d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c26d8-124">Authorization</span></span>  | <span data-ttu-id="c26d8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c26d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c26d8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c26d8-127">Request body</span></span>
<span data-ttu-id="c26d8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c26d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c26d8-129">応答</span><span class="sxs-lookup"><span data-stu-id="c26d8-129">Response</span></span>
<span data-ttu-id="c26d8-130">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c26d8-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26d8-131">例</span><span class="sxs-lookup"><span data-stu-id="c26d8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c26d8-132">要求</span><span class="sxs-lookup"><span data-stu-id="c26d8-132">Request</span></span>
<span data-ttu-id="c26d8-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c26d8-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="c26d8-134">応答</span><span class="sxs-lookup"><span data-stu-id="c26d8-134">Response</span></span>
<span data-ttu-id="c26d8-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c26d8-135">The following is an example of the response.</span></span> <span data-ttu-id="c26d8-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c26d8-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c26d8-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c26d8-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self"，
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self"，
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
