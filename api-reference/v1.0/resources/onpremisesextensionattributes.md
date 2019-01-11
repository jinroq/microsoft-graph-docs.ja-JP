---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。 クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824746"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="4ca65-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ca65-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="4ca65-106">[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ca65-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="4ca65-107">このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。</span><span class="sxs-lookup"><span data-stu-id="4ca65-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="4ca65-108">クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。</span><span class="sxs-lookup"><span data-stu-id="4ca65-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="4ca65-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ca65-109">Properties</span></span>
| <span data-ttu-id="4ca65-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ca65-110">Property</span></span>     | <span data-ttu-id="4ca65-111">種類</span><span class="sxs-lookup"><span data-stu-id="4ca65-111">Type</span></span>   |<span data-ttu-id="4ca65-112">説明</span><span class="sxs-lookup"><span data-stu-id="4ca65-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca65-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="4ca65-113">extensionAttribute1</span></span>|<span data-ttu-id="4ca65-114">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-114">String</span></span>| <span data-ttu-id="4ca65-115">最初の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="4ca65-116">extensionAttribute2</span></span>|<span data-ttu-id="4ca65-117">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-117">String</span></span>| <span data-ttu-id="4ca65-118">2 つ目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="4ca65-119">extensionAttribute3</span></span>|<span data-ttu-id="4ca65-120">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-120">String</span></span>| <span data-ttu-id="4ca65-121">3 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="4ca65-122">extensionAttribute4</span></span>|<span data-ttu-id="4ca65-123">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-123">String</span></span>| <span data-ttu-id="4ca65-124">4 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="4ca65-125">extensionAttribute5</span></span>|<span data-ttu-id="4ca65-126">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-126">String</span></span>| <span data-ttu-id="4ca65-127">5 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="4ca65-128">extensionAttribute6</span></span>|<span data-ttu-id="4ca65-129">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-129">String</span></span>| <span data-ttu-id="4ca65-130">6 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="4ca65-131">extensionAttribute7</span></span>|<span data-ttu-id="4ca65-132">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-132">String</span></span>| <span data-ttu-id="4ca65-133">7 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="4ca65-134">extensionAttribute8</span></span>|<span data-ttu-id="4ca65-135">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-135">String</span></span>| <span data-ttu-id="4ca65-136">8 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="4ca65-137">extensionAttribute9</span></span>|<span data-ttu-id="4ca65-138">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-138">String</span></span>| <span data-ttu-id="4ca65-139">9 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="4ca65-140">extensionAttribute10</span></span>|<span data-ttu-id="4ca65-141">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-141">String</span></span>| <span data-ttu-id="4ca65-142">10 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="4ca65-143">extensionAttribute11</span></span>|<span data-ttu-id="4ca65-144">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-144">String</span></span>| <span data-ttu-id="4ca65-145">11 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="4ca65-146">extensionAttribute12</span></span>|<span data-ttu-id="4ca65-147">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-147">String</span></span>| <span data-ttu-id="4ca65-148">12 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="4ca65-149">extensionAttribute13</span></span>|<span data-ttu-id="4ca65-150">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-150">String</span></span>| <span data-ttu-id="4ca65-151">13 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="4ca65-152">extensionAttribute14</span></span>|<span data-ttu-id="4ca65-153">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-153">String</span></span>| <span data-ttu-id="4ca65-154">14 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="4ca65-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="4ca65-155">extensionAttribute15</span></span>|<span data-ttu-id="4ca65-156">String</span><span class="sxs-lookup"><span data-stu-id="4ca65-156">String</span></span>| <span data-ttu-id="4ca65-157">15 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="4ca65-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ca65-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ca65-158">JSON representation</span></span>

<span data-ttu-id="4ca65-159">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4ca65-159">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
