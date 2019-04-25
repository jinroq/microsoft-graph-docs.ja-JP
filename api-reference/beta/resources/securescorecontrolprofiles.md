---
title: securescorecontrolprofiles のリソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549175"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="5837b-104">securescorecontrolprofiles のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="5837b-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5837b-105">テナントのセキュリティスコア (コントロールデータごと) を表します。</span><span class="sxs-lookup"><span data-stu-id="5837b-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="5837b-106">既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="5837b-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="5837b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5837b-107">Methods</span></span>

| <span data-ttu-id="5837b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5837b-108">Method</span></span>   | <span data-ttu-id="5837b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5837b-109">Return Type</span></span>|<span data-ttu-id="5837b-110">説明</span><span class="sxs-lookup"><span data-stu-id="5837b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5837b-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="5837b-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="5837b-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="5837b-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="5837b-113">securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5837b-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5837b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5837b-114">Properties</span></span>

|<span data-ttu-id="5837b-115">名前</span><span class="sxs-lookup"><span data-stu-id="5837b-115">Name</span></span> |<span data-ttu-id="5837b-116">型</span><span class="sxs-lookup"><span data-stu-id="5837b-116">Type</span></span> |<span data-ttu-id="5837b-117">説明</span><span class="sxs-lookup"><span data-stu-id="5837b-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="5837b-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="5837b-118">azureTenantId</span></span>   |   <span data-ttu-id="5837b-119">String</span><span class="sxs-lookup"><span data-stu-id="5837b-119">String</span></span>  |   <span data-ttu-id="5837b-120">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="5837b-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="5837b-121">controlName</span><span class="sxs-lookup"><span data-stu-id="5837b-121">controlName</span></span> |   <span data-ttu-id="5837b-122">String</span><span class="sxs-lookup"><span data-stu-id="5837b-122">String</span></span>  |   <span data-ttu-id="5837b-123">コントロールの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="5837b-123">Name of the control.</span></span> |
|   <span data-ttu-id="5837b-124">title</span><span class="sxs-lookup"><span data-stu-id="5837b-124">title</span></span>   |   <span data-ttu-id="5837b-125">String</span><span class="sxs-lookup"><span data-stu-id="5837b-125">String</span></span>  |   <span data-ttu-id="5837b-126">コントロールのタイトルを指定します。</span><span class="sxs-lookup"><span data-stu-id="5837b-126">Title of the control.</span></span>   |
| <span data-ttu-id="5837b-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="5837b-127">complianceInformation</span></span> | <span data-ttu-id="5837b-128">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5837b-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="5837b-129">セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション</span><span class="sxs-lookup"><span data-stu-id="5837b-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="5837b-130">controlcategory</span><span class="sxs-lookup"><span data-stu-id="5837b-130">controlCategory</span></span> |   <span data-ttu-id="5837b-131">String</span><span class="sxs-lookup"><span data-stu-id="5837b-131">String</span></span>  |   <span data-ttu-id="5837b-132">コントロールアクションカテゴリ (アカウント、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="5837b-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="5837b-133">actionType</span><span class="sxs-lookup"><span data-stu-id="5837b-133">actionType</span></span>  |   <span data-ttu-id="5837b-134">String</span><span class="sxs-lookup"><span data-stu-id="5837b-134">String</span></span>  |   <span data-ttu-id="5837b-135">アクションの種類 (Config、Review、Behavior) を制御します。</span><span class="sxs-lookup"><span data-stu-id="5837b-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="5837b-136">service</span><span class="sxs-lookup"><span data-stu-id="5837b-136">service</span></span> |   <span data-ttu-id="5837b-137">String</span><span class="sxs-lookup"><span data-stu-id="5837b-137">String</span></span>  |   <span data-ttu-id="5837b-138">コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="5837b-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="5837b-139">maxscore</span><span class="sxs-lookup"><span data-stu-id="5837b-139">maxScore</span></span> |  <span data-ttu-id="5837b-140">String</span><span class="sxs-lookup"><span data-stu-id="5837b-140">String</span></span>  |   <span data-ttu-id="5837b-141">指定された日付における現在の取得最高スコア。</span><span class="sxs-lookup"><span data-stu-id="5837b-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="5837b-142">層</span><span class="sxs-lookup"><span data-stu-id="5837b-142">tier</span></span> |  <span data-ttu-id="5837b-143">String</span><span class="sxs-lookup"><span data-stu-id="5837b-143">String</span></span>  |   <span data-ttu-id="5837b-144">Control 層 (コア、多層防御、詳細)</span><span class="sxs-lookup"><span data-stu-id="5837b-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="5837b-145">userimpact</span><span class="sxs-lookup"><span data-stu-id="5837b-145">userImpact</span></span> |    <span data-ttu-id="5837b-146">String</span><span class="sxs-lookup"><span data-stu-id="5837b-146">String</span></span>  | <span data-ttu-id="5837b-147">制御を実装するユーザーへの影響 (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="5837b-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="5837b-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="5837b-148">implementationCost</span></span> |    <span data-ttu-id="5837b-149">String</span><span class="sxs-lookup"><span data-stu-id="5837b-149">String</span></span>  |   <span data-ttu-id="5837b-150">implemmentating コントロールのリソースコスト (低、中、高)。</span><span class="sxs-lookup"><span data-stu-id="5837b-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="5837b-151">rank</span><span class="sxs-lookup"><span data-stu-id="5837b-151">rank</span></span> |  <span data-ttu-id="5837b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5837b-152">Int32</span></span>   |   <span data-ttu-id="5837b-153">Microsoft のスタックランキング。</span><span class="sxs-lookup"><span data-stu-id="5837b-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="5837b-154">主</span><span class="sxs-lookup"><span data-stu-id="5837b-154">threats</span></span> |   <span data-ttu-id="5837b-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5837b-155">String Collection</span></span>   |   <span data-ttu-id="5837b-156">統制によって軽減される脅威のリスト (accountbreach、datadeletion、dataexのフィルター、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordcracking、phishingOrWhaling、スプーフィング)。</span><span class="sxs-lookup"><span data-stu-id="5837b-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="5837b-157">予定</span><span class="sxs-lookup"><span data-stu-id="5837b-157">deprecated</span></span> |    <span data-ttu-id="5837b-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="5837b-158">Boolean</span></span> |   <span data-ttu-id="5837b-159">コントロールが減価償却されているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="5837b-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="5837b-160">修復</span><span class="sxs-lookup"><span data-stu-id="5837b-160">remediation</span></span> |   <span data-ttu-id="5837b-161">String</span><span class="sxs-lookup"><span data-stu-id="5837b-161">String</span></span>  |   <span data-ttu-id="5837b-162">修復に役立つコントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="5837b-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="5837b-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="5837b-163">remediationImpact</span></span> | <span data-ttu-id="5837b-164">String</span><span class="sxs-lookup"><span data-stu-id="5837b-164">String</span></span>  |   <span data-ttu-id="5837b-165">修復のユーザーへの影響についての説明。</span><span class="sxs-lookup"><span data-stu-id="5837b-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="5837b-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="5837b-166">actionUrl</span></span> | <span data-ttu-id="5837b-167">String</span><span class="sxs-lookup"><span data-stu-id="5837b-167">String</span></span>  |   <span data-ttu-id="5837b-168">コントロールを actioned できる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="5837b-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="5837b-169">controlstateupdates</span><span class="sxs-lookup"><span data-stu-id="5837b-169">controlStateUpdates</span></span> |   <span data-ttu-id="5837b-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5837b-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="5837b-171">テナントがコントロールをマークした場所を示すフラグ (ignore、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofiles-update.md)をサポート)。</span><span class="sxs-lookup"><span data-stu-id="5837b-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="5837b-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5837b-172">Relationships</span></span>

<span data-ttu-id="5837b-173">なし。</span><span class="sxs-lookup"><span data-stu-id="5837b-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5837b-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5837b-174">JSON representation</span></span>

<span data-ttu-id="5837b-175">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5837b-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
