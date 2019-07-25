---
title: List groupLifecyclePolicies
description: グループが属する groupLifecyclePolicy オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b5e08c900f864478b8ab510dea5774136df1a255
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889167"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="3582f-103">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="3582f-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="3582f-104">グループが属する [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="3582f-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="3582f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3582f-105">Permissions</span></span>

<span data-ttu-id="3582f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3582f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3582f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3582f-108">Permission type</span></span>      | <span data-ttu-id="3582f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3582f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3582f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3582f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3582f-111">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3582f-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3582f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3582f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3582f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3582f-113">Not supported.</span></span>    |
|<span data-ttu-id="3582f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3582f-114">Application</span></span> | <span data-ttu-id="3582f-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3582f-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3582f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3582f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3582f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3582f-117">Optional query parameters</span></span>
<span data-ttu-id="3582f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3582f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3582f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3582f-119">Request headers</span></span>
| <span data-ttu-id="3582f-120">名前</span><span class="sxs-lookup"><span data-stu-id="3582f-120">Name</span></span> | <span data-ttu-id="3582f-121">説明</span><span class="sxs-lookup"><span data-stu-id="3582f-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3582f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3582f-122">Authorization</span></span> | <span data-ttu-id="3582f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3582f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3582f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3582f-125">Request body</span></span>
<span data-ttu-id="3582f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3582f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3582f-127">応答</span><span class="sxs-lookup"><span data-stu-id="3582f-127">Response</span></span>
<span data-ttu-id="3582f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3582f-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3582f-129">例</span><span class="sxs-lookup"><span data-stu-id="3582f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3582f-130">要求</span><span class="sxs-lookup"><span data-stu-id="3582f-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3582f-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3582f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3582f-132">C#</span><span class="sxs-lookup"><span data-stu-id="3582f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3582f-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="3582f-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3582f-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="3582f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3582f-135">Java</span><span class="sxs-lookup"><span data-stu-id="3582f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3582f-136">応答</span><span class="sxs-lookup"><span data-stu-id="3582f-136">Response</span></span>

<span data-ttu-id="3582f-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3582f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
