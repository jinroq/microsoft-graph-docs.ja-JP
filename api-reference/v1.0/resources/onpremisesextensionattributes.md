---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。 クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022446"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="3eaa4-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3eaa4-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="3eaa4-106">[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="3eaa4-107">このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="3eaa4-108">クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="3eaa4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eaa4-109">Properties</span></span>
| <span data-ttu-id="3eaa4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eaa4-110">Property</span></span>     | <span data-ttu-id="3eaa4-111">型</span><span class="sxs-lookup"><span data-stu-id="3eaa4-111">Type</span></span>   |<span data-ttu-id="3eaa4-112">説明</span><span class="sxs-lookup"><span data-stu-id="3eaa4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3eaa4-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="3eaa4-113">extensionAttribute1</span></span>|<span data-ttu-id="3eaa4-114">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-114">String</span></span>| <span data-ttu-id="3eaa4-115">最初の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3eaa4-116">extensionAttribute2</span></span>|<span data-ttu-id="3eaa4-117">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-117">String</span></span>| <span data-ttu-id="3eaa4-118">2 つ目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3eaa4-119">extensionAttribute3</span></span>|<span data-ttu-id="3eaa4-120">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-120">String</span></span>| <span data-ttu-id="3eaa4-121">3 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3eaa4-122">extensionAttribute4</span></span>|<span data-ttu-id="3eaa4-123">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-123">String</span></span>| <span data-ttu-id="3eaa4-124">4 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3eaa4-125">extensionAttribute5</span></span>|<span data-ttu-id="3eaa4-126">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-126">String</span></span>| <span data-ttu-id="3eaa4-127">5 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3eaa4-128">extensionAttribute6</span></span>|<span data-ttu-id="3eaa4-129">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-129">String</span></span>| <span data-ttu-id="3eaa4-130">6 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3eaa4-131">extensionAttribute7</span></span>|<span data-ttu-id="3eaa4-132">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-132">String</span></span>| <span data-ttu-id="3eaa4-133">7 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3eaa4-134">extensionAttribute8</span></span>|<span data-ttu-id="3eaa4-135">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-135">String</span></span>| <span data-ttu-id="3eaa4-136">8 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3eaa4-137">extensionAttribute9</span></span>|<span data-ttu-id="3eaa4-138">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-138">String</span></span>| <span data-ttu-id="3eaa4-139">9 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3eaa4-140">extensionAttribute10</span></span>|<span data-ttu-id="3eaa4-141">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-141">String</span></span>| <span data-ttu-id="3eaa4-142">10 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3eaa4-143">extensionAttribute11</span></span>|<span data-ttu-id="3eaa4-144">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-144">String</span></span>| <span data-ttu-id="3eaa4-145">11 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3eaa4-146">extensionAttribute12</span></span>|<span data-ttu-id="3eaa4-147">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-147">String</span></span>| <span data-ttu-id="3eaa4-148">12 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3eaa4-149">extensionAttribute13</span></span>|<span data-ttu-id="3eaa4-150">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-150">String</span></span>| <span data-ttu-id="3eaa4-151">13 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3eaa4-152">extensionAttribute14</span></span>|<span data-ttu-id="3eaa4-153">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-153">String</span></span>| <span data-ttu-id="3eaa4-154">14 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3eaa4-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3eaa4-155">extensionAttribute15</span></span>|<span data-ttu-id="3eaa4-156">String</span><span class="sxs-lookup"><span data-stu-id="3eaa4-156">String</span></span>| <span data-ttu-id="3eaa4-157">15 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="3eaa4-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3eaa4-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3eaa4-158">JSON representation</span></span>

<span data-ttu-id="3eaa4-159">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3eaa4-159">Here is a JSON representation of the resource</span></span>

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