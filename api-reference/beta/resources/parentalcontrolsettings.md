---
title: parentalcontrolsettings リソースの種類
description: アプリケーションにおける、保護者による制限設定を指定します。 これらの設定は、同意操作を制御します。
localization_priority: Normal
ms.openlocfilehash: 8e62e137b872437626a5c77c114f14c6ad0c5eb2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344994"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="f5146-104">parentalcontrolsettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5146-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5146-105">アプリケーションにおける、保護者による制限設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5146-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="f5146-106">これらの設定は、同意操作を制御します。</span><span class="sxs-lookup"><span data-stu-id="f5146-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="f5146-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5146-107">Properties</span></span>

| <span data-ttu-id="f5146-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5146-108">Property</span></span> | <span data-ttu-id="f5146-109">型</span><span class="sxs-lookup"><span data-stu-id="f5146-109">Type</span></span> | <span data-ttu-id="f5146-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5146-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="f5146-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="f5146-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="f5146-112">String collection</span><span class="sxs-lookup"><span data-stu-id="f5146-112">String collection</span></span>| <span data-ttu-id="f5146-113">[2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5146-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="f5146-114">この一覧で指定された国からの未成年者では、アプリケーションへのアクセスがブロックされます。</span><span class="sxs-lookup"><span data-stu-id="f5146-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="f5146-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="f5146-115">legalAgeGroupRule</span></span>| <span data-ttu-id="f5146-116">String</span><span class="sxs-lookup"><span data-stu-id="f5146-116">String</span></span> | <span data-ttu-id="f5146-117">アプリのユーザーに適用する法的年齢グループルールを指定します。</span><span class="sxs-lookup"><span data-stu-id="f5146-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="f5146-118">以下のいずれかの値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="f5146-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="f5146-119">値</span><span class="sxs-lookup"><span data-stu-id="f5146-119">Value</span></span></th><th><span data-ttu-id="f5146-120">説明</span><span class="sxs-lookup"><span data-stu-id="f5146-120">Description</span></span></th></tr><tr><td><span data-ttu-id="f5146-121">許可</span><span class="sxs-lookup"><span data-stu-id="f5146-121">Allow</span></span></td><td><span data-ttu-id="f5146-122">既定値です。</span><span class="sxs-lookup"><span data-stu-id="f5146-122">Default.</span></span> <span data-ttu-id="f5146-123">リーガルの最小値を強制します。</span><span class="sxs-lookup"><span data-stu-id="f5146-123">Enforces the legal minimum.</span></span> <span data-ttu-id="f5146-124">これは、欧州連合と韓国の未成年者について、キッズセーフティが必要であることを意味します。</span><span class="sxs-lookup"><span data-stu-id="f5146-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="f5146-125">requireconforprivacyservices</span><span class="sxs-lookup"><span data-stu-id="f5146-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="f5146-126">ユーザーが COPPA ルールに準拠する生年月日を指定することを強制します。</span><span class="sxs-lookup"><span data-stu-id="f5146-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="f5146-127">requireconforminor</span><span class="sxs-lookup"><span data-stu-id="f5146-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="f5146-128">国のマイナールールに関係なく、18才以下の年齢に対しては、上位下位の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5146-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f5146-129">requireconforkids</span><span class="sxs-lookup"><span data-stu-id="f5146-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="f5146-130">国のマイナールールに関係なく、14才未満の年齢に対して上位下位の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5146-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f5146-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="f5146-131">BlockMinors</span></span></td><td><span data-ttu-id="f5146-132">未成年者がアプリを使用することをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f5146-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="f5146-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5146-133">JSON representation</span></span>
<span data-ttu-id="f5146-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5146-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
