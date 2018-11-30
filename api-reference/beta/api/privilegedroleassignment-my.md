---
title: 'privilegedRoleAssignment: マイ'
description: 要求側の特権を持つ役割の割り当てを取得します。
ms.openlocfilehash: 7291d7ae27804c633f98a24ed7c36170e77c61e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069269"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="d77d3-103">privilegedRoleAssignment: マイ</span><span class="sxs-lookup"><span data-stu-id="d77d3-103">privilegedRoleAssignment: my</span></span>

> <span data-ttu-id="d77d3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d77d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d77d3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d77d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d77d3-106">要求側の特権を持つ役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="d77d3-106">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="d77d3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d77d3-107">Permissions</span></span>
<span data-ttu-id="d77d3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d77d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d77d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d77d3-110">Permission type</span></span>      | <span data-ttu-id="d77d3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d77d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d77d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d77d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d77d3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d77d3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d77d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d77d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d77d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d77d3-115">Not supported.</span></span>    |
|<span data-ttu-id="d77d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d77d3-116">Application</span></span> | <span data-ttu-id="d77d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d77d3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d77d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d77d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="d77d3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d77d3-119">Request headers</span></span>
| <span data-ttu-id="d77d3-120">名前</span><span class="sxs-lookup"><span data-stu-id="d77d3-120">Name</span></span>       | <span data-ttu-id="d77d3-121">説明</span><span class="sxs-lookup"><span data-stu-id="d77d3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d77d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d77d3-122">Authorization</span></span>  | <span data-ttu-id="d77d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d77d3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d77d3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d77d3-125">Request body</span></span>
<span data-ttu-id="d77d3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d77d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d77d3-127">応答</span><span class="sxs-lookup"><span data-stu-id="d77d3-127">Response</span></span>

<span data-ttu-id="d77d3-128">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d77d3-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d77d3-129">例</span><span class="sxs-lookup"><span data-stu-id="d77d3-129">Example</span></span>
<span data-ttu-id="d77d3-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d77d3-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d77d3-131">要求</span><span class="sxs-lookup"><span data-stu-id="d77d3-131">Request</span></span>
<span data-ttu-id="d77d3-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d77d3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="d77d3-133">応答</span><span class="sxs-lookup"><span data-stu-id="d77d3-133">Response</span></span>
<span data-ttu-id="d77d3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d77d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->