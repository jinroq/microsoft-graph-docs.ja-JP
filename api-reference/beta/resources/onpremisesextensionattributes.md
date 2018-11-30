---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。 クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。
ms.openlocfilehash: 547fc8ac19059611f5983a8b5ee0bd905f130f79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071969"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="207e0-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="207e0-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="207e0-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="207e0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="207e0-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="207e0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="207e0-108">[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="207e0-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="207e0-109">このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。</span><span class="sxs-lookup"><span data-stu-id="207e0-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="207e0-110">クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。</span><span class="sxs-lookup"><span data-stu-id="207e0-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="207e0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="207e0-111">Properties</span></span>
| <span data-ttu-id="207e0-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="207e0-112">Property</span></span>     | <span data-ttu-id="207e0-113">型</span><span class="sxs-lookup"><span data-stu-id="207e0-113">Type</span></span>   |<span data-ttu-id="207e0-114">説明</span><span class="sxs-lookup"><span data-stu-id="207e0-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="207e0-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="207e0-115">extensionAttribute1</span></span>|<span data-ttu-id="207e0-116">String</span><span class="sxs-lookup"><span data-stu-id="207e0-116">String</span></span>| <span data-ttu-id="207e0-117">最初の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="207e0-118">extensionAttribute2</span></span>|<span data-ttu-id="207e0-119">String</span><span class="sxs-lookup"><span data-stu-id="207e0-119">String</span></span>| <span data-ttu-id="207e0-120">2 つ目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="207e0-121">extensionAttribute3</span></span>|<span data-ttu-id="207e0-122">String</span><span class="sxs-lookup"><span data-stu-id="207e0-122">String</span></span>| <span data-ttu-id="207e0-123">3 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="207e0-124">extensionAttribute4</span></span>|<span data-ttu-id="207e0-125">String</span><span class="sxs-lookup"><span data-stu-id="207e0-125">String</span></span>| <span data-ttu-id="207e0-126">4 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="207e0-127">extensionAttribute5</span></span>|<span data-ttu-id="207e0-128">String</span><span class="sxs-lookup"><span data-stu-id="207e0-128">String</span></span>| <span data-ttu-id="207e0-129">5 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="207e0-130">extensionAttribute6</span></span>|<span data-ttu-id="207e0-131">String</span><span class="sxs-lookup"><span data-stu-id="207e0-131">String</span></span>| <span data-ttu-id="207e0-132">6 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="207e0-133">extensionAttribute7</span></span>|<span data-ttu-id="207e0-134">String</span><span class="sxs-lookup"><span data-stu-id="207e0-134">String</span></span>| <span data-ttu-id="207e0-135">7 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="207e0-136">extensionAttribute8</span></span>|<span data-ttu-id="207e0-137">String</span><span class="sxs-lookup"><span data-stu-id="207e0-137">String</span></span>| <span data-ttu-id="207e0-138">8 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="207e0-139">extensionAttribute9</span></span>|<span data-ttu-id="207e0-140">String</span><span class="sxs-lookup"><span data-stu-id="207e0-140">String</span></span>| <span data-ttu-id="207e0-141">9 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="207e0-142">extensionAttribute10</span></span>|<span data-ttu-id="207e0-143">String</span><span class="sxs-lookup"><span data-stu-id="207e0-143">String</span></span>| <span data-ttu-id="207e0-144">10 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="207e0-145">extensionAttribute11</span></span>|<span data-ttu-id="207e0-146">String</span><span class="sxs-lookup"><span data-stu-id="207e0-146">String</span></span>| <span data-ttu-id="207e0-147">11 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="207e0-148">extensionAttribute12</span></span>|<span data-ttu-id="207e0-149">String</span><span class="sxs-lookup"><span data-stu-id="207e0-149">String</span></span>| <span data-ttu-id="207e0-150">12 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="207e0-151">extensionAttribute13</span></span>|<span data-ttu-id="207e0-152">String</span><span class="sxs-lookup"><span data-stu-id="207e0-152">String</span></span>| <span data-ttu-id="207e0-153">13 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="207e0-154">extensionAttribute14</span></span>|<span data-ttu-id="207e0-155">String</span><span class="sxs-lookup"><span data-stu-id="207e0-155">String</span></span>| <span data-ttu-id="207e0-156">14 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="207e0-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="207e0-157">extensionAttribute15</span></span>|<span data-ttu-id="207e0-158">String</span><span class="sxs-lookup"><span data-stu-id="207e0-158">String</span></span>| <span data-ttu-id="207e0-159">15 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="207e0-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="207e0-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="207e0-160">JSON representation</span></span>

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