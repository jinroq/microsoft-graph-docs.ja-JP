---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380584"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="3fdd1-104">secureScoreControlProfiles リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3fdd1-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="3fdd1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fdd1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fdd1-107">コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="3fdd1-108">既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="3fdd1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3fdd1-109">Methods</span></span>

| <span data-ttu-id="3fdd1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="3fdd1-110">Method</span></span>   | <span data-ttu-id="3fdd1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3fdd1-111">Return Type</span></span>|<span data-ttu-id="3fdd1-112">説明</span><span class="sxs-lookup"><span data-stu-id="3fdd1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3fdd1-113">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="3fdd1-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="3fdd1-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="3fdd1-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="3fdd1-115">プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="3fdd1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fdd1-116">Properties</span></span>

|<span data-ttu-id="3fdd1-117">名前</span><span class="sxs-lookup"><span data-stu-id="3fdd1-117">Name</span></span> |<span data-ttu-id="3fdd1-118">型</span><span class="sxs-lookup"><span data-stu-id="3fdd1-118">Type</span></span> |<span data-ttu-id="3fdd1-119">説明</span><span class="sxs-lookup"><span data-stu-id="3fdd1-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="3fdd1-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="3fdd1-120">azureTenantId</span></span>   |   <span data-ttu-id="3fdd1-121">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-121">String</span></span>  |   <span data-ttu-id="3fdd1-122">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="3fdd1-123">controlName</span><span class="sxs-lookup"><span data-stu-id="3fdd1-123">controlName</span></span> |   <span data-ttu-id="3fdd1-124">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-124">String</span></span>  |   <span data-ttu-id="3fdd1-125">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-125">Name of the control.</span></span> |
|   <span data-ttu-id="3fdd1-126">タイトル</span><span class="sxs-lookup"><span data-stu-id="3fdd1-126">title</span></span>   |   <span data-ttu-id="3fdd1-127">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-127">String</span></span>  |   <span data-ttu-id="3fdd1-128">コントロールのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-128">Title of the control.</span></span>   |
| <span data-ttu-id="3fdd1-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="3fdd1-129">complianceInformation</span></span> | <span data-ttu-id="3fdd1-130">[complianceInformation](complianceinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3fdd1-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="3fdd1-131">関連付けられているコンプライアンス情報の収集は、スコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="3fdd1-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="3fdd1-132">controlCategory</span></span> |   <span data-ttu-id="3fdd1-133">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-133">String</span></span>  |   <span data-ttu-id="3fdd1-134">コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="3fdd1-135">actionType</span><span class="sxs-lookup"><span data-stu-id="3fdd1-135">actionType</span></span>  |   <span data-ttu-id="3fdd1-136">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-136">String</span></span>  |   <span data-ttu-id="3fdd1-137">アクションの種類 (構成、レビュー、動作) を制御します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="3fdd1-138">service</span><span class="sxs-lookup"><span data-stu-id="3fdd1-138">service</span></span> |   <span data-ttu-id="3fdd1-139">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-139">String</span></span>  |   <span data-ttu-id="3fdd1-140">(Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="3fdd1-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="3fdd1-141">maxScore</span></span> |  <span data-ttu-id="3fdd1-142">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-142">String</span></span>  |   <span data-ttu-id="3fdd1-143">現在では、指定した日付の最大のスコアを取得します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="3fdd1-144">層</span><span class="sxs-lookup"><span data-stu-id="3fdd1-144">tier</span></span> |  <span data-ttu-id="3fdd1-145">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-145">String</span></span>  |   <span data-ttu-id="3fdd1-146">制御層 (コア、防御の深さ、高度な)。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="3fdd1-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="3fdd1-147">userImpact</span></span> |    <span data-ttu-id="3fdd1-148">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-148">String</span></span>  | <span data-ttu-id="3fdd1-149">コントロール (低、中、高) を実装するためのユーザーへの影響。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="3fdd1-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="3fdd1-150">implementationCost</span></span> |    <span data-ttu-id="3fdd1-151">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-151">String</span></span>  |   <span data-ttu-id="3fdd1-152">Implemmentating コントロール (低、中、高) のリソースのコストです。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="3fdd1-153">rank</span><span class="sxs-lookup"><span data-stu-id="3fdd1-153">rank</span></span> |  <span data-ttu-id="3fdd1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3fdd1-154">Int32</span></span>   |   <span data-ttu-id="3fdd1-155">マイクロソフトのコントロールのレベルを調整します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="3fdd1-156">脅威</span><span class="sxs-lookup"><span data-stu-id="3fdd1-156">threats</span></span> |   <span data-ttu-id="3fdd1-157">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3fdd1-157">String Collection</span></span>   |   <span data-ttu-id="3fdd1-158">コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="3fdd1-159">非推奨</span><span class="sxs-lookup"><span data-stu-id="3fdd1-159">deprecated</span></span> |    <span data-ttu-id="3fdd1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fdd1-160">Boolean</span></span> |   <span data-ttu-id="3fdd1-161">コントロールで減価償却されるかどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="3fdd1-162">改善計画</span><span class="sxs-lookup"><span data-stu-id="3fdd1-162">remediation</span></span> |   <span data-ttu-id="3fdd1-163">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-163">String</span></span>  |   <span data-ttu-id="3fdd1-164">どのようなコントロールの説明は、改善に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="3fdd1-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="3fdd1-165">remediationImpact</span></span> | <span data-ttu-id="3fdd1-166">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-166">String</span></span>  |   <span data-ttu-id="3fdd1-167">改善のユーザーへの影響の説明です。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="3fdd1-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="3fdd1-168">actionUrl</span></span> | <span data-ttu-id="3fdd1-169">String</span><span class="sxs-lookup"><span data-stu-id="3fdd1-169">String</span></span>  |   <span data-ttu-id="3fdd1-170">URL は、コントロールが対象になることです。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="3fdd1-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="3fdd1-171">controlStateUpdates</span></span> |   <span data-ttu-id="3fdd1-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3fdd1-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="3fdd1-173">テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="3fdd1-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3fdd1-174">Relationships</span></span>

<span data-ttu-id="3fdd1-175">なし。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fdd1-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3fdd1-176">JSON representation</span></span>

<span data-ttu-id="3fdd1-177">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3fdd1-177">The following is a JSON representation of the resource.</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
