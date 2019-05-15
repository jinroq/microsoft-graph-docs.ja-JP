---
title: List groupLifecyclePolicies
description: すべての groupLifecyclePolicies を一覧表示します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 17128d77444cc79ffd4e1954736a980bd550be2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33592405"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="6f274-103">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="6f274-103">List groupLifecyclePolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f274-104">すべての [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6f274-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f274-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f274-105">Permissions</span></span>

<span data-ttu-id="6f274-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f274-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f274-108">Permission type</span></span>      | <span data-ttu-id="6f274-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f274-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f274-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f274-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f274-111">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f274-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6f274-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f274-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f274-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6f274-113">Not supported</span></span> |
|<span data-ttu-id="6f274-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f274-114">Application</span></span> | <span data-ttu-id="6f274-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f274-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f274-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f274-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f274-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f274-117">Optional query parameters</span></span>
<span data-ttu-id="6f274-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6f274-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f274-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f274-119">Request headers</span></span>
| <span data-ttu-id="6f274-120">名前</span><span class="sxs-lookup"><span data-stu-id="6f274-120">Name</span></span> | <span data-ttu-id="6f274-121">説明</span><span class="sxs-lookup"><span data-stu-id="6f274-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="6f274-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f274-122">Authorization</span></span> | <span data-ttu-id="6f274-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6f274-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f274-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f274-125">Request body</span></span>
<span data-ttu-id="6f274-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f274-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f274-127">応答</span><span class="sxs-lookup"><span data-stu-id="6f274-127">Response</span></span>

<span data-ttu-id="6f274-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6f274-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f274-129">例</span><span class="sxs-lookup"><span data-stu-id="6f274-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f274-130">要求</span><span class="sxs-lookup"><span data-stu-id="6f274-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="6f274-131">応答</span><span class="sxs-lookup"><span data-stu-id="6f274-131">Response</span></span>

<span data-ttu-id="6f274-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6f274-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6f274-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="6f274-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6f274-135">C#</span><span class="sxs-lookup"><span data-stu-id="6f274-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f274-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f274-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
