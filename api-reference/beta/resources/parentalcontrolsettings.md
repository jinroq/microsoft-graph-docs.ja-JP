---
title: parentalControlSettings リソースの種類
description: アプリケーションの視聴制限の設定を指定します。 これらの設定は、同意の操作性を制御します。
ms.openlocfilehash: 96f0fa96f9257187e404b61eaca877302d50ccee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067389"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="c3035-104">parentalControlSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3035-104">parentalControlSettings resource type</span></span>

> <span data-ttu-id="c3035-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3035-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3035-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3035-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3035-107">アプリケーションの視聴制限の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3035-107">Specifies parental control settings for an application.</span></span> <span data-ttu-id="c3035-108">これらの設定は、同意の操作性を制御します。</span><span class="sxs-lookup"><span data-stu-id="c3035-108">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="c3035-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3035-109">Properties</span></span>

| <span data-ttu-id="c3035-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3035-110">Property</span></span> | <span data-ttu-id="c3035-111">型</span><span class="sxs-lookup"><span data-stu-id="c3035-111">Type</span></span> | <span data-ttu-id="c3035-112">説明</span><span class="sxs-lookup"><span data-stu-id="c3035-112">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="c3035-113">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="c3035-113">countriesBlockedForMinors</span></span>|<span data-ttu-id="c3035-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c3035-114">String collection</span></span>| <span data-ttu-id="c3035-115">[2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3035-115">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="c3035-116">アプリケーションへのアクセスは、このリストで指定した国からの未成年者がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="c3035-116">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="c3035-117">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="c3035-117">legalAgeGroupRule</span></span>| <span data-ttu-id="c3035-118">String</span><span class="sxs-lookup"><span data-stu-id="c3035-118">String</span></span> | <span data-ttu-id="c3035-119">アプリケーションのユーザーに適用される法律の年齢グループの規則を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3035-119">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="c3035-120">次の値のいずれかに設定できます。</span><span class="sxs-lookup"><span data-stu-id="c3035-120">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="c3035-121">値</span><span class="sxs-lookup"><span data-stu-id="c3035-121">Value</span></span></th><th><span data-ttu-id="c3035-122">説明</span><span class="sxs-lookup"><span data-stu-id="c3035-122">Description</span></span></th></tr><tr><td><span data-ttu-id="c3035-123">Allow</span><span class="sxs-lookup"><span data-stu-id="c3035-123">Allow</span></span></td><td><span data-ttu-id="c3035-124">既定値です。</span><span class="sxs-lookup"><span data-stu-id="c3035-124">Default.</span></span> <span data-ttu-id="c3035-125">有効な最小値を適用します。</span><span class="sxs-lookup"><span data-stu-id="c3035-125">Enforces the legal minimum.</span></span> <span data-ttu-id="c3035-126">これは、保護者の同意は、欧州連合と韓国で未成年者に必要なことを意味します。</span><span class="sxs-lookup"><span data-stu-id="c3035-126">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="c3035-127">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="c3035-127">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="c3035-128">COPPA の規則に準拠する誕生日の日付を指定するユーザーを強制します。</span><span class="sxs-lookup"><span data-stu-id="c3035-128">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="c3035-129">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="c3035-129">RequireConsentForMinors</span></span></td><td><span data-ttu-id="c3035-130">下国のマイナー ルールに関係なく、18 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3035-130">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="c3035-131">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="c3035-131">RequireConsentForKids</span></span></td><td><span data-ttu-id="c3035-132">下国のマイナー ルールに関係なく、14 歳の保護者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3035-132">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="c3035-133">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="c3035-133">BlockMinors</span></span></td><td><span data-ttu-id="c3035-134">アプリケーションを使用してから未成年をブロックします。</span><span class="sxs-lookup"><span data-stu-id="c3035-134">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="c3035-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3035-135">JSON representation</span></span>
<span data-ttu-id="c3035-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3035-136">Here is a JSON representation of the resource.</span></span>

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
