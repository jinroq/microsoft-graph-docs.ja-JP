---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576060"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="89840-104">secureScoreControlProfiles リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89840-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89840-105">コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="89840-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="89840-106">既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。</span><span class="sxs-lookup"><span data-stu-id="89840-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="89840-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="89840-107">Methods</span></span>

| <span data-ttu-id="89840-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="89840-108">Method</span></span>   | <span data-ttu-id="89840-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="89840-109">Return Type</span></span>|<span data-ttu-id="89840-110">説明</span><span class="sxs-lookup"><span data-stu-id="89840-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89840-111">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="89840-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="89840-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="89840-112">secureScoreControlProfile</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="89840-113">プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="89840-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="89840-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89840-114">Properties</span></span>

|<span data-ttu-id="89840-115">名前</span><span class="sxs-lookup"><span data-stu-id="89840-115">Name</span></span> |<span data-ttu-id="89840-116">型</span><span class="sxs-lookup"><span data-stu-id="89840-116">Type</span></span> |<span data-ttu-id="89840-117">説明</span><span class="sxs-lookup"><span data-stu-id="89840-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="89840-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="89840-118">azureTenantId</span></span>   |   <span data-ttu-id="89840-119">String</span><span class="sxs-lookup"><span data-stu-id="89840-119">String</span></span>  |   <span data-ttu-id="89840-120">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="89840-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="89840-121">controlName</span><span class="sxs-lookup"><span data-stu-id="89840-121">controlName</span></span> |   <span data-ttu-id="89840-122">String</span><span class="sxs-lookup"><span data-stu-id="89840-122">String</span></span>  |   <span data-ttu-id="89840-123">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="89840-123">Name of the control.</span></span> |
|   <span data-ttu-id="89840-124">タイトル</span><span class="sxs-lookup"><span data-stu-id="89840-124">title</span></span>   |   <span data-ttu-id="89840-125">String</span><span class="sxs-lookup"><span data-stu-id="89840-125">String</span></span>  |   <span data-ttu-id="89840-126">コントロールのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="89840-126">Title of the control.</span></span>   |
|   <span data-ttu-id="89840-127">controlCategory</span><span class="sxs-lookup"><span data-stu-id="89840-127">controlCategory</span></span> |   <span data-ttu-id="89840-128">String</span><span class="sxs-lookup"><span data-stu-id="89840-128">String</span></span>  |   <span data-ttu-id="89840-129">コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="89840-129">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="89840-130">actionType</span><span class="sxs-lookup"><span data-stu-id="89840-130">actionType</span></span>  |   <span data-ttu-id="89840-131">String</span><span class="sxs-lookup"><span data-stu-id="89840-131">String</span></span>  |   <span data-ttu-id="89840-132">アクションの種類 (構成、レビュー、動作) を制御します。</span><span class="sxs-lookup"><span data-stu-id="89840-132">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="89840-133">service</span><span class="sxs-lookup"><span data-stu-id="89840-133">service</span></span> |   <span data-ttu-id="89840-134">String</span><span class="sxs-lookup"><span data-stu-id="89840-134">String</span></span>  |   <span data-ttu-id="89840-135">(Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。</span><span class="sxs-lookup"><span data-stu-id="89840-135">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="89840-136">maxScore</span><span class="sxs-lookup"><span data-stu-id="89840-136">maxScore</span></span> |  <span data-ttu-id="89840-137">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="89840-137">Double</span></span>  |   <span data-ttu-id="89840-138">現在では、指定した日付の最大のスコアを取得します。</span><span class="sxs-lookup"><span data-stu-id="89840-138">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="89840-139">層</span><span class="sxs-lookup"><span data-stu-id="89840-139">tier</span></span> |  <span data-ttu-id="89840-140">String</span><span class="sxs-lookup"><span data-stu-id="89840-140">String</span></span>  |   <span data-ttu-id="89840-141">制御層 (コア、防御の深さ、高度な)。</span><span class="sxs-lookup"><span data-stu-id="89840-141">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="89840-142">userImpact</span><span class="sxs-lookup"><span data-stu-id="89840-142">userImpact</span></span> |    <span data-ttu-id="89840-143">String</span><span class="sxs-lookup"><span data-stu-id="89840-143">String</span></span>  | <span data-ttu-id="89840-144">コントロール (低、中、高) を実装するためのユーザーへの影響。</span><span class="sxs-lookup"><span data-stu-id="89840-144">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="89840-145">implementationCost</span><span class="sxs-lookup"><span data-stu-id="89840-145">implementationCost</span></span> |    <span data-ttu-id="89840-146">String</span><span class="sxs-lookup"><span data-stu-id="89840-146">String</span></span>  |   <span data-ttu-id="89840-147">Implemmentating コントロール (低、中、高) のリソースのコストです。</span><span class="sxs-lookup"><span data-stu-id="89840-147">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="89840-148">rank</span><span class="sxs-lookup"><span data-stu-id="89840-148">rank</span></span> |  <span data-ttu-id="89840-149">Int32</span><span class="sxs-lookup"><span data-stu-id="89840-149">Int32</span></span>   |   <span data-ttu-id="89840-150">マイクロソフトのコントロールのレベルを調整します。</span><span class="sxs-lookup"><span data-stu-id="89840-150">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="89840-151">脅威</span><span class="sxs-lookup"><span data-stu-id="89840-151">threats</span></span> |   <span data-ttu-id="89840-152">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="89840-152">String Collection</span></span>   |   <span data-ttu-id="89840-153">コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。</span><span class="sxs-lookup"><span data-stu-id="89840-153">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="89840-154">非推奨</span><span class="sxs-lookup"><span data-stu-id="89840-154">deprecated</span></span> |    <span data-ttu-id="89840-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="89840-155">Boolean</span></span> |   <span data-ttu-id="89840-156">コントロールで減価償却されるかどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="89840-156">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="89840-157">改善計画</span><span class="sxs-lookup"><span data-stu-id="89840-157">remediation</span></span> |   <span data-ttu-id="89840-158">String</span><span class="sxs-lookup"><span data-stu-id="89840-158">String</span></span>  |   <span data-ttu-id="89840-159">どのようなコントロールの説明は、改善に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="89840-159">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="89840-160">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="89840-160">remediationImpact</span></span> | <span data-ttu-id="89840-161">String</span><span class="sxs-lookup"><span data-stu-id="89840-161">String</span></span>  |   <span data-ttu-id="89840-162">改善のユーザーへの影響の説明です。</span><span class="sxs-lookup"><span data-stu-id="89840-162">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="89840-163">actionUrl</span><span class="sxs-lookup"><span data-stu-id="89840-163">actionUrl</span></span> | <span data-ttu-id="89840-164">String</span><span class="sxs-lookup"><span data-stu-id="89840-164">String</span></span>  |   <span data-ttu-id="89840-165">URL は、コントロールが対象になることです。</span><span class="sxs-lookup"><span data-stu-id="89840-165">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="89840-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89840-166">lastModifiedDateTime</span></span> |  <span data-ttu-id="89840-167">文字列 (DateTimeOffset)</span><span class="sxs-lookup"><span data-stu-id="89840-167">String (DateTimeOffset)</span></span> |   <span data-ttu-id="89840-168">最終更新日</span><span class="sxs-lookup"><span data-stu-id="89840-168">Date last modified</span></span> |
|   <span data-ttu-id="89840-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="89840-169">controlStateUpdates</span></span> |   <span data-ttu-id="89840-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89840-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |  <span data-ttu-id="89840-171">テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="89840-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="89840-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="89840-172">vendorInformation</span></span> | [<span data-ttu-id="89840-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="89840-173">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="89840-174">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="89840-174">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="89840-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="89840-175">Relationships</span></span>

<span data-ttu-id="89840-176">なし。</span><span class="sxs-lookup"><span data-stu-id="89840-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89840-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89840-177">JSON representation</span></span>

<span data-ttu-id="89840-178">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89840-178">The following is a JSON representation of the resource.</span></span>

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
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
