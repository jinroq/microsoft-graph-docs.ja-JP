---
title: List groupLifecyclePolicies
description: グループが属する groupLifecyclePolicy オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 034b9d0ff3a61a976a61c19cd0be83ed49e6d1e9
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812790"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="f957a-103">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="f957a-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="f957a-104">グループが属する [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f957a-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="f957a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f957a-105">Permissions</span></span>

<span data-ttu-id="f957a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f957a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f957a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f957a-108">Permission type</span></span>      | <span data-ttu-id="f957a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f957a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f957a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f957a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f957a-111">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f957a-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f957a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f957a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f957a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f957a-113">Not supported.</span></span>    |
|<span data-ttu-id="f957a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f957a-114">Application</span></span> | <span data-ttu-id="f957a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f957a-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f957a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f957a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f957a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f957a-117">Optional query parameters</span></span>
<span data-ttu-id="f957a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f957a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f957a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f957a-119">Request headers</span></span>
| <span data-ttu-id="f957a-120">名前</span><span class="sxs-lookup"><span data-stu-id="f957a-120">Name</span></span> | <span data-ttu-id="f957a-121">説明</span><span class="sxs-lookup"><span data-stu-id="f957a-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f957a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f957a-122">Authorization</span></span> | <span data-ttu-id="f957a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f957a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f957a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f957a-125">Request body</span></span>
<span data-ttu-id="f957a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f957a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f957a-127">応答</span><span class="sxs-lookup"><span data-stu-id="f957a-127">Response</span></span>
<span data-ttu-id="f957a-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f957a-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f957a-129">例</span><span class="sxs-lookup"><span data-stu-id="f957a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f957a-130">要求</span><span class="sxs-lookup"><span data-stu-id="f957a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="f957a-131">応答</span><span class="sxs-lookup"><span data-stu-id="f957a-131">Response</span></span>

<span data-ttu-id="f957a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f957a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f957a-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f957a-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f957a-135">C#</span><span class="sxs-lookup"><span data-stu-id="f957a-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f957a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="f957a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
