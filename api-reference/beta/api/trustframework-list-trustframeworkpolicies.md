---
title: trustframeworkpolicies を一覧表示する
description: この操作では、Azure AD B2C テナントのすべての trustframeworkpolicy オブジェクトを一覧表示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 873fe9de84ec58ded43141668dd3681409032e56
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989444"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="95c09-103">trustframeworkpolicies を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="95c09-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="95c09-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95c09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95c09-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95c09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95c09-106">テナント/ディレクトリの[trustframeworkpolicies](../resources/trustframeworkpolicy.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="95c09-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="95c09-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95c09-107">Permissions</span></span>

<span data-ttu-id="95c09-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95c09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="95c09-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95c09-110">Permission type</span></span>      | <span data-ttu-id="95c09-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95c09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95c09-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95c09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95c09-113">ポリシー. trustframework, policy. すべて</span><span class="sxs-lookup"><span data-stu-id="95c09-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="95c09-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95c09-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="95c09-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95c09-115">Not supported.</span></span>|
|<span data-ttu-id="95c09-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95c09-116">Application</span></span>|<span data-ttu-id="95c09-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95c09-117">Not supported.</span></span>|

<span data-ttu-id="95c09-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="95c09-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="95c09-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95c09-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95c09-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="95c09-120">Optional query parameters</span></span>

<span data-ttu-id="95c09-121">このメソッドは、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="95c09-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95c09-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95c09-122">Request headers</span></span>

|<span data-ttu-id="95c09-123">名前</span><span class="sxs-lookup"><span data-stu-id="95c09-123">Name</span></span>|<span data-ttu-id="95c09-124">説明</span><span class="sxs-lookup"><span data-stu-id="95c09-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="95c09-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="95c09-125">Authorization</span></span>|<span data-ttu-id="95c09-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95c09-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95c09-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="95c09-128">Request body</span></span>

<span data-ttu-id="95c09-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95c09-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95c09-130">応答</span><span class="sxs-lookup"><span data-stu-id="95c09-130">Response</span></span>

<span data-ttu-id="95c09-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文の JSON 表記で[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="95c09-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95c09-132">例</span><span class="sxs-lookup"><span data-stu-id="95c09-132">Example</span></span>

<span data-ttu-id="95c09-133">次の例では、すべての**trustframeworkpolicies**を取得します。</span><span class="sxs-lookup"><span data-stu-id="95c09-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="95c09-134">要求</span><span class="sxs-lookup"><span data-stu-id="95c09-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get__trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="95c09-135">応答</span><span class="sxs-lookup"><span data-stu-id="95c09-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFramework.policy",
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
  "tocPath": ""
}-->
