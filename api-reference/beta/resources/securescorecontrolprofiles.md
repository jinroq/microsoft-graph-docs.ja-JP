---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524430"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="6ac91-104">secureScoreControlProfiles リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ac91-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ac91-105">コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="6ac91-106">既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。</span><span class="sxs-lookup"><span data-stu-id="6ac91-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="6ac91-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ac91-107">Methods</span></span>

| <span data-ttu-id="6ac91-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ac91-108">Method</span></span>   | <span data-ttu-id="6ac91-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ac91-109">Return Type</span></span>|<span data-ttu-id="6ac91-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ac91-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ac91-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="6ac91-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="6ac91-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6ac91-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="6ac91-113">プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ac91-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6ac91-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ac91-114">Properties</span></span>

|<span data-ttu-id="6ac91-115">名前</span><span class="sxs-lookup"><span data-stu-id="6ac91-115">Name</span></span> |<span data-ttu-id="6ac91-116">型</span><span class="sxs-lookup"><span data-stu-id="6ac91-116">Type</span></span> |<span data-ttu-id="6ac91-117">説明</span><span class="sxs-lookup"><span data-stu-id="6ac91-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6ac91-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6ac91-118">azureTenantId</span></span>   |   <span data-ttu-id="6ac91-119">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-119">String</span></span>  |   <span data-ttu-id="6ac91-120">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="6ac91-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6ac91-121">controlName</span><span class="sxs-lookup"><span data-stu-id="6ac91-121">controlName</span></span> |   <span data-ttu-id="6ac91-122">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-122">String</span></span>  |   <span data-ttu-id="6ac91-123">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="6ac91-123">Name of the control.</span></span> |
|   <span data-ttu-id="6ac91-124">タイトル</span><span class="sxs-lookup"><span data-stu-id="6ac91-124">title</span></span>   |   <span data-ttu-id="6ac91-125">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-125">String</span></span>  |   <span data-ttu-id="6ac91-126">コントロールのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="6ac91-126">Title of the control.</span></span>   |
| <span data-ttu-id="6ac91-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="6ac91-127">complianceInformation</span></span> | <span data-ttu-id="6ac91-128">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ac91-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="6ac91-129">関連付けられているコンプライアンス情報の収集は、スコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="6ac91-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6ac91-130">controlCategory</span></span> |   <span data-ttu-id="6ac91-131">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-131">String</span></span>  |   <span data-ttu-id="6ac91-132">コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="6ac91-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="6ac91-133">actionType</span><span class="sxs-lookup"><span data-stu-id="6ac91-133">actionType</span></span>  |   <span data-ttu-id="6ac91-134">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-134">String</span></span>  |   <span data-ttu-id="6ac91-135">アクションの種類 (構成、レビュー、動作) を制御します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="6ac91-136">service</span><span class="sxs-lookup"><span data-stu-id="6ac91-136">service</span></span> |   <span data-ttu-id="6ac91-137">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-137">String</span></span>  |   <span data-ttu-id="6ac91-138">(Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。</span><span class="sxs-lookup"><span data-stu-id="6ac91-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="6ac91-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="6ac91-139">maxScore</span></span> |  <span data-ttu-id="6ac91-140">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-140">String</span></span>  |   <span data-ttu-id="6ac91-141">現在では、指定した日付の最大のスコアを取得します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="6ac91-142">階層</span><span class="sxs-lookup"><span data-stu-id="6ac91-142">tier</span></span> |  <span data-ttu-id="6ac91-143">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-143">String</span></span>  |   <span data-ttu-id="6ac91-144">制御層 (コア、防御の深さ、高度な)。</span><span class="sxs-lookup"><span data-stu-id="6ac91-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="6ac91-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="6ac91-145">userImpact</span></span> |    <span data-ttu-id="6ac91-146">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-146">String</span></span>  | <span data-ttu-id="6ac91-147">コントロール (低、中、高) を実装するためのユーザーへの影響。</span><span class="sxs-lookup"><span data-stu-id="6ac91-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="6ac91-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="6ac91-148">implementationCost</span></span> |    <span data-ttu-id="6ac91-149">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-149">String</span></span>  |   <span data-ttu-id="6ac91-150">Implemmentating コントロール (低、中、高) のリソースのコストです。</span><span class="sxs-lookup"><span data-stu-id="6ac91-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="6ac91-151">rank</span><span class="sxs-lookup"><span data-stu-id="6ac91-151">rank</span></span> |  <span data-ttu-id="6ac91-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac91-152">Int32</span></span>   |   <span data-ttu-id="6ac91-153">マイクロソフトのコントロールのレベルを調整します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="6ac91-154">脅威</span><span class="sxs-lookup"><span data-stu-id="6ac91-154">threats</span></span> |   <span data-ttu-id="6ac91-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6ac91-155">String Collection</span></span>   |   <span data-ttu-id="6ac91-156">コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。</span><span class="sxs-lookup"><span data-stu-id="6ac91-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="6ac91-157">非推奨</span><span class="sxs-lookup"><span data-stu-id="6ac91-157">deprecated</span></span> |    <span data-ttu-id="6ac91-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="6ac91-158">Boolean</span></span> |   <span data-ttu-id="6ac91-159">コントロールで減価償却されるかどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="6ac91-160">改善計画</span><span class="sxs-lookup"><span data-stu-id="6ac91-160">remediation</span></span> |   <span data-ttu-id="6ac91-161">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-161">String</span></span>  |   <span data-ttu-id="6ac91-162">どのようなコントロールの説明は、改善に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="6ac91-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="6ac91-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="6ac91-163">remediationImpact</span></span> | <span data-ttu-id="6ac91-164">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-164">String</span></span>  |   <span data-ttu-id="6ac91-165">改善のユーザーへの影響の説明です。</span><span class="sxs-lookup"><span data-stu-id="6ac91-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="6ac91-166">ActionURL</span><span class="sxs-lookup"><span data-stu-id="6ac91-166">actionUrl</span></span> | <span data-ttu-id="6ac91-167">String</span><span class="sxs-lookup"><span data-stu-id="6ac91-167">String</span></span>  |   <span data-ttu-id="6ac91-168">URL は、コントロールが対象になることです。</span><span class="sxs-lookup"><span data-stu-id="6ac91-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="6ac91-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="6ac91-169">controlStateUpdates</span></span> |   <span data-ttu-id="6ac91-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ac91-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="6ac91-171">テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="6ac91-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6ac91-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ac91-172">Relationships</span></span>

<span data-ttu-id="6ac91-173">なし。</span><span class="sxs-lookup"><span data-stu-id="6ac91-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ac91-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ac91-174">JSON representation</span></span>

<span data-ttu-id="6ac91-175">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ac91-175">The following is a JSON representation of the resource.</span></span>

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
