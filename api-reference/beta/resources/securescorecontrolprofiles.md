---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071878"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="ebe60-104">secureScoreControlProfiles リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebe60-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="ebe60-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebe60-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebe60-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebe60-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebe60-107">コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="ebe60-108">既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。</span><span class="sxs-lookup"><span data-stu-id="ebe60-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="ebe60-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebe60-109">Methods</span></span>

| <span data-ttu-id="ebe60-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebe60-110">Method</span></span>   | <span data-ttu-id="ebe60-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ebe60-111">Return Type</span></span>|<span data-ttu-id="ebe60-112">説明</span><span class="sxs-lookup"><span data-stu-id="ebe60-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebe60-113">リスト secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ebe60-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="ebe60-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ebe60-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="ebe60-115">プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebe60-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ebe60-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebe60-116">Properties</span></span>

|<span data-ttu-id="ebe60-117">名前</span><span class="sxs-lookup"><span data-stu-id="ebe60-117">Name</span></span> |<span data-ttu-id="ebe60-118">型</span><span class="sxs-lookup"><span data-stu-id="ebe60-118">Type</span></span> |<span data-ttu-id="ebe60-119">説明</span><span class="sxs-lookup"><span data-stu-id="ebe60-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ebe60-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="ebe60-120">azureTenantId</span></span>   |   <span data-ttu-id="ebe60-121">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-121">String</span></span>  |   <span data-ttu-id="ebe60-122">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="ebe60-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="ebe60-123">controlName</span><span class="sxs-lookup"><span data-stu-id="ebe60-123">controlName</span></span> |   <span data-ttu-id="ebe60-124">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-124">String</span></span>  |   <span data-ttu-id="ebe60-125">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="ebe60-125">Name of the control.</span></span> |
|   <span data-ttu-id="ebe60-126">タイトル</span><span class="sxs-lookup"><span data-stu-id="ebe60-126">title</span></span>   |   <span data-ttu-id="ebe60-127">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-127">String</span></span>  |   <span data-ttu-id="ebe60-128">コントロールのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="ebe60-128">Title of the control.</span></span>   |
|   <span data-ttu-id="ebe60-129">controlCategory</span><span class="sxs-lookup"><span data-stu-id="ebe60-129">controlCategory</span></span> |   <span data-ttu-id="ebe60-130">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-130">String</span></span>  |   <span data-ttu-id="ebe60-131">コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="ebe60-131">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="ebe60-132">actionType</span><span class="sxs-lookup"><span data-stu-id="ebe60-132">actionType</span></span>  |   <span data-ttu-id="ebe60-133">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-133">String</span></span>  |   <span data-ttu-id="ebe60-134">アクションの種類 (構成、レビュー、動作) を制御します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-134">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="ebe60-135">service</span><span class="sxs-lookup"><span data-stu-id="ebe60-135">service</span></span> |   <span data-ttu-id="ebe60-136">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-136">String</span></span>  |   <span data-ttu-id="ebe60-137">(Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。</span><span class="sxs-lookup"><span data-stu-id="ebe60-137">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="ebe60-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="ebe60-138">maxScore</span></span> |  <span data-ttu-id="ebe60-139">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-139">String</span></span>  |   <span data-ttu-id="ebe60-140">現在では、指定した日付の最大のスコアを取得します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-140">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="ebe60-141">層</span><span class="sxs-lookup"><span data-stu-id="ebe60-141">tier</span></span> |  <span data-ttu-id="ebe60-142">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-142">String</span></span>  |   <span data-ttu-id="ebe60-143">制御層 (コア、防御の深さ、高度な)。</span><span class="sxs-lookup"><span data-stu-id="ebe60-143">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="ebe60-144">userImpact</span><span class="sxs-lookup"><span data-stu-id="ebe60-144">userImpact</span></span> |    <span data-ttu-id="ebe60-145">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-145">String</span></span>  | <span data-ttu-id="ebe60-146">コントロール (低、中、高) を実装するためのユーザーへの影響。</span><span class="sxs-lookup"><span data-stu-id="ebe60-146">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="ebe60-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="ebe60-147">implementationCost</span></span> |    <span data-ttu-id="ebe60-148">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-148">String</span></span>  |   <span data-ttu-id="ebe60-149">Implemmentating コントロール (低、中、高) のリソースのコストです。</span><span class="sxs-lookup"><span data-stu-id="ebe60-149">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="ebe60-150">rank</span><span class="sxs-lookup"><span data-stu-id="ebe60-150">rank</span></span> |  <span data-ttu-id="ebe60-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ebe60-151">Int32</span></span>   |   <span data-ttu-id="ebe60-152">マイクロソフトのコントロールのレベルを調整します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-152">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="ebe60-153">脅威</span><span class="sxs-lookup"><span data-stu-id="ebe60-153">threats</span></span> |   <span data-ttu-id="ebe60-154">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ebe60-154">String Collection</span></span>   |   <span data-ttu-id="ebe60-155">コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。</span><span class="sxs-lookup"><span data-stu-id="ebe60-155">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="ebe60-156">非推奨</span><span class="sxs-lookup"><span data-stu-id="ebe60-156">deprecated</span></span> |    <span data-ttu-id="ebe60-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="ebe60-157">Boolean</span></span> |   <span data-ttu-id="ebe60-158">コントロールで減価償却されるかどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-158">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="ebe60-159">改善計画</span><span class="sxs-lookup"><span data-stu-id="ebe60-159">remediation</span></span> |   <span data-ttu-id="ebe60-160">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-160">String</span></span>  |   <span data-ttu-id="ebe60-161">どのようなコントロールの説明は、改善に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ebe60-161">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="ebe60-162">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="ebe60-162">remediationImpact</span></span> | <span data-ttu-id="ebe60-163">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-163">String</span></span>  |   <span data-ttu-id="ebe60-164">改善のユーザーへの影響の説明です。</span><span class="sxs-lookup"><span data-stu-id="ebe60-164">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="ebe60-165">actionUrl</span><span class="sxs-lookup"><span data-stu-id="ebe60-165">actionUrl</span></span> | <span data-ttu-id="ebe60-166">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-166">String</span></span>  |   <span data-ttu-id="ebe60-167">URL は、コントロールが対象になることです。</span><span class="sxs-lookup"><span data-stu-id="ebe60-167">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="ebe60-168">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="ebe60-168">controlStateUpdates</span></span> |   <span data-ttu-id="ebe60-169">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-169">String</span></span>  |   <span data-ttu-id="ebe60-170">テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="ebe60-170">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="ebe60-171">tenantNote</span><span class="sxs-lookup"><span data-stu-id="ebe60-171">tenantNote</span></span> |    <span data-ttu-id="ebe60-172">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-172">String</span></span>  |   <span data-ttu-id="ebe60-173">テナントは、制御用コメント ([更新](../api/securescorecontrolprofiles-update.md)) ごとに設定できます。</span><span class="sxs-lookup"><span data-stu-id="ebe60-173">Tenant can set per control comments (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="ebe60-174">担当者</span><span class="sxs-lookup"><span data-stu-id="ebe60-174">assignedTo</span></span> |    <span data-ttu-id="ebe60-175">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-175">String</span></span>  |   <span data-ttu-id="ebe60-176">テナントは、([更新](../api/securescorecontrolprofiles-update.md)) を個別にコントロールを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="ebe60-176">Tenant can assign the control to a individual (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="ebe60-177">updatedBy</span><span class="sxs-lookup"><span data-stu-id="ebe60-177">updatedBy</span></span> | <span data-ttu-id="ebe60-178">String</span><span class="sxs-lookup"><span data-stu-id="ebe60-178">String</span></span>  |   <span data-ttu-id="ebe60-179">コントロールの状態に変更を行ったユーザーのユーザー プリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="ebe60-179">User principal name of who made changes to a control's state.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ebe60-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebe60-180">Relationships</span></span>

<span data-ttu-id="ebe60-181">なし。</span><span class="sxs-lookup"><span data-stu-id="ebe60-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebe60-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebe60-182">JSON representation</span></span>

<span data-ttu-id="ebe60-183">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebe60-183">The following is a JSON representation of the resource.</span></span>

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
