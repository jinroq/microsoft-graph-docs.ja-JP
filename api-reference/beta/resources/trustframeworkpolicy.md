---
title: trustframeworkpolicy
description: Azure AD B2C 信頼フレームワークポリシーは、カスタムポリシーと呼ばれます。 これは、テナントの trustframeworkpolicy オブジェクトで利用可能な操作を示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b822f1b9788d0502c1376ed437593dfb96469ad
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989395"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="6ff41-104">trustframeworkpolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ff41-104">trustFrameworkPolicy resource type</span></span>

> <span data-ttu-id="6ff41-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ff41-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ff41-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ff41-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ff41-107">[Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview)の[信頼フレームワーク](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)ポリシー ([カスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)とも呼ばれます) を表します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-107">Represents a [Trust Framework](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="6ff41-108">信頼フレームワークポリシーにより、ユーザー手順を完全に制御できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6ff41-108">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="6ff41-109">次の場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-109">Use it to:</span></span>

* <span data-ttu-id="6ff41-110">サインアップおよびサインインの完全なエクスペリエンスをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="6ff41-110">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="6ff41-111">任意の SAML、Open id Connect、または OAuth2 id プロバイダーとのフェデレーションを行います。</span><span class="sxs-lookup"><span data-stu-id="6ff41-111">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="6ff41-112">REST エンドポイントを呼び出すことで、他のシステムまたはユーザーのデータストアと統合します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-112">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="6ff41-113">クレームを変換し、証明書利用者アプリケーションに発行されたトークンをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="6ff41-113">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="6ff41-114">詳細については、「 [Azure Active Directory B2C のカスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ff41-114">For more information, see [Custom policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="6ff41-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ff41-115">Methods</span></span>

| <span data-ttu-id="6ff41-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ff41-116">Method</span></span>       | <span data-ttu-id="6ff41-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ff41-117">Return Type</span></span>  |<span data-ttu-id="6ff41-118">説明</span><span class="sxs-lookup"><span data-stu-id="6ff41-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ff41-119">trustframeworkpolicy の作成</span><span class="sxs-lookup"><span data-stu-id="6ff41-119">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="6ff41-120">trustframeworkpolicy</span><span class="sxs-lookup"><span data-stu-id="6ff41-120">trustFrameworkPolicy</span></span>|<span data-ttu-id="6ff41-121">新しい trustframeworkpolicy を作成します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-121">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="6ff41-122">trustframeworkpolicy の取得</span><span class="sxs-lookup"><span data-stu-id="6ff41-122">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="6ff41-123">trustframeworkpolicy</span><span class="sxs-lookup"><span data-stu-id="6ff41-123">trustFrameworkPolicy</span></span>|<span data-ttu-id="6ff41-124">既存の trustframeworkpolicy のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6ff41-124">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="6ff41-125">trustframeworkpolicies を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6ff41-125">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="6ff41-126">trustframeworkpolicy コレクション</span><span class="sxs-lookup"><span data-stu-id="6ff41-126">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="6ff41-127">テナントで構成されているすべての trustframeworkpolicies を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-127">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="6ff41-128">trustframeworkpolicy を更新または作成する</span><span class="sxs-lookup"><span data-stu-id="6ff41-128">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="6ff41-129">なし</span><span class="sxs-lookup"><span data-stu-id="6ff41-129">None</span></span>|<span data-ttu-id="6ff41-130">既存の trustframeworkpolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-130">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="6ff41-131">trustframeworkpolicy の削除</span><span class="sxs-lookup"><span data-stu-id="6ff41-131">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="6ff41-132">なし</span><span class="sxs-lookup"><span data-stu-id="6ff41-132">None</span></span>|<span data-ttu-id="6ff41-133">既存の trustframeworkpolicy を削除します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-133">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ff41-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff41-134">Properties</span></span>

|<span data-ttu-id="6ff41-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff41-135">Property</span></span>|<span data-ttu-id="6ff41-136">型</span><span class="sxs-lookup"><span data-stu-id="6ff41-136">Type</span></span>|<span data-ttu-id="6ff41-137">説明</span><span class="sxs-lookup"><span data-stu-id="6ff41-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ff41-138">id</span><span class="sxs-lookup"><span data-stu-id="6ff41-138">id</span></span>|<span data-ttu-id="6ff41-139">String</span><span class="sxs-lookup"><span data-stu-id="6ff41-139">String</span></span>|<span data-ttu-id="6ff41-140">ポリシーの ID。</span><span class="sxs-lookup"><span data-stu-id="6ff41-140">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ff41-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ff41-141">JSON representation</span></span>

<span data-ttu-id="6ff41-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-142">The following is a JSON representation of the resource.</span></span>

```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a><span data-ttu-id="6ff41-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ff41-143">See also</span></span>

- <span data-ttu-id="6ff41-144">[trustframeworkpolicy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy)スキーマ要素に関する情報を示します。</span><span class="sxs-lookup"><span data-stu-id="6ff41-144">[trustFrameworkPolicy schema](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>  
- [<span data-ttu-id="6ff41-145">trustframeworkpolicy .xsd</span><span class="sxs-lookup"><span data-stu-id="6ff41-145">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
