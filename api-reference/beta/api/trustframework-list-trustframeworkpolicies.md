---
title: TrustFrameworkPolicies を一覧表示する
description: この操作では、Azure AD B2C テナントのすべての trustFrameworkPolicy オブジェクトを一覧表示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67531e5364256e55bb94f88647b1b56a915dce36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867956"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="366bb-103">TrustFrameworkPolicies を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="366bb-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="366bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="366bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="366bb-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="366bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="366bb-106">テナント/ディレクトリの[Trustframeworkpolicies](../resources/trustframeworkpolicy.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="366bb-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="366bb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="366bb-107">Permissions</span></span>

<span data-ttu-id="366bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="366bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="366bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="366bb-110">Permission type</span></span>      | <span data-ttu-id="366bb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="366bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="366bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="366bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="366bb-113">ポリシー. TrustFramework, Policy. すべて</span><span class="sxs-lookup"><span data-stu-id="366bb-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="366bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="366bb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="366bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="366bb-115">Not supported.</span></span>|
|<span data-ttu-id="366bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="366bb-116">Application</span></span>|<span data-ttu-id="366bb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="366bb-117">Not supported.</span></span>|

<span data-ttu-id="366bb-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="366bb-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="366bb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="366bb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="366bb-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="366bb-120">Optional query parameters</span></span>

<span data-ttu-id="366bb-121">このメソッドは、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="366bb-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="366bb-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="366bb-122">Request headers</span></span>

|<span data-ttu-id="366bb-123">名前</span><span class="sxs-lookup"><span data-stu-id="366bb-123">Name</span></span>|<span data-ttu-id="366bb-124">説明</span><span class="sxs-lookup"><span data-stu-id="366bb-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="366bb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="366bb-125">Authorization</span></span>|<span data-ttu-id="366bb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="366bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="366bb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="366bb-128">Request body</span></span>

<span data-ttu-id="366bb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="366bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="366bb-130">応答</span><span class="sxs-lookup"><span data-stu-id="366bb-130">Response</span></span>

<span data-ttu-id="366bb-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文の JSON 表記で[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="366bb-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="366bb-132">例</span><span class="sxs-lookup"><span data-stu-id="366bb-132">Example</span></span>

<span data-ttu-id="366bb-133">次の例では、すべての**Trustframeworkpolicies**を取得します。</span><span class="sxs-lookup"><span data-stu-id="366bb-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="366bb-134">要求</span><span class="sxs-lookup"><span data-stu-id="366bb-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="366bb-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="366bb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="366bb-136">C#</span><span class="sxs-lookup"><span data-stu-id="366bb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="366bb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="366bb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="366bb-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="366bb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="366bb-139">Java</span><span class="sxs-lookup"><span data-stu-id="366bb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="366bb-140">応答</span><span class="sxs-lookup"><span data-stu-id="366bb-140">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
