---
title: secureScores リソースの種類
description: 'top = n、n は取得するデータの日数を指定します。 '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549203"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="0d938-103">secureScores リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d938-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d938-104">テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="0d938-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="0d938-105">既定では、90日間のデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="0d938-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="0d938-106">このデータは、新しい**日付**から最も古い日付までの日付で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="0d938-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="0d938-107">これにより、$top = n (n は取得するデータの日数) を使用して、応答をページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="0d938-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="0d938-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d938-108">Methods</span></span>

| <span data-ttu-id="0d938-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d938-109">Method</span></span>   | <span data-ttu-id="0d938-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d938-110">Return Type</span></span>|<span data-ttu-id="0d938-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d938-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d938-112">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="0d938-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="0d938-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="0d938-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="0d938-114">secureScores オブジェクトのプロパティとメタデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0d938-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0d938-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d938-115">Properties</span></span>
<span data-ttu-id="0d938-116">テナントのセキュリティスコアのプロパティを含むエンティティ型 (毎日のスナップショットデータ)。</span><span class="sxs-lookup"><span data-stu-id="0d938-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="0d938-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d938-117">Property</span></span> |<span data-ttu-id="0d938-118">型</span><span class="sxs-lookup"><span data-stu-id="0d938-118">Type</span></span> |<span data-ttu-id="0d938-119">説明</span><span class="sxs-lookup"><span data-stu-id="0d938-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="0d938-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="0d938-120">azureTenantId</span></span>   |   <span data-ttu-id="0d938-121">String</span><span class="sxs-lookup"><span data-stu-id="0d938-121">String</span></span>  |   <span data-ttu-id="0d938-122">テナント ID の GUID 文字列。</span><span class="sxs-lookup"><span data-stu-id="0d938-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="0d938-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d938-123">createdDateTime</span></span> |   <span data-ttu-id="0d938-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d938-124">DateTimeOffset</span></span>  |   <span data-ttu-id="0d938-125">エンティティが作成された日付。</span><span class="sxs-lookup"><span data-stu-id="0d938-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="0d938-126">id</span><span class="sxs-lookup"><span data-stu-id="0d938-126">id</span></span>  |   <span data-ttu-id="0d938-127">String</span><span class="sxs-lookup"><span data-stu-id="0d938-127">String</span></span>  |   <span data-ttu-id="0d938-128">azureTenantId_createdDateTime の組み合わせ。</span><span class="sxs-lookup"><span data-stu-id="0d938-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="0d938-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="0d938-129">licensedUserCount</span></span>   |   <span data-ttu-id="0d938-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0d938-130">Int32</span></span>   |   <span data-ttu-id="0d938-131">指定したテナントのライセンスされたユーザーカウント。</span><span class="sxs-lookup"><span data-stu-id="0d938-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="0d938-132">activeusercount</span><span class="sxs-lookup"><span data-stu-id="0d938-132">activeUserCount</span></span> |   <span data-ttu-id="0d938-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0d938-133">Int32</span></span>   |   <span data-ttu-id="0d938-134">指定したテナントのアクティブなユーザー数。</span><span class="sxs-lookup"><span data-stu-id="0d938-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="0d938-135">currentscore</span><span class="sxs-lookup"><span data-stu-id="0d938-135">currentScore</span></span>    |   <span data-ttu-id="0d938-136">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="0d938-136">Double</span></span>  |   <span data-ttu-id="0d938-137">指定された日付における現在のテナントのスコア。</span><span class="sxs-lookup"><span data-stu-id="0d938-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="0d938-138">maxscore</span><span class="sxs-lookup"><span data-stu-id="0d938-138">maxScore</span></span> |  <span data-ttu-id="0d938-139">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="0d938-139">Double</span></span>  |   <span data-ttu-id="0d938-140">指定した日付の有効なテナントの最大スコア。</span><span class="sxs-lookup"><span data-stu-id="0d938-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="0d938-141">enabledservices</span><span class="sxs-lookup"><span data-stu-id="0d938-141">enabledServices</span></span> |   <span data-ttu-id="0d938-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0d938-142">String collection</span></span>   |   <span data-ttu-id="0d938-143">テナントの Microsoft 提供のサービス (Exchange online、Skype、Sharepoint など)。</span><span class="sxs-lookup"><span data-stu-id="0d938-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="0d938-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="0d938-144">averageComparativeScores</span></span> |  <span data-ttu-id="0d938-145">[averageComparativeScore](averagecomparativescore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d938-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="0d938-146">範囲内の別のスコープ (たとえば、業種別平均、座席の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) の平均スコア。</span><span class="sxs-lookup"><span data-stu-id="0d938-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="0d938-147">controlscores</span><span class="sxs-lookup"><span data-stu-id="0d938-147">controlScores</span></span> | <span data-ttu-id="0d938-148">[controlscore](controlscore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d938-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="0d938-149">一連のコントロールのテナントスコアを含みます。</span><span class="sxs-lookup"><span data-stu-id="0d938-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="0d938-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d938-150">Relationships</span></span>

<span data-ttu-id="0d938-151">なし。</span><span class="sxs-lookup"><span data-stu-id="0d938-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d938-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d938-152">JSON representation</span></span>

<span data-ttu-id="0d938-153">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d938-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
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
