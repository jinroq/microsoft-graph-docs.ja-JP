---
title: 'privilegedApproval: myRequests'
description: 要求側の承認の要求を取得します。
localization_priority: Normal
ms.openlocfilehash: 26c8805d669b5786ac2c46821570f6cd29a99f2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806413"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="8d185-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="8d185-103">privilegedApproval: myRequests</span></span>

> <span data-ttu-id="8d185-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d185-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d185-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d185-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d185-106">要求側の承認の要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d185-106">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d185-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d185-107">Permissions</span></span>
<span data-ttu-id="8d185-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d185-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8d185-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d185-110">Permission type</span></span>      | <span data-ttu-id="8d185-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d185-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d185-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d185-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d185-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d185-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d185-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d185-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d185-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d185-115">Not supported.</span></span>    |
|<span data-ttu-id="8d185-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d185-116">Application</span></span> | <span data-ttu-id="8d185-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d185-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d185-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d185-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="8d185-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d185-119">Request headers</span></span>
| <span data-ttu-id="8d185-120">名前</span><span class="sxs-lookup"><span data-stu-id="8d185-120">Name</span></span>       | <span data-ttu-id="8d185-121">説明</span><span class="sxs-lookup"><span data-stu-id="8d185-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d185-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d185-122">Authorization</span></span>  | <span data-ttu-id="8d185-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d185-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d185-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d185-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8d185-126">応答</span><span class="sxs-lookup"><span data-stu-id="8d185-126">Response</span></span>

<span data-ttu-id="8d185-127">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8d185-127">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="8d185-128">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8d185-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8d185-129">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d185-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="8d185-130">例</span><span class="sxs-lookup"><span data-stu-id="8d185-130">Example</span></span>
<span data-ttu-id="8d185-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8d185-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d185-132">要求</span><span class="sxs-lookup"><span data-stu-id="8d185-132">Request</span></span>
<span data-ttu-id="8d185-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d185-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="8d185-134">応答</span><span class="sxs-lookup"><span data-stu-id="8d185-134">Response</span></span>
<span data-ttu-id="8d185-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d185-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
