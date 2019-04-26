---
title: trustframeworkpolicy の作成
description: この操作により、Azure AD B2C テナントに新しい trustframeworkpolicy オブジェクトが作成されます。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5b06048859853fbf15b1d82cdee97ac507513fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329817"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="f93ce-103">trustframeworkpolicy の作成</span><span class="sxs-lookup"><span data-stu-id="f93ce-103">Create trustFrameworkPolicy</span></span>

> <span data-ttu-id="f93ce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f93ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f93ce-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f93ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f93ce-106">新しい[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f93ce-106">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f93ce-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f93ce-107">Permissions</span></span>

<span data-ttu-id="f93ce-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f93ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f93ce-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f93ce-110">Permission type</span></span>      | <span data-ttu-id="f93ce-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f93ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f93ce-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f93ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f93ce-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f93ce-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="f93ce-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f93ce-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f93ce-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f93ce-115">Not supported.</span></span>|
|<span data-ttu-id="f93ce-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f93ce-116">Application</span></span>|<span data-ttu-id="f93ce-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f93ce-117">Not supported.</span></span>|

<span data-ttu-id="f93ce-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f93ce-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f93ce-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f93ce-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="f93ce-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f93ce-120">Request headers</span></span>

|<span data-ttu-id="f93ce-121">名前</span><span class="sxs-lookup"><span data-stu-id="f93ce-121">Name</span></span>|<span data-ttu-id="f93ce-122">説明</span><span class="sxs-lookup"><span data-stu-id="f93ce-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f93ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f93ce-123">Authorization</span></span>|<span data-ttu-id="f93ce-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f93ce-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f93ce-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f93ce-126">Content-Type</span></span>|<span data-ttu-id="f93ce-127">アプリケーション/xml。</span><span class="sxs-lookup"><span data-stu-id="f93ce-127">application/xml.</span></span> <span data-ttu-id="f93ce-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="f93ce-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f93ce-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f93ce-129">Request body</span></span>

<span data-ttu-id="f93ce-130">要求本文で、 [trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトの XML 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f93ce-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="f93ce-131">コンテンツ タイプは `application/xml` でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f93ce-131">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="f93ce-132">応答</span><span class="sxs-lookup"><span data-stu-id="f93ce-132">Response</span></span>

<span data-ttu-id="f93ce-133">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f93ce-133">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="f93ce-134">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="f93ce-134">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f93ce-135">例</span><span class="sxs-lookup"><span data-stu-id="f93ce-135">Example</span></span>

<span data-ttu-id="f93ce-136">次の例では、 **trustframeworkpolicy**を作成します。</span><span class="sxs-lookup"><span data-stu-id="f93ce-136">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f93ce-137">要求</span><span class="sxs-lookup"><span data-stu-id="f93ce-137">Request</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "name": "create_trustframeworkpolicy_from_trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="f93ce-138">応答</span><span class="sxs-lookup"><span data-stu-id="f93ce-138">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/xml
Location: /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
