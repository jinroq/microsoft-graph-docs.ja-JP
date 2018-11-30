---
title: List groupLifecyclePolicies
description: すべての groupLifecyclePolicies を一覧表示します。
ms.openlocfilehash: 1294120772aecf6f14c0bf71e463e18825285c19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022166"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="41f26-103">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="41f26-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="41f26-104">すべての [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="41f26-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41f26-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41f26-105">Permissions</span></span>

<span data-ttu-id="41f26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="41f26-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41f26-108">Permission type</span></span>      | <span data-ttu-id="41f26-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41f26-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41f26-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41f26-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41f26-111">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f26-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="41f26-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41f26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41f26-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41f26-113">Not supported.</span></span>    |
|<span data-ttu-id="41f26-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41f26-114">Application</span></span> | <span data-ttu-id="41f26-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f26-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41f26-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41f26-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41f26-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41f26-117">Optional query parameters</span></span>
<span data-ttu-id="41f26-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41f26-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41f26-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41f26-119">Request headers</span></span>
| <span data-ttu-id="41f26-120">名前</span><span class="sxs-lookup"><span data-stu-id="41f26-120">Name</span></span> | <span data-ttu-id="41f26-121">説明</span><span class="sxs-lookup"><span data-stu-id="41f26-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="41f26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41f26-122">Authorization</span></span> | <span data-ttu-id="41f26-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="41f26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41f26-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="41f26-125">Request body</span></span>
<span data-ttu-id="41f26-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41f26-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41f26-127">応答</span><span class="sxs-lookup"><span data-stu-id="41f26-127">Response</span></span>

<span data-ttu-id="41f26-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="41f26-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f26-129">例</span><span class="sxs-lookup"><span data-stu-id="41f26-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41f26-130">要求</span><span class="sxs-lookup"><span data-stu-id="41f26-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="41f26-131">応答</span><span class="sxs-lookup"><span data-stu-id="41f26-131">Response</span></span>

<span data-ttu-id="41f26-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41f26-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->