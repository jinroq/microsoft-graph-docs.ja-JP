---
title: secureScore リソースの種類
description: テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 89842579457365f7da10509b2b4ade31f55de4f9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629265"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="2fa0a-103">secureScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fa0a-103">secureScore resource type</span></span>

<span data-ttu-id="2fa0a-104">テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="2fa0a-105">既定では、90日間のデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="2fa0a-106">このデータは、新しい**日付**から最も古い日付までの日付で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="2fa0a-107">これにより、$top = n (n は取得するデータの日数) を使用して、応答をページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="2fa0a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa0a-108">Methods</span></span>

| <span data-ttu-id="2fa0a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa0a-109">Method</span></span>   | <span data-ttu-id="2fa0a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2fa0a-110">Return Type</span></span>|<span data-ttu-id="2fa0a-111">説明</span><span class="sxs-lookup"><span data-stu-id="2fa0a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fa0a-112">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="2fa0a-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="2fa0a-113">[secureScores](securescore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0a-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="2fa0a-114">SecureScore オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="2fa0a-115">SecureScore を取得する</span><span class="sxs-lookup"><span data-stu-id="2fa0a-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="2fa0a-116">secureScore</span><span class="sxs-lookup"><span data-stu-id="2fa0a-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="2fa0a-117">SecureScore オブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="2fa0a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa0a-118">Properties</span></span>

|<span data-ttu-id="2fa0a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa0a-119">Property</span></span> |<span data-ttu-id="2fa0a-120">型</span><span class="sxs-lookup"><span data-stu-id="2fa0a-120">Type</span></span> |<span data-ttu-id="2fa0a-121">説明</span><span class="sxs-lookup"><span data-stu-id="2fa0a-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="2fa0a-122">id</span><span class="sxs-lookup"><span data-stu-id="2fa0a-122">id</span></span> |<span data-ttu-id="2fa0a-123">String</span><span class="sxs-lookup"><span data-stu-id="2fa0a-123">String</span></span>|<span data-ttu-id="2fa0a-124">プロバイダーによって生成された GUID/一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="2fa0a-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-125">Read-only.</span></span> <span data-ttu-id="2fa0a-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-126">Required.</span></span>|
|   <span data-ttu-id="2fa0a-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="2fa0a-127">azureTenantId</span></span>   |   <span data-ttu-id="2fa0a-128">String</span><span class="sxs-lookup"><span data-stu-id="2fa0a-128">String</span></span>  |   <span data-ttu-id="2fa0a-129">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="2fa0a-130">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="2fa0a-130">activeUserCount</span></span> |   <span data-ttu-id="2fa0a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa0a-131">Int32</span></span>   |   <span data-ttu-id="2fa0a-132">指定したテナントのアクティブなユーザー数。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="2fa0a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa0a-133">createdDateTime</span></span> |   <span data-ttu-id="2fa0a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa0a-134">DateTimeOffset</span></span>  |   <span data-ttu-id="2fa0a-135">エンティティが作成された日付。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="2fa0a-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="2fa0a-136">currentScore</span></span>    |   <span data-ttu-id="2fa0a-137">2 行分</span><span class="sxs-lookup"><span data-stu-id="2fa0a-137">Double</span></span>  |   <span data-ttu-id="2fa0a-138">指定された日付における現在のテナントのスコア。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="2fa0a-139">enabledServices</span><span class="sxs-lookup"><span data-stu-id="2fa0a-139">enabledServices</span></span> |   <span data-ttu-id="2fa0a-140">String collection</span><span class="sxs-lookup"><span data-stu-id="2fa0a-140">String collection</span></span>   |   <span data-ttu-id="2fa0a-141">テナントの Microsoft 提供のサービス (Exchange online、Skype、Sharepoint など)。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="2fa0a-142">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="2fa0a-142">licensedUserCount</span></span>   |   <span data-ttu-id="2fa0a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa0a-143">Int32</span></span>   |   <span data-ttu-id="2fa0a-144">指定したテナントのライセンスされたユーザーカウント。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="2fa0a-145">maxScore</span><span class="sxs-lookup"><span data-stu-id="2fa0a-145">maxScore</span></span> |  <span data-ttu-id="2fa0a-146">2 行分</span><span class="sxs-lookup"><span data-stu-id="2fa0a-146">Double</span></span>  |   <span data-ttu-id="2fa0a-147">指定した日付の有効なテナントの最大スコア。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="2fa0a-148">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="2fa0a-148">averageComparativeScores</span></span> |  <span data-ttu-id="2fa0a-149">[averageComparativeScore](averagecomparativescore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0a-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="2fa0a-150">範囲内の別のスコープ (たとえば、業種別平均、座席の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="2fa0a-151">controlScores</span><span class="sxs-lookup"><span data-stu-id="2fa0a-151">controlScores</span></span> | <span data-ttu-id="2fa0a-152">[Controlscore](controlscore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0a-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="2fa0a-153">一連のコントロールのテナントスコアを含みます。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="2fa0a-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="2fa0a-154">vendorInformation</span></span> |[<span data-ttu-id="2fa0a-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="2fa0a-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="2fa0a-156">セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore)。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="2fa0a-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2fa0a-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fa0a-158">Relationships</span></span>

<span data-ttu-id="2fa0a-159">なし。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fa0a-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fa0a-160">JSON representation</span></span>

<span data-ttu-id="2fa0a-161">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->