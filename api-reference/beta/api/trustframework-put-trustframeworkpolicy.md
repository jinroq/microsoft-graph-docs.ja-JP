---
title: trustframeworkpolicy の更新
description: 'この操作は、既存の trustframeworkpolicy オブジェクトを更新するか、存在しない場合は作成します。 '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cb40c5a70056990bfa7d00443289bbcd565707d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335088"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="ae953-103">trustframeworkpolicy を更新または作成する</span><span class="sxs-lookup"><span data-stu-id="ae953-103">Update or create trustFrameworkPolicy</span></span>

><span data-ttu-id="ae953-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae953-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae953-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae953-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae953-106">既存の[trustframeworkpolicy](../resources/trustframeworkpolicy.md)を更新するか、存在しない場合は作成します。</span><span class="sxs-lookup"><span data-stu-id="ae953-106">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae953-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae953-107">Permissions</span></span>

<span data-ttu-id="ae953-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae953-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="ae953-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae953-110">Permission type</span></span>      | <span data-ttu-id="ae953-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae953-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae953-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae953-113">ポリシーの場合は、ポリシーによって。</span><span class="sxs-lookup"><span data-stu-id="ae953-113">Policy.ReadWrite.TrustFramework, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="ae953-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae953-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ae953-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae953-115">Not supported.</span></span>|
|<span data-ttu-id="ae953-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae953-116">Application</span></span>|<span data-ttu-id="ae953-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae953-117">Not supported.</span></span>|

<span data-ttu-id="ae953-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae953-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae953-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae953-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="ae953-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae953-120">Request headers</span></span>

|<span data-ttu-id="ae953-121">名前</span><span class="sxs-lookup"><span data-stu-id="ae953-121">Name</span></span>|<span data-ttu-id="ae953-122">説明</span><span class="sxs-lookup"><span data-stu-id="ae953-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ae953-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae953-123">Authorization</span></span>|<span data-ttu-id="ae953-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae953-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae953-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae953-126">Content-Type</span></span>|<span data-ttu-id="ae953-127">アプリケーション/xml。</span><span class="sxs-lookup"><span data-stu-id="ae953-127">application/xml.</span></span> <span data-ttu-id="ae953-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="ae953-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae953-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae953-129">Request body</span></span>

<span data-ttu-id="ae953-130">要求本文で、 [trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトの XML 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae953-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="ae953-131">**注:** コンテンツタイプはで`application/xml`ある必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae953-131">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="ae953-132">応答</span><span class="sxs-lookup"><span data-stu-id="ae953-132">Response</span></span>

<span data-ttu-id="ae953-133">応答は、次のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="ae953-133">The response will be one of the following:</span></span>
- <span data-ttu-id="ae953-134">[trustframeworkpolicy](../resources/trustframeworkpolicy.md)が存在する場合、成功した要求`200 OK`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ae953-134">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="ae953-135">[trustframeworkpolicy](../resources/trustframeworkpolicy.md)が存在しない場合、成功した要求は`201 Created`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ae953-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="ae953-136">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="ae953-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ae953-137">例</span><span class="sxs-lookup"><span data-stu-id="ae953-137">Example</span></span>

<span data-ttu-id="ae953-138">次の例では、 **trustframeworkpolicy**を更新します。</span><span class="sxs-lookup"><span data-stu-id="ae953-138">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="ae953-139">要求</span><span class="sxs-lookup"><span data-stu-id="ae953-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="ae953-140">応答</span><span class="sxs-lookup"><span data-stu-id="ae953-140">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true
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
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
