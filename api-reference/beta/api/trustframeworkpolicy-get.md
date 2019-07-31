---
title: TrustFrameworkPolicy の取得
description: この操作では、Azure AD B2C テナントから既存の trustFrameworkPolicy コンテンツを取得します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 39cd3f11644eca36720fccbf60ba81fd5384af6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987867"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="c51be-103">TrustFrameworkPolicy の取得</span><span class="sxs-lookup"><span data-stu-id="c51be-103">Get trustFrameworkPolicy</span></span>

><span data-ttu-id="c51be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c51be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c51be-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c51be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c51be-106">既存の[Trustframeworkpolicy](../resources/trustframeworkpolicy.md)の内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="c51be-106">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c51be-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c51be-107">Permissions</span></span>

<span data-ttu-id="c51be-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c51be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="c51be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c51be-110">Permission type</span></span>      | <span data-ttu-id="c51be-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c51be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c51be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c51be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c51be-113">ポリシー. TrustFramework, Policy. すべて</span><span class="sxs-lookup"><span data-stu-id="c51be-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="c51be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c51be-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c51be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c51be-115">Not supported.</span></span>|
|<span data-ttu-id="c51be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c51be-116">Application</span></span>|<span data-ttu-id="c51be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c51be-117">Not supported.</span></span>|

<span data-ttu-id="c51be-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c51be-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c51be-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c51be-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c51be-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c51be-120">Optional query parameters</span></span>

<span data-ttu-id="c51be-121">このメソッドは、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51be-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c51be-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c51be-122">Request headers</span></span>

|<span data-ttu-id="c51be-123">名前</span><span class="sxs-lookup"><span data-stu-id="c51be-123">Name</span></span>|<span data-ttu-id="c51be-124">説明</span><span class="sxs-lookup"><span data-stu-id="c51be-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c51be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51be-125">Authorization</span></span>|<span data-ttu-id="c51be-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c51be-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51be-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c51be-128">Request body</span></span>

<span data-ttu-id="c51be-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c51be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c51be-130">応答</span><span class="sxs-lookup"><span data-stu-id="c51be-130">Response</span></span>

<span data-ttu-id="c51be-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[TRUSTFRAMEWORKPOLICY](../resources/trustframeworkpolicy.md)の XML 表記を返します。</span><span class="sxs-lookup"><span data-stu-id="c51be-131">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="c51be-132">**注:** 応答コンテンツタイプはになり`application/xml`ます。</span><span class="sxs-lookup"><span data-stu-id="c51be-132">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="c51be-133">例</span><span class="sxs-lookup"><span data-stu-id="c51be-133">Example</span></span>

<span data-ttu-id="c51be-134">次の例では、特定の**Trustframeworkpolicy**を取得します。</span><span class="sxs-lookup"><span data-stu-id="c51be-134">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="c51be-135">要求</span><span class="sxs-lookup"><span data-stu-id="c51be-135">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="c51be-136">応答</span><span class="sxs-lookup"><span data-stu-id="c51be-136">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFramework policy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
