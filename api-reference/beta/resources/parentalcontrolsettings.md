---
title: parentalControlSettings リソースの種類
description: アプリケーションの視聴制限の設定を指定します。 これらの設定は、同意の操作性を制御します。
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528404"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="e5a15-104">parentalControlSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5a15-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5a15-105">アプリケーションの視聴制限の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="e5a15-106">これらの設定は、同意の操作性を制御します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="e5a15-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5a15-107">Properties</span></span>

| <span data-ttu-id="e5a15-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5a15-108">Property</span></span> | <span data-ttu-id="e5a15-109">型</span><span class="sxs-lookup"><span data-stu-id="e5a15-109">Type</span></span> | <span data-ttu-id="e5a15-110">サポートのメモ</span><span class="sxs-lookup"><span data-stu-id="e5a15-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="e5a15-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="e5a15-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="e5a15-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a15-112">String collection</span></span>| <span data-ttu-id="e5a15-113">[2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="e5a15-114">アプリケーションへのアクセスは、このリストで指定した国からの未成年者がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="e5a15-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="e5a15-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="e5a15-115">legalAgeGroupRule</span></span>| <span data-ttu-id="e5a15-116">String</span><span class="sxs-lookup"><span data-stu-id="e5a15-116">String</span></span> | <span data-ttu-id="e5a15-117">アプリケーションのユーザーに適用される法律の年齢グループの規則を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="e5a15-118">次の値のいずれかに設定できます。</span><span class="sxs-lookup"><span data-stu-id="e5a15-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="e5a15-119">値</span><span class="sxs-lookup"><span data-stu-id="e5a15-119">Value</span></span></th><th><span data-ttu-id="e5a15-120">説明</span><span class="sxs-lookup"><span data-stu-id="e5a15-120">Description</span></span></th></tr><tr><td><span data-ttu-id="e5a15-121">Allow</span><span class="sxs-lookup"><span data-stu-id="e5a15-121">Allow</span></span></td><td><span data-ttu-id="e5a15-122">既定値。</span><span class="sxs-lookup"><span data-stu-id="e5a15-122">Default.</span></span> <span data-ttu-id="e5a15-123">有効な最小値を適用します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-123">Enforces the legal minimum.</span></span> <span data-ttu-id="e5a15-124">これは、保護者の同意は、欧州連合と韓国で未成年者に必要なことを意味します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="e5a15-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="e5a15-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="e5a15-126">COPPA の規則に準拠する誕生日の日付を指定するユーザーを強制します。</span><span class="sxs-lookup"><span data-stu-id="e5a15-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="e5a15-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="e5a15-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="e5a15-128">下国のマイナー ルールに関係なく、18 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5a15-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e5a15-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="e5a15-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="e5a15-130">下国のマイナー ルールに関係なく、14 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5a15-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e5a15-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="e5a15-131">BlockMinors</span></span></td><td><span data-ttu-id="e5a15-132">アプリケーションを使用してから未成年をブロックします。</span><span class="sxs-lookup"><span data-stu-id="e5a15-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="e5a15-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5a15-133">JSON representation</span></span>
<span data-ttu-id="e5a15-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5a15-134">Here is a JSON representation of the resource.</span></span>

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
