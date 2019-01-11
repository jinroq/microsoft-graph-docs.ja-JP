---
title: secureScores リソースの種類
description: '上部 = n、n = のデータを取得する日数です。 '
localization_priority: Normal
ms.openlocfilehash: 332a9656d8237bb07d5c7739b666e09539cf984f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828736"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="adde6-103">secureScores リソースの種類</span><span class="sxs-lookup"><span data-stu-id="adde6-103">secureScores resource type</span></span>

> <span data-ttu-id="adde6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="adde6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adde6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adde6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adde6-106">テナントとコントロール レベルでのデータのスコアの 1 日あたりのテナントのセキュリティで保護されたスコアを表します。</span><span class="sxs-lookup"><span data-stu-id="adde6-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="adde6-107">既定では、90 日間のデータを保持しています。</span><span class="sxs-lookup"><span data-stu-id="adde6-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="adde6-108">このデータの並べ替えに**createdDateTime**から最初に最新です。</span><span class="sxs-lookup"><span data-stu-id="adde6-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="adde6-109">これにより、ページの応答に $top を使用して = n、n = のデータを取得する日数です。</span><span class="sxs-lookup"><span data-stu-id="adde6-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="adde6-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="adde6-110">Methods</span></span>

| <span data-ttu-id="adde6-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="adde6-111">Method</span></span>   | <span data-ttu-id="adde6-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="adde6-112">Return Type</span></span>|<span data-ttu-id="adde6-113">説明</span><span class="sxs-lookup"><span data-stu-id="adde6-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adde6-114">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="adde6-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="adde6-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="adde6-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="adde6-116">プロパティと、secureScores オブジェクトのメタデータを参照してください。</span><span class="sxs-lookup"><span data-stu-id="adde6-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="adde6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="adde6-117">Properties</span></span>
<span data-ttu-id="adde6-118">テナントのセキュリティのエンティティの型を含むプロパティ (日単位のスナップショット データ) のスコアです。</span><span class="sxs-lookup"><span data-stu-id="adde6-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="adde6-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="adde6-119">Property</span></span> |<span data-ttu-id="adde6-120">種類</span><span class="sxs-lookup"><span data-stu-id="adde6-120">Type</span></span> |<span data-ttu-id="adde6-121">説明</span><span class="sxs-lookup"><span data-stu-id="adde6-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="adde6-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="adde6-122">azureTenantId</span></span>   |   <span data-ttu-id="adde6-123">String</span><span class="sxs-lookup"><span data-stu-id="adde6-123">String</span></span>  |   <span data-ttu-id="adde6-124">テナントの GUID の文字列 id。</span><span class="sxs-lookup"><span data-stu-id="adde6-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="adde6-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adde6-125">createdDateTime</span></span> |   <span data-ttu-id="adde6-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adde6-126">DateTimeOffset</span></span>  |   <span data-ttu-id="adde6-127">エンティティが作成されたときの日付。</span><span class="sxs-lookup"><span data-stu-id="adde6-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="adde6-128">id</span><span class="sxs-lookup"><span data-stu-id="adde6-128">id</span></span>  |   <span data-ttu-id="adde6-129">String</span><span class="sxs-lookup"><span data-stu-id="adde6-129">String</span></span>  |   <span data-ttu-id="adde6-130">AzureTenantId_createdDateTime の組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="adde6-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="adde6-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="adde6-131">licensedUserCount</span></span>   |   <span data-ttu-id="adde6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="adde6-132">Int32</span></span>   |   <span data-ttu-id="adde6-133">特定のテナントのユーザー数のライセンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="adde6-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="adde6-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="adde6-134">activeUserCount</span></span> |   <span data-ttu-id="adde6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="adde6-135">Int32</span></span>   |   <span data-ttu-id="adde6-136">特定のテナントのアクティブなユーザー数です。</span><span class="sxs-lookup"><span data-stu-id="adde6-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="adde6-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="adde6-137">currentScore</span></span>    |   <span data-ttu-id="adde6-138">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="adde6-138">Double</span></span>  |   <span data-ttu-id="adde6-139">現在のテナントは、指定した日付のスコアを達成します。</span><span class="sxs-lookup"><span data-stu-id="adde6-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="adde6-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="adde6-140">maxScore</span></span> |  <span data-ttu-id="adde6-141">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="adde6-141">Double</span></span>  |   <span data-ttu-id="adde6-142">有効最大スコアを指定した日付のテナントです。</span><span class="sxs-lookup"><span data-stu-id="adde6-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="adde6-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="adde6-143">enabledServices</span></span> |   <span data-ttu-id="adde6-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="adde6-144">String collection</span></span>   |   <span data-ttu-id="adde6-145">(たとえば、Exchange のオンライン、Skype、Sharepoint) テナントの Microsoft 提供のサービスです。</span><span class="sxs-lookup"><span data-stu-id="adde6-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="adde6-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="adde6-146">averageComparativeScores</span></span> |  <span data-ttu-id="adde6-147">[averageComparativeScore](averagecomparativescore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="adde6-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="adde6-148">さまざまなスコープ (業界では、座席で平均での平均値など) およびコントロールの分類 (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のスコープ内での平均スコアです。</span><span class="sxs-lookup"><span data-stu-id="adde6-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="adde6-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="adde6-149">controlScores</span></span> | <span data-ttu-id="adde6-150">[controlScore](controlscore.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="adde6-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="adde6-151">コントロールのセットのテナントのスコアが含まれています。</span><span class="sxs-lookup"><span data-stu-id="adde6-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="adde6-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="adde6-152">Relationships</span></span>

<span data-ttu-id="adde6-153">なし。</span><span class="sxs-lookup"><span data-stu-id="adde6-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adde6-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="adde6-154">JSON representation</span></span>

<span data-ttu-id="adde6-155">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="adde6-155">The following is a JSON representation of the resource.</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
