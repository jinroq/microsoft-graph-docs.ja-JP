---
title: 'privilegedRoleAssignmentRequest: my'
description: 要求者の特権の役割の割り当て要求を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d9a2f5d961f53e030cac0a0b3a82705d2228938e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412622"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="7fabe-103">privilegedRoleAssignmentRequest: my</span><span class="sxs-lookup"><span data-stu-id="7fabe-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fabe-104">要求者の特権の役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="7fabe-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fabe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7fabe-105">Permissions</span></span>
<span data-ttu-id="7fabe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7fabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fabe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7fabe-108">Permission type</span></span>                        | <span data-ttu-id="7fabe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7fabe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fabe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7fabe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fabe-111">PrivilegedAccess、AzureAD、Directory.accessasuser.all のいずれかのディレクトリを取得します。</span><span class="sxs-lookup"><span data-stu-id="7fabe-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7fabe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7fabe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fabe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fabe-113">Not supported.</span></span> |
|<span data-ttu-id="7fabe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7fabe-114">Application</span></span>                            | <span data-ttu-id="7fabe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fabe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fabe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7fabe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7fabe-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7fabe-117">Optional query parameters</span></span>
<span data-ttu-id="7fabe-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7fabe-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fabe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fabe-119">Request headers</span></span>
| <span data-ttu-id="7fabe-120">名前</span><span class="sxs-lookup"><span data-stu-id="7fabe-120">Name</span></span>      |<span data-ttu-id="7fabe-121">説明</span><span class="sxs-lookup"><span data-stu-id="7fabe-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fabe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fabe-122">Authorization</span></span>  | <span data-ttu-id="7fabe-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7fabe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fabe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7fabe-125">Request body</span></span>
<span data-ttu-id="7fabe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7fabe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fabe-127">応答</span><span class="sxs-lookup"><span data-stu-id="7fabe-127">Response</span></span>
<span data-ttu-id="7fabe-128">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7fabe-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fabe-129">例</span><span class="sxs-lookup"><span data-stu-id="7fabe-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fabe-130">要求</span><span class="sxs-lookup"><span data-stu-id="7fabe-130">Request</span></span>
<span data-ttu-id="7fabe-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fabe-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fabe-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7fabe-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fabe-133">C#</span><span class="sxs-lookup"><span data-stu-id="7fabe-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fabe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fabe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fabe-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="7fabe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7fabe-136">応答</span><span class="sxs-lookup"><span data-stu-id="7fabe-136">Response</span></span>
<span data-ttu-id="7fabe-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fabe-137">The following is an example of the response.</span></span> <span data-ttu-id="7fabe-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7fabe-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7fabe-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7fabe-139">All of the properties will be returned from an actual call.</span></span>
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
         "userId": "Self",
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
        "userId": "Self",
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
