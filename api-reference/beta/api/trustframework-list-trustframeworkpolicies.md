---
title: TrustFrameworkPolicies を一覧表示する
description: この操作では、Azure AD B2C テナントのすべての trustFrameworkPolicy オブジェクトを一覧表示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afdaf352494b0f68f37d88707fad98aa9373969a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637452"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="537e5-103">TrustFrameworkPolicies を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="537e5-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="537e5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="537e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="537e5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="537e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="537e5-106">テナント/ディレクトリの[Trustframeworkpolicies](../resources/trustframeworkpolicy.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="537e5-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="537e5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="537e5-107">Permissions</span></span>

<span data-ttu-id="537e5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="537e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="537e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="537e5-110">Permission type</span></span>      | <span data-ttu-id="537e5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="537e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="537e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="537e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="537e5-113">ポリシー. TrustFramework, Policy. すべて</span><span class="sxs-lookup"><span data-stu-id="537e5-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="537e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="537e5-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="537e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="537e5-115">Not supported.</span></span>|
|<span data-ttu-id="537e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="537e5-116">Application</span></span>|<span data-ttu-id="537e5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="537e5-117">Not supported.</span></span>|

<span data-ttu-id="537e5-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="537e5-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="537e5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="537e5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="537e5-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="537e5-120">Optional query parameters</span></span>

<span data-ttu-id="537e5-121">このメソッドは、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="537e5-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="537e5-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="537e5-122">Request headers</span></span>

|<span data-ttu-id="537e5-123">名前</span><span class="sxs-lookup"><span data-stu-id="537e5-123">Name</span></span>|<span data-ttu-id="537e5-124">説明</span><span class="sxs-lookup"><span data-stu-id="537e5-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="537e5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="537e5-125">Authorization</span></span>|<span data-ttu-id="537e5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="537e5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="537e5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="537e5-128">Request body</span></span>

<span data-ttu-id="537e5-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="537e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="537e5-130">応答</span><span class="sxs-lookup"><span data-stu-id="537e5-130">Response</span></span>

<span data-ttu-id="537e5-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文の JSON 表記で[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="537e5-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="537e5-132">例</span><span class="sxs-lookup"><span data-stu-id="537e5-132">Example</span></span>

<span data-ttu-id="537e5-133">次の例では、すべての**Trustframeworkpolicies**を取得します。</span><span class="sxs-lookup"><span data-stu-id="537e5-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="537e5-134">要求</span><span class="sxs-lookup"><span data-stu-id="537e5-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="537e5-135">応答</span><span class="sxs-lookup"><span data-stu-id="537e5-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "B2C_1A_CustomPolicy2"
        },
        {
            "id": "B2C_1A_CustomPolicy3"
        },
        {
            "id": "B2C_1A_SocialAndLocalAccounts_Base"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="537e5-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="537e5-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="537e5-137">Visual</span><span class="sxs-lookup"><span data-stu-id="537e5-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="537e5-138">Java</span><span class="sxs-lookup"><span data-stu-id="537e5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
