---
title: secureScoreControlProfile リソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 98b335d536ab64000b65756f8c60e0f401f028fd
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537199"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="97473-104">secureScoreControlProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97473-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="97473-105">テナントのセキュリティスコア (コントロールデータごと) を表します。</span><span class="sxs-lookup"><span data-stu-id="97473-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="97473-106">既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="97473-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="97473-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="97473-107">Methods</span></span>

| <span data-ttu-id="97473-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="97473-108">Method</span></span>   | <span data-ttu-id="97473-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="97473-109">Return Type</span></span>|<span data-ttu-id="97473-110">説明</span><span class="sxs-lookup"><span data-stu-id="97473-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97473-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="97473-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="97473-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="97473-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="97473-113">Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="97473-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="97473-114">secureScoreControlProfile の取得</span><span class="sxs-lookup"><span data-stu-id="97473-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="97473-115">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="97473-115">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="97473-116">Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="97473-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="97473-117">Securescorecontrolprofile の更新</span><span class="sxs-lookup"><span data-stu-id="97473-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="97473-118">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="97473-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="97473-119">Securescorecontrolprofile オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="97473-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="97473-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97473-120">Properties</span></span>

|<span data-ttu-id="97473-121">名前</span><span class="sxs-lookup"><span data-stu-id="97473-121">Name</span></span> |<span data-ttu-id="97473-122">型</span><span class="sxs-lookup"><span data-stu-id="97473-122">Type</span></span> |<span data-ttu-id="97473-123">説明</span><span class="sxs-lookup"><span data-stu-id="97473-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="97473-124">id</span><span class="sxs-lookup"><span data-stu-id="97473-124">id</span></span>|<span data-ttu-id="97473-125">String</span><span class="sxs-lookup"><span data-stu-id="97473-125">String</span></span>|<span data-ttu-id="97473-126">プロバイダーによって生成された GUID/一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="97473-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="97473-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97473-127">Read-only.</span></span> <span data-ttu-id="97473-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="97473-128">Required.</span></span>|
|<span data-ttu-id="97473-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="97473-129">azureTenantId</span></span>|<span data-ttu-id="97473-130">String</span><span class="sxs-lookup"><span data-stu-id="97473-130">String</span></span>|<span data-ttu-id="97473-131">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="97473-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="97473-132">actionType</span><span class="sxs-lookup"><span data-stu-id="97473-132">actionType</span></span>|<span data-ttu-id="97473-133">String</span><span class="sxs-lookup"><span data-stu-id="97473-133">String</span></span>|<span data-ttu-id="97473-134">アクションの種類 (Config、Review、Behavior) を制御します。</span><span class="sxs-lookup"><span data-stu-id="97473-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="97473-135">actionUrl</span><span class="sxs-lookup"><span data-stu-id="97473-135">actionUrl</span></span>|<span data-ttu-id="97473-136">String</span><span class="sxs-lookup"><span data-stu-id="97473-136">String</span></span>|<span data-ttu-id="97473-137">コントロールを actioned できる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="97473-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="97473-138">controlCategory</span><span class="sxs-lookup"><span data-stu-id="97473-138">controlCategory</span></span>|<span data-ttu-id="97473-139">String</span><span class="sxs-lookup"><span data-stu-id="97473-139">String</span></span>|<span data-ttu-id="97473-140">コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="97473-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="97473-141">title</span><span class="sxs-lookup"><span data-stu-id="97473-141">title</span></span>|<span data-ttu-id="97473-142">String</span><span class="sxs-lookup"><span data-stu-id="97473-142">String</span></span>|<span data-ttu-id="97473-143">コントロールのタイトルを指定します。</span><span class="sxs-lookup"><span data-stu-id="97473-143">Title of the control.</span></span>|
|<span data-ttu-id="97473-144">予定</span><span class="sxs-lookup"><span data-stu-id="97473-144">deprecated</span></span>|<span data-ttu-id="97473-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="97473-145">Boolean</span></span>|<span data-ttu-id="97473-146">コントロールが減価償却されているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="97473-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="97473-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="97473-147">implementationCost</span></span>|<span data-ttu-id="97473-148">String</span><span class="sxs-lookup"><span data-stu-id="97473-148">String</span></span>|<span data-ttu-id="97473-149">Implemmentating コントロールのリソースコスト (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="97473-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="97473-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97473-150">lastModifiedDateTime</span></span>|<span data-ttu-id="97473-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97473-151">DateTimeOffset</span></span>|<span data-ttu-id="97473-152">コントロールプロファイルエンティティが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="97473-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="97473-153">タイムスタンプの種類は、日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="97473-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="97473-154">maxScore</span><span class="sxs-lookup"><span data-stu-id="97473-154">maxScore</span></span>|<span data-ttu-id="97473-155">2 行分</span><span class="sxs-lookup"><span data-stu-id="97473-155">Double</span></span>|<span data-ttu-id="97473-156">コントロールの最大達成数スコア。</span><span class="sxs-lookup"><span data-stu-id="97473-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="97473-157">rank</span><span class="sxs-lookup"><span data-stu-id="97473-157">rank</span></span>|<span data-ttu-id="97473-158">Int32</span><span class="sxs-lookup"><span data-stu-id="97473-158">Int32</span></span>|<span data-ttu-id="97473-159">Microsoft のスタックランキング。</span><span class="sxs-lookup"><span data-stu-id="97473-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="97473-160">修復</span><span class="sxs-lookup"><span data-stu-id="97473-160">remediation</span></span>|<span data-ttu-id="97473-161">String</span><span class="sxs-lookup"><span data-stu-id="97473-161">String</span></span>|<span data-ttu-id="97473-162">修復に役立つコントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="97473-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="97473-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="97473-163">remediationImpact</span></span>|<span data-ttu-id="97473-164">String</span><span class="sxs-lookup"><span data-stu-id="97473-164">String</span></span>|<span data-ttu-id="97473-165">修復のユーザーへの影響についての説明。</span><span class="sxs-lookup"><span data-stu-id="97473-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="97473-166">service</span><span class="sxs-lookup"><span data-stu-id="97473-166">service</span></span>|<span data-ttu-id="97473-167">String</span><span class="sxs-lookup"><span data-stu-id="97473-167">String</span></span>|<span data-ttu-id="97473-168">コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="97473-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="97473-169">主</span><span class="sxs-lookup"><span data-stu-id="97473-169">threats</span></span>|<span data-ttu-id="97473-170">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="97473-170">String collection</span></span>|<span data-ttu-id="97473-171">統制によって軽減される脅威のリスト (accountBreach、dataDeletion、Dataexフィルター、、</span><span class="sxs-lookup"><span data-stu-id="97473-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="97473-172">elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、スプーフィング)。</span><span class="sxs-lookup"><span data-stu-id="97473-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="97473-173">層</span><span class="sxs-lookup"><span data-stu-id="97473-173">tier</span></span>|<span data-ttu-id="97473-174">String</span><span class="sxs-lookup"><span data-stu-id="97473-174">String</span></span>|<span data-ttu-id="97473-175">Control 層 (コア、多層防御、詳細)</span><span class="sxs-lookup"><span data-stu-id="97473-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="97473-176">userImpact</span><span class="sxs-lookup"><span data-stu-id="97473-176">userImpact</span></span>|<span data-ttu-id="97473-177">String</span><span class="sxs-lookup"><span data-stu-id="97473-177">String</span></span>|<span data-ttu-id="97473-178">制御を実装するユーザーへの影響 (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="97473-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="97473-179">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="97473-179">complianceInformation</span></span>|<span data-ttu-id="97473-180">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="97473-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="97473-181">セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション</span><span class="sxs-lookup"><span data-stu-id="97473-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="97473-182">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="97473-182">controlStateUpdates</span></span>|<span data-ttu-id="97473-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="97473-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="97473-184">テナントがコントロールをマークした場所を示すフラグ (無視、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofile-update.md)をサポート)。</span><span class="sxs-lookup"><span data-stu-id="97473-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="97473-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="97473-185">vendorInformation</span></span>|[<span data-ttu-id="97473-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="97473-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="97473-187">セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore)。</span><span class="sxs-lookup"><span data-stu-id="97473-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="97473-188">必須です。</span><span class="sxs-lookup"><span data-stu-id="97473-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97473-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97473-189">Relationships</span></span>

<span data-ttu-id="97473-190">なし。</span><span class="sxs-lookup"><span data-stu-id="97473-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97473-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97473-191">JSON representation</span></span>

<span data-ttu-id="97473-192">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97473-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
