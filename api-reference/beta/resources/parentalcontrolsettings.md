---
title: parentalControlSettings リソースの種類
description: アプリケーションの視聴制限の設定を指定します。 これらの設定は、同意の操作性を制御します。
localization_priority: Normal
ms.openlocfilehash: 8a3a768cc9264b6d1a25532455da20d87a5bc4e8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573873"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="890d7-104">parentalControlSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="890d7-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="890d7-105">アプリケーションの視聴制限の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="890d7-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="890d7-106">これらの設定は、同意の操作性を制御します。</span><span class="sxs-lookup"><span data-stu-id="890d7-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="890d7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="890d7-107">Properties</span></span>

| <span data-ttu-id="890d7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="890d7-108">Property</span></span> | <span data-ttu-id="890d7-109">型</span><span class="sxs-lookup"><span data-stu-id="890d7-109">Type</span></span> | <span data-ttu-id="890d7-110">説明</span><span class="sxs-lookup"><span data-stu-id="890d7-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="890d7-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="890d7-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="890d7-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="890d7-112">String collection</span></span>| <span data-ttu-id="890d7-113">[2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。</span><span class="sxs-lookup"><span data-stu-id="890d7-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="890d7-114">アプリケーションへのアクセスは、このリストで指定した国からの未成年者がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="890d7-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="890d7-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="890d7-115">legalAgeGroupRule</span></span>| <span data-ttu-id="890d7-116">String</span><span class="sxs-lookup"><span data-stu-id="890d7-116">String</span></span> | <span data-ttu-id="890d7-117">アプリケーションのユーザーに適用される法律の年齢グループの規則を指定します。</span><span class="sxs-lookup"><span data-stu-id="890d7-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="890d7-118">次の値のいずれかに設定できます。</span><span class="sxs-lookup"><span data-stu-id="890d7-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="890d7-119">値</span><span class="sxs-lookup"><span data-stu-id="890d7-119">Value</span></span></th><th><span data-ttu-id="890d7-120">説明</span><span class="sxs-lookup"><span data-stu-id="890d7-120">Description</span></span></th></tr><tr><td><span data-ttu-id="890d7-121">Allow</span><span class="sxs-lookup"><span data-stu-id="890d7-121">Allow</span></span></td><td><span data-ttu-id="890d7-122">既定値。</span><span class="sxs-lookup"><span data-stu-id="890d7-122">Default.</span></span> <span data-ttu-id="890d7-123">有効な最小値を適用します。</span><span class="sxs-lookup"><span data-stu-id="890d7-123">Enforces the legal minimum.</span></span> <span data-ttu-id="890d7-124">これは、保護者の同意は、欧州連合と韓国で未成年者に必要なことを意味します。</span><span class="sxs-lookup"><span data-stu-id="890d7-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="890d7-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="890d7-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="890d7-126">COPPA の規則に準拠する誕生日の日付を指定するユーザーを強制します。</span><span class="sxs-lookup"><span data-stu-id="890d7-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="890d7-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="890d7-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="890d7-128">下国のマイナー ルールに関係なく、18 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="890d7-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="890d7-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="890d7-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="890d7-130">下国のマイナー ルールに関係なく、14 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="890d7-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="890d7-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="890d7-131">BlockMinors</span></span></td><td><span data-ttu-id="890d7-132">アプリケーションを使用してから未成年をブロックします。</span><span class="sxs-lookup"><span data-stu-id="890d7-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="890d7-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="890d7-133">JSON representation</span></span>
<span data-ttu-id="890d7-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="890d7-134">Here is a JSON representation of the resource.</span></span>
<!-- 
{
    "blockType": "resource",
    "@odata.type":"microsoft.graph.parentalControlSettings"
}
-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
