---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641611"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="d7b5b-104">secureScoreControlProfiles リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7b5b-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b5b-105">コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="d7b5b-106">既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="d7b5b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7b5b-107">Methods</span></span>

| <span data-ttu-id="d7b5b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7b5b-108">Method</span></span>   | <span data-ttu-id="d7b5b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7b5b-109">Return Type</span></span>|<span data-ttu-id="d7b5b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d7b5b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7b5b-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="d7b5b-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="d7b5b-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="d7b5b-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="d7b5b-113">プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d7b5b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b5b-114">Properties</span></span>

|<span data-ttu-id="d7b5b-115">名前</span><span class="sxs-lookup"><span data-stu-id="d7b5b-115">Name</span></span> |<span data-ttu-id="d7b5b-116">型</span><span class="sxs-lookup"><span data-stu-id="d7b5b-116">Type</span></span> |<span data-ttu-id="d7b5b-117">説明</span><span class="sxs-lookup"><span data-stu-id="d7b5b-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="d7b5b-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="d7b5b-118">azureTenantId</span></span>   |   <span data-ttu-id="d7b5b-119">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-119">String</span></span>  |   <span data-ttu-id="d7b5b-120">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="d7b5b-121">controlName</span><span class="sxs-lookup"><span data-stu-id="d7b5b-121">controlName</span></span> |   <span data-ttu-id="d7b5b-122">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-122">String</span></span>  |   <span data-ttu-id="d7b5b-123">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-123">Name of the control.</span></span> |
|   <span data-ttu-id="d7b5b-124">タイトル</span><span class="sxs-lookup"><span data-stu-id="d7b5b-124">title</span></span>   |   <span data-ttu-id="d7b5b-125">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-125">String</span></span>  |   <span data-ttu-id="d7b5b-126">コントロールのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-126">Title of the control.</span></span>   |
| <span data-ttu-id="d7b5b-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="d7b5b-127">complianceInformation</span></span> | <span data-ttu-id="d7b5b-128">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b5b-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="d7b5b-129">関連付けられているコンプライアンス情報の収集は、スコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="d7b5b-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="d7b5b-130">controlCategory</span></span> |   <span data-ttu-id="d7b5b-131">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-131">String</span></span>  |   <span data-ttu-id="d7b5b-132">コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="d7b5b-133">actionType</span><span class="sxs-lookup"><span data-stu-id="d7b5b-133">actionType</span></span>  |   <span data-ttu-id="d7b5b-134">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-134">String</span></span>  |   <span data-ttu-id="d7b5b-135">アクションの種類 (構成、レビュー、動作) を制御します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="d7b5b-136">service</span><span class="sxs-lookup"><span data-stu-id="d7b5b-136">service</span></span> |   <span data-ttu-id="d7b5b-137">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-137">String</span></span>  |   <span data-ttu-id="d7b5b-138">(Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="d7b5b-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="d7b5b-139">maxScore</span></span> |  <span data-ttu-id="d7b5b-140">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-140">String</span></span>  |   <span data-ttu-id="d7b5b-141">現在では、指定した日付の最大のスコアを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="d7b5b-142">層</span><span class="sxs-lookup"><span data-stu-id="d7b5b-142">tier</span></span> |  <span data-ttu-id="d7b5b-143">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-143">String</span></span>  |   <span data-ttu-id="d7b5b-144">制御層 (コア、防御の深さ、高度な)。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="d7b5b-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="d7b5b-145">userImpact</span></span> |    <span data-ttu-id="d7b5b-146">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-146">String</span></span>  | <span data-ttu-id="d7b5b-147">コントロール (低、中、高) を実装するためのユーザーへの影響。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="d7b5b-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="d7b5b-148">implementationCost</span></span> |    <span data-ttu-id="d7b5b-149">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-149">String</span></span>  |   <span data-ttu-id="d7b5b-150">Implemmentating コントロール (低、中、高) のリソースのコストです。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="d7b5b-151">rank</span><span class="sxs-lookup"><span data-stu-id="d7b5b-151">rank</span></span> |  <span data-ttu-id="d7b5b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d7b5b-152">Int32</span></span>   |   <span data-ttu-id="d7b5b-153">マイクロソフトのコントロールのレベルを調整します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="d7b5b-154">脅威</span><span class="sxs-lookup"><span data-stu-id="d7b5b-154">threats</span></span> |   <span data-ttu-id="d7b5b-155">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b5b-155">String Collection</span></span>   |   <span data-ttu-id="d7b5b-156">コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="d7b5b-157">非推奨</span><span class="sxs-lookup"><span data-stu-id="d7b5b-157">deprecated</span></span> |    <span data-ttu-id="d7b5b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7b5b-158">Boolean</span></span> |   <span data-ttu-id="d7b5b-159">コントロールで減価償却されるかどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="d7b5b-160">改善計画</span><span class="sxs-lookup"><span data-stu-id="d7b5b-160">remediation</span></span> |   <span data-ttu-id="d7b5b-161">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-161">String</span></span>  |   <span data-ttu-id="d7b5b-162">どのようなコントロールの説明は、改善に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="d7b5b-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="d7b5b-163">remediationImpact</span></span> | <span data-ttu-id="d7b5b-164">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-164">String</span></span>  |   <span data-ttu-id="d7b5b-165">改善のユーザーへの影響の説明です。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="d7b5b-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="d7b5b-166">actionUrl</span></span> | <span data-ttu-id="d7b5b-167">String</span><span class="sxs-lookup"><span data-stu-id="d7b5b-167">String</span></span>  |   <span data-ttu-id="d7b5b-168">URL は、コントロールが対象になることです。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="d7b5b-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="d7b5b-169">controlStateUpdates</span></span> |   <span data-ttu-id="d7b5b-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b5b-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="d7b5b-171">テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d7b5b-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7b5b-172">Relationships</span></span>

<span data-ttu-id="d7b5b-173">なし。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7b5b-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7b5b-174">JSON representation</span></span>

<span data-ttu-id="d7b5b-175">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7b5b-175">The following is a JSON representation of the resource.</span></span>

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
