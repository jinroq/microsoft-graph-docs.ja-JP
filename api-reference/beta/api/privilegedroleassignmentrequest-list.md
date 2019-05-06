---
title: リスト privilegedRoleAssignmentRequests
description: 'PrivilegedRoleAssignmentRequest のコレクションを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 887eeda1c357e31ffa56be0e2e0f9d5f5de041df
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593787"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="7bb23-103">リスト privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="7bb23-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb23-104">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7bb23-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="7bb23-105">**注:** この依頼者は、リソースに対して少なくとも1つのロール割り当てを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bb23-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bb23-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7bb23-106">Permissions</span></span>
<span data-ttu-id="7bb23-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bb23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb23-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bb23-109">Permission type</span></span>                        | <span data-ttu-id="7bb23-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bb23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bb23-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bb23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7bb23-112">PrivilegedAccess、AzureAD、Directory.accessasuser.all のいずれかのディレクトリを取得します。</span><span class="sxs-lookup"><span data-stu-id="7bb23-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7bb23-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bb23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bb23-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bb23-114">Not supported.</span></span> |
|<span data-ttu-id="7bb23-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bb23-115">Application</span></span>                            | <span data-ttu-id="7bb23-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bb23-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bb23-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bb23-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bb23-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7bb23-118">Optional query parameters</span></span>
<span data-ttu-id="7bb23-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7bb23-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bb23-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bb23-120">Request headers</span></span>
| <span data-ttu-id="7bb23-121">名前</span><span class="sxs-lookup"><span data-stu-id="7bb23-121">Name</span></span>      |<span data-ttu-id="7bb23-122">説明</span><span class="sxs-lookup"><span data-stu-id="7bb23-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bb23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bb23-123">Authorization</span></span>  | <span data-ttu-id="7bb23-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7bb23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bb23-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bb23-126">Request body</span></span>
<span data-ttu-id="7bb23-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7bb23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bb23-128">応答</span><span class="sxs-lookup"><span data-stu-id="7bb23-128">Response</span></span>
<span data-ttu-id="7bb23-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7bb23-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb23-130">例</span><span class="sxs-lookup"><span data-stu-id="7bb23-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bb23-131">要求</span><span class="sxs-lookup"><span data-stu-id="7bb23-131">Request</span></span>
<span data-ttu-id="7bb23-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bb23-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="7bb23-133">応答</span><span class="sxs-lookup"><span data-stu-id="7bb23-133">Response</span></span>
<span data-ttu-id="7bb23-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bb23-134">The following is an example of the response.</span></span> <span data-ttu-id="7bb23-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7bb23-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7bb23-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7bb23-136">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bb23-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="7bb23-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bb23-138">Visual</span><span class="sxs-lookup"><span data-stu-id="7bb23-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bb23-139">Java</span><span class="sxs-lookup"><span data-stu-id="7bb23-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
