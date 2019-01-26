---
title: secureScores リソースの種類
description: '上部 = n、n = のデータを取得する日数です。 '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576081"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="1a667-103">secureScores リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a667-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a667-104">テナントとコントロール レベルでのデータのスコアの 1 日あたりのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="1a667-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="1a667-105">既定では、90 日間のデータを保持しています。</span><span class="sxs-lookup"><span data-stu-id="1a667-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="1a667-106">このデータの並べ替えに**createdDateTime**から最初に最新です。</span><span class="sxs-lookup"><span data-stu-id="1a667-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="1a667-107">これにより、ページの応答に $top を使用して = n、n = のデータを取得する日数です。</span><span class="sxs-lookup"><span data-stu-id="1a667-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="1a667-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a667-108">Methods</span></span>

| <span data-ttu-id="1a667-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a667-109">Method</span></span>   | <span data-ttu-id="1a667-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a667-110">Return Type</span></span>|<span data-ttu-id="1a667-111">説明</span><span class="sxs-lookup"><span data-stu-id="1a667-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a667-112">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="1a667-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="1a667-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="1a667-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="1a667-114">プロパティと、secureScores オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a667-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1a667-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a667-115">Properties</span></span>
<span data-ttu-id="1a667-116">テナントのセキュリティのエンティティの型を含むプロパティ (日単位のスナップショット データ) のスコアです。</span><span class="sxs-lookup"><span data-stu-id="1a667-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="1a667-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a667-117">Property</span></span> |<span data-ttu-id="1a667-118">型</span><span class="sxs-lookup"><span data-stu-id="1a667-118">Type</span></span> |<span data-ttu-id="1a667-119">説明</span><span class="sxs-lookup"><span data-stu-id="1a667-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="1a667-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="1a667-120">azureTenantId</span></span>   |   <span data-ttu-id="1a667-121">String</span><span class="sxs-lookup"><span data-stu-id="1a667-121">String</span></span>  |   <span data-ttu-id="1a667-122">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="1a667-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="1a667-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a667-123">createdDateTime</span></span> |   <span data-ttu-id="1a667-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a667-124">DateTimeOffset</span></span>  |   <span data-ttu-id="1a667-125">エンティティが作成されたときの日付。</span><span class="sxs-lookup"><span data-stu-id="1a667-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="1a667-126">id</span><span class="sxs-lookup"><span data-stu-id="1a667-126">id</span></span>  |   <span data-ttu-id="1a667-127">String</span><span class="sxs-lookup"><span data-stu-id="1a667-127">String</span></span>  |   <span data-ttu-id="1a667-128">AzureTenantId_createdDateTime の組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="1a667-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="1a667-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="1a667-129">licensedUserCount</span></span>   |   <span data-ttu-id="1a667-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1a667-130">Int32</span></span>   |   <span data-ttu-id="1a667-131">特定のテナントのユーザー数のライセンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a667-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="1a667-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="1a667-132">activeUserCount</span></span> |   <span data-ttu-id="1a667-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1a667-133">Int32</span></span>   |   <span data-ttu-id="1a667-134">特定のテナントのアクティブなユーザー数です。</span><span class="sxs-lookup"><span data-stu-id="1a667-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="1a667-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="1a667-135">currentScore</span></span>    |   <span data-ttu-id="1a667-136">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1a667-136">Double</span></span>  |   <span data-ttu-id="1a667-137">現在のテナントは、指定した日付のスコアを達成します。</span><span class="sxs-lookup"><span data-stu-id="1a667-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="1a667-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="1a667-138">maxScore</span></span> |  <span data-ttu-id="1a667-139">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1a667-139">Double</span></span>  |   <span data-ttu-id="1a667-140">有効最大スコアを指定した日付のテナントです。</span><span class="sxs-lookup"><span data-stu-id="1a667-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="1a667-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="1a667-141">enabledServices</span></span> |   <span data-ttu-id="1a667-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1a667-142">String collection</span></span>   |   <span data-ttu-id="1a667-143">(たとえば、Exchange のオンライン、Skype、Sharepoint) テナントの Microsoft 提供のサービスです。</span><span class="sxs-lookup"><span data-stu-id="1a667-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="1a667-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="1a667-144">averageComparativeScores</span></span> |  <span data-ttu-id="1a667-145">[averageComparativeScore](averagecomparativescore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a667-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="1a667-146">さまざまなスコープ (業界では、座席で平均での平均値など) およびコントロールの分類 (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のスコープ内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="1a667-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="1a667-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="1a667-147">controlScores</span></span> | <span data-ttu-id="1a667-148">[controlScore](controlscore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a667-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="1a667-149">コントロールのセットのテナントのスコアが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1a667-149">Contains tenant scores for a set of controls.</span></span>   |
|   <span data-ttu-id="1a667-150">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="1a667-150">vendorInformation</span></span> | [<span data-ttu-id="1a667-151">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="1a667-151">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="1a667-152">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="1a667-152">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a667-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a667-153">Relationships</span></span>

<span data-ttu-id="1a667-154">なし。</span><span class="sxs-lookup"><span data-stu-id="1a667-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a667-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a667-155">JSON representation</span></span>

<span data-ttu-id="1a667-156">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a667-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
    "id": "String",
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
