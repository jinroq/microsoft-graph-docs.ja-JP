---
title: secureScoreControlProfile リソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 7ea9550e7fc6417ac28e32acd1d95cb9178f7360
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629258"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="5aed9-104">secureScoreControlProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5aed9-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="5aed9-105">テナントのセキュリティスコア (コントロールデータごと) を表します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="5aed9-106">既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="5aed9-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="5aed9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aed9-107">Methods</span></span>

| <span data-ttu-id="5aed9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aed9-108">Method</span></span>   | <span data-ttu-id="5aed9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5aed9-109">Return Type</span></span>|<span data-ttu-id="5aed9-110">説明</span><span class="sxs-lookup"><span data-stu-id="5aed9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5aed9-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="5aed9-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="5aed9-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="5aed9-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="5aed9-113">Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5aed9-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="5aed9-114">SecureScoreControlProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="5aed9-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="5aed9-115">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="5aed9-115">securescorecontrolprofile</span></span>](secureScoreControlProfile.md) |<span data-ttu-id="5aed9-116">Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5aed9-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="5aed9-117">Securescorecontrolprofile の更新</span><span class="sxs-lookup"><span data-stu-id="5aed9-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="5aed9-118">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="5aed9-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="5aed9-119">Securescorecontrolprofile オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="5aed9-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5aed9-120">Properties</span></span>

|<span data-ttu-id="5aed9-121">名前</span><span class="sxs-lookup"><span data-stu-id="5aed9-121">Name</span></span> |<span data-ttu-id="5aed9-122">型</span><span class="sxs-lookup"><span data-stu-id="5aed9-122">Type</span></span> |<span data-ttu-id="5aed9-123">説明</span><span class="sxs-lookup"><span data-stu-id="5aed9-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="5aed9-124">id</span><span class="sxs-lookup"><span data-stu-id="5aed9-124">id</span></span>|<span data-ttu-id="5aed9-125">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-125">String</span></span>|<span data-ttu-id="5aed9-126">プロバイダーによって生成された GUID/一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5aed9-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="5aed9-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5aed9-127">Read-only.</span></span> <span data-ttu-id="5aed9-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="5aed9-128">Required.</span></span>|
|<span data-ttu-id="5aed9-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="5aed9-129">azureTenantId</span></span>|<span data-ttu-id="5aed9-130">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-130">String</span></span>|<span data-ttu-id="5aed9-131">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="5aed9-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="5aed9-132">actionType</span><span class="sxs-lookup"><span data-stu-id="5aed9-132">actionType</span></span>|<span data-ttu-id="5aed9-133">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-133">String</span></span>|<span data-ttu-id="5aed9-134">アクションの種類 (Config、Review、Behavior) を制御します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="5aed9-135">actionUrl</span><span class="sxs-lookup"><span data-stu-id="5aed9-135">actionUrl</span></span>|<span data-ttu-id="5aed9-136">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-136">String</span></span>|<span data-ttu-id="5aed9-137">コントロールを actioned できる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="5aed9-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="5aed9-138">controlCategory</span><span class="sxs-lookup"><span data-stu-id="5aed9-138">controlCategory</span></span>|<span data-ttu-id="5aed9-139">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-139">String</span></span>|<span data-ttu-id="5aed9-140">コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="5aed9-141">title</span><span class="sxs-lookup"><span data-stu-id="5aed9-141">title</span></span>|<span data-ttu-id="5aed9-142">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-142">String</span></span>|<span data-ttu-id="5aed9-143">コントロールのタイトルを指定します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-143">Title of the control.</span></span>|
|<span data-ttu-id="5aed9-144">予定</span><span class="sxs-lookup"><span data-stu-id="5aed9-144">deprecated</span></span>|<span data-ttu-id="5aed9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aed9-145">Boolean</span></span>|<span data-ttu-id="5aed9-146">コントロールが減価償却されているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="5aed9-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="5aed9-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="5aed9-147">implementationCost</span></span>|<span data-ttu-id="5aed9-148">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-148">String</span></span>|<span data-ttu-id="5aed9-149">Implemmentating コントロールのリソースコスト (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="5aed9-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5aed9-150">lastModifiedDateTime</span></span>|<span data-ttu-id="5aed9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aed9-151">DateTimeOffset</span></span>|<span data-ttu-id="5aed9-152">コントロールプロファイルエンティティが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="5aed9-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="5aed9-153">タイムスタンプの種類は、日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="5aed9-154">maxScore</span><span class="sxs-lookup"><span data-stu-id="5aed9-154">maxScore</span></span>|<span data-ttu-id="5aed9-155">2 行分</span><span class="sxs-lookup"><span data-stu-id="5aed9-155">Double</span></span>|<span data-ttu-id="5aed9-156">コントロールの最大達成数スコア。</span><span class="sxs-lookup"><span data-stu-id="5aed9-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="5aed9-157">rank</span><span class="sxs-lookup"><span data-stu-id="5aed9-157">rank</span></span>|<span data-ttu-id="5aed9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5aed9-158">Int32</span></span>|<span data-ttu-id="5aed9-159">Microsoft のスタックランキング。</span><span class="sxs-lookup"><span data-stu-id="5aed9-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="5aed9-160">修復</span><span class="sxs-lookup"><span data-stu-id="5aed9-160">remediation</span></span>|<span data-ttu-id="5aed9-161">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-161">String</span></span>|<span data-ttu-id="5aed9-162">修復に役立つコントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="5aed9-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="5aed9-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="5aed9-163">remediationImpact</span></span>|<span data-ttu-id="5aed9-164">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-164">String</span></span>|<span data-ttu-id="5aed9-165">修復のユーザーへの影響についての説明。</span><span class="sxs-lookup"><span data-stu-id="5aed9-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="5aed9-166">service</span><span class="sxs-lookup"><span data-stu-id="5aed9-166">service</span></span>|<span data-ttu-id="5aed9-167">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-167">String</span></span>|<span data-ttu-id="5aed9-168">コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="5aed9-169">主</span><span class="sxs-lookup"><span data-stu-id="5aed9-169">threats</span></span>|<span data-ttu-id="5aed9-170">String collection</span><span class="sxs-lookup"><span data-stu-id="5aed9-170">String collection</span></span>|<span data-ttu-id="5aed9-171">統制によって軽減される脅威のリスト (accountBreach、dataDeletion、Dataexフィルター、、</span><span class="sxs-lookup"><span data-stu-id="5aed9-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="5aed9-172">elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、スプーフィング)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="5aed9-173">層</span><span class="sxs-lookup"><span data-stu-id="5aed9-173">tier</span></span>|<span data-ttu-id="5aed9-174">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-174">String</span></span>|<span data-ttu-id="5aed9-175">Control 層 (コア、多層防御、詳細)</span><span class="sxs-lookup"><span data-stu-id="5aed9-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="5aed9-176">userImpact</span><span class="sxs-lookup"><span data-stu-id="5aed9-176">userImpact</span></span>|<span data-ttu-id="5aed9-177">String</span><span class="sxs-lookup"><span data-stu-id="5aed9-177">String</span></span>|<span data-ttu-id="5aed9-178">制御を実装するユーザーへの影響 (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="5aed9-179">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="5aed9-179">complianceInformation</span></span>|<span data-ttu-id="5aed9-180">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5aed9-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="5aed9-181">セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション</span><span class="sxs-lookup"><span data-stu-id="5aed9-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="5aed9-182">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="5aed9-182">controlStateUpdates</span></span>|<span data-ttu-id="5aed9-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5aed9-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="5aed9-184">テナントがコントロールをマークした場所を示すフラグ (無視、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofile-update.md)をサポート)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="5aed9-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="5aed9-185">vendorInformation</span></span>|[<span data-ttu-id="5aed9-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="5aed9-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="5aed9-187">セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore)。</span><span class="sxs-lookup"><span data-stu-id="5aed9-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="5aed9-188">必須です。</span><span class="sxs-lookup"><span data-stu-id="5aed9-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aed9-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5aed9-189">Relationships</span></span>

<span data-ttu-id="5aed9-190">なし。</span><span class="sxs-lookup"><span data-stu-id="5aed9-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5aed9-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5aed9-191">JSON representation</span></span>

<span data-ttu-id="5aed9-192">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5aed9-192">The following is a JSON representation of the resource.</span></span>

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
