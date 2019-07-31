---
title: secureScoreControlProfile リソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e244576cb014719d454fe37bd8395054efe2e2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965281"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="0a9b9-104">secureScoreControlProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a9b9-104">secureScoreControlProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9b9-105">テナントのセキュリティスコア (コントロールデータごと) を表します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="0a9b9-106">既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="0a9b9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a9b9-107">Methods</span></span>

| <span data-ttu-id="0a9b9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a9b9-108">Method</span></span>   | <span data-ttu-id="0a9b9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a9b9-109">Return Type</span></span>|<span data-ttu-id="0a9b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a9b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a9b9-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="0a9b9-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="0a9b9-112">[secureScoreControlProfile](securescorecontrolprofiles.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b9-112">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="0a9b9-113">SecureScoreControlProfile オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-113">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="0a9b9-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a9b9-114">Properties</span></span>

|<span data-ttu-id="0a9b9-115">名前</span><span class="sxs-lookup"><span data-stu-id="0a9b9-115">Name</span></span> |<span data-ttu-id="0a9b9-116">型</span><span class="sxs-lookup"><span data-stu-id="0a9b9-116">Type</span></span> |<span data-ttu-id="0a9b9-117">説明</span><span class="sxs-lookup"><span data-stu-id="0a9b9-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="0a9b9-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="0a9b9-118">azureTenantId</span></span>   |   <span data-ttu-id="0a9b9-119">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-119">String</span></span>  |   <span data-ttu-id="0a9b9-120">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="0a9b9-121">controlName</span><span class="sxs-lookup"><span data-stu-id="0a9b9-121">controlName</span></span> |   <span data-ttu-id="0a9b9-122">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-122">String</span></span>  |   <span data-ttu-id="0a9b9-123">コントロールの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-123">Name of the control.</span></span> |
|   <span data-ttu-id="0a9b9-124">title</span><span class="sxs-lookup"><span data-stu-id="0a9b9-124">title</span></span>   |   <span data-ttu-id="0a9b9-125">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-125">String</span></span>  |   <span data-ttu-id="0a9b9-126">コントロールのタイトルを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-126">Title of the control.</span></span>   |
| <span data-ttu-id="0a9b9-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="0a9b9-127">complianceInformation</span></span> | <span data-ttu-id="0a9b9-128">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b9-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="0a9b9-129">セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b9-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="0a9b9-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="0a9b9-130">controlCategory</span></span> |   <span data-ttu-id="0a9b9-131">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-131">String</span></span>  |   <span data-ttu-id="0a9b9-132">コントロールアクションカテゴリ (アカウント、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="0a9b9-133">actionType</span><span class="sxs-lookup"><span data-stu-id="0a9b9-133">actionType</span></span>  |   <span data-ttu-id="0a9b9-134">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-134">String</span></span>  |   <span data-ttu-id="0a9b9-135">アクションの種類 (Config、Review、Behavior) を制御します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="0a9b9-136">service</span><span class="sxs-lookup"><span data-stu-id="0a9b9-136">service</span></span> |   <span data-ttu-id="0a9b9-137">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-137">String</span></span>  |   <span data-ttu-id="0a9b9-138">コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="0a9b9-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="0a9b9-139">maxScore</span></span> |  <span data-ttu-id="0a9b9-140">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-140">String</span></span>  |   <span data-ttu-id="0a9b9-141">指定された日付における現在の取得最高スコア。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="0a9b9-142">層</span><span class="sxs-lookup"><span data-stu-id="0a9b9-142">tier</span></span> |  <span data-ttu-id="0a9b9-143">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-143">String</span></span>  |   <span data-ttu-id="0a9b9-144">Control 層 (コア、多層防御、詳細)</span><span class="sxs-lookup"><span data-stu-id="0a9b9-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="0a9b9-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="0a9b9-145">userImpact</span></span> |    <span data-ttu-id="0a9b9-146">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-146">String</span></span>  | <span data-ttu-id="0a9b9-147">制御を実装するユーザーへの影響 (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="0a9b9-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="0a9b9-148">implementationCost</span></span> |    <span data-ttu-id="0a9b9-149">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-149">String</span></span>  |   <span data-ttu-id="0a9b9-150">Implemmentating コントロールのリソースコスト (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="0a9b9-151">rank</span><span class="sxs-lookup"><span data-stu-id="0a9b9-151">rank</span></span> |  <span data-ttu-id="0a9b9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0a9b9-152">Int32</span></span>   |   <span data-ttu-id="0a9b9-153">Microsoft のスタックランキング。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="0a9b9-154">主</span><span class="sxs-lookup"><span data-stu-id="0a9b9-154">threats</span></span> |   <span data-ttu-id="0a9b9-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b9-155">String Collection</span></span>   |   <span data-ttu-id="0a9b9-156">統制によって軽減される脅威のリスト (accountBreach、dataDeletion、Dataexのフィルター、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、スプーフィング)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="0a9b9-157">予定</span><span class="sxs-lookup"><span data-stu-id="0a9b9-157">deprecated</span></span> |    <span data-ttu-id="0a9b9-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a9b9-158">Boolean</span></span> |   <span data-ttu-id="0a9b9-159">コントロールが減価償却されているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="0a9b9-160">修復</span><span class="sxs-lookup"><span data-stu-id="0a9b9-160">remediation</span></span> |   <span data-ttu-id="0a9b9-161">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-161">String</span></span>  |   <span data-ttu-id="0a9b9-162">修復に役立つコントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="0a9b9-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="0a9b9-163">remediationImpact</span></span> | <span data-ttu-id="0a9b9-164">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-164">String</span></span>  |   <span data-ttu-id="0a9b9-165">修復のユーザーへの影響についての説明。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="0a9b9-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="0a9b9-166">actionUrl</span></span> | <span data-ttu-id="0a9b9-167">String</span><span class="sxs-lookup"><span data-stu-id="0a9b9-167">String</span></span>  |   <span data-ttu-id="0a9b9-168">コントロールを actioned できる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="0a9b9-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="0a9b9-169">controlStateUpdates</span></span> | <span data-ttu-id="0a9b9-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b9-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="0a9b9-171">テナントがコントロールをマークした場所を示すフラグ (ignore、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofiles-update.md)をサポート)。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="0a9b9-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="0a9b9-172">vendorInformation</span></span> | [<span data-ttu-id="0a9b9-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0a9b9-173">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="0a9b9-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a9b9-174">Relationships</span></span>

<span data-ttu-id="0a9b9-175">なし。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a9b9-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a9b9-176">JSON representation</span></span>

<span data-ttu-id="0a9b9-177">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b9-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
