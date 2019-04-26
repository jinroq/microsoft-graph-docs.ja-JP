---
title: 'privilegedRoleAssignment: my'
description: 要求者の特権の役割の割り当てを取得します。
localization_priority: Normal
ms.openlocfilehash: acf03e62eff3195fb922a324a231e5d58f768b11
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337314"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="1e080-103">privilegedRoleAssignment: my</span><span class="sxs-lookup"><span data-stu-id="1e080-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e080-104">要求者の特権の役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e080-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e080-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e080-105">Permissions</span></span>
<span data-ttu-id="1e080-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e080-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e080-108">Permission type</span></span>      | <span data-ttu-id="1e080-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e080-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e080-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e080-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e080-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e080-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e080-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e080-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e080-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e080-113">Not supported.</span></span>    |
|<span data-ttu-id="1e080-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e080-114">Application</span></span> | <span data-ttu-id="1e080-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e080-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e080-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e080-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="1e080-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e080-117">Request headers</span></span>
| <span data-ttu-id="1e080-118">名前</span><span class="sxs-lookup"><span data-stu-id="1e080-118">Name</span></span>       | <span data-ttu-id="1e080-119">説明</span><span class="sxs-lookup"><span data-stu-id="1e080-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e080-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e080-120">Authorization</span></span>  | <span data-ttu-id="1e080-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e080-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e080-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e080-123">Request body</span></span>
<span data-ttu-id="1e080-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e080-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e080-125">応答</span><span class="sxs-lookup"><span data-stu-id="1e080-125">Response</span></span>

<span data-ttu-id="1e080-126">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e080-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e080-127">例</span><span class="sxs-lookup"><span data-stu-id="1e080-127">Example</span></span>
<span data-ttu-id="1e080-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1e080-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e080-129">要求</span><span class="sxs-lookup"><span data-stu-id="1e080-129">Request</span></span>
<span data-ttu-id="1e080-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e080-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="1e080-131">応答</span><span class="sxs-lookup"><span data-stu-id="1e080-131">Response</span></span>
<span data-ttu-id="1e080-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e080-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
