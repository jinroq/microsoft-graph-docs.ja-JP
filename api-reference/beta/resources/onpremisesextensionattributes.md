---
title: onPremisesExtensionAttributes リソースの種類
description: User エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。 **OnPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。 クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbcb3d548a99d33e05768c765ab7a7e06981acc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966403"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="fc233-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc233-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc233-106">[User](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc233-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="fc233-107">**OnPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="fc233-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="fc233-108">クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。</span><span class="sxs-lookup"><span data-stu-id="fc233-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="fc233-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc233-109">Properties</span></span>
| <span data-ttu-id="fc233-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc233-110">Property</span></span>     | <span data-ttu-id="fc233-111">型</span><span class="sxs-lookup"><span data-stu-id="fc233-111">Type</span></span>   |<span data-ttu-id="fc233-112">説明</span><span class="sxs-lookup"><span data-stu-id="fc233-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc233-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="fc233-113">extensionAttribute1</span></span>|<span data-ttu-id="fc233-114">String</span><span class="sxs-lookup"><span data-stu-id="fc233-114">String</span></span>| <span data-ttu-id="fc233-115">最初のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="fc233-116">extensionAttribute2</span></span>|<span data-ttu-id="fc233-117">String</span><span class="sxs-lookup"><span data-stu-id="fc233-117">String</span></span>| <span data-ttu-id="fc233-118">2番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="fc233-119">extensionAttribute3</span></span>|<span data-ttu-id="fc233-120">String</span><span class="sxs-lookup"><span data-stu-id="fc233-120">String</span></span>| <span data-ttu-id="fc233-121">3番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="fc233-122">extensionAttribute4</span></span>|<span data-ttu-id="fc233-123">String</span><span class="sxs-lookup"><span data-stu-id="fc233-123">String</span></span>| <span data-ttu-id="fc233-124">4番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="fc233-125">extensionAttribute5</span></span>|<span data-ttu-id="fc233-126">String</span><span class="sxs-lookup"><span data-stu-id="fc233-126">String</span></span>| <span data-ttu-id="fc233-127">5番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="fc233-128">extensionAttribute6</span></span>|<span data-ttu-id="fc233-129">String</span><span class="sxs-lookup"><span data-stu-id="fc233-129">String</span></span>| <span data-ttu-id="fc233-130">6番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="fc233-131">extensionAttribute7</span></span>|<span data-ttu-id="fc233-132">String</span><span class="sxs-lookup"><span data-stu-id="fc233-132">String</span></span>| <span data-ttu-id="fc233-133">7番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="fc233-134">extensionAttribute8</span></span>|<span data-ttu-id="fc233-135">String</span><span class="sxs-lookup"><span data-stu-id="fc233-135">String</span></span>| <span data-ttu-id="fc233-136">8番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="fc233-137">extensionAttribute9</span></span>|<span data-ttu-id="fc233-138">String</span><span class="sxs-lookup"><span data-stu-id="fc233-138">String</span></span>| <span data-ttu-id="fc233-139">9番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="fc233-140">extensionAttribute10</span></span>|<span data-ttu-id="fc233-141">String</span><span class="sxs-lookup"><span data-stu-id="fc233-141">String</span></span>| <span data-ttu-id="fc233-142">10番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="fc233-143">extensionAttribute11</span></span>|<span data-ttu-id="fc233-144">String</span><span class="sxs-lookup"><span data-stu-id="fc233-144">String</span></span>| <span data-ttu-id="fc233-145">11番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="fc233-146">extensionAttribute12</span></span>|<span data-ttu-id="fc233-147">String</span><span class="sxs-lookup"><span data-stu-id="fc233-147">String</span></span>| <span data-ttu-id="fc233-148">12番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="fc233-149">extensionAttribute13</span></span>|<span data-ttu-id="fc233-150">String</span><span class="sxs-lookup"><span data-stu-id="fc233-150">String</span></span>| <span data-ttu-id="fc233-151">13番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="fc233-152">extensionAttribute14</span></span>|<span data-ttu-id="fc233-153">String</span><span class="sxs-lookup"><span data-stu-id="fc233-153">String</span></span>| <span data-ttu-id="fc233-154">14番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fc233-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="fc233-155">extensionAttribute15</span></span>|<span data-ttu-id="fc233-156">String</span><span class="sxs-lookup"><span data-stu-id="fc233-156">String</span></span>| <span data-ttu-id="fc233-157">15番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="fc233-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc233-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc233-158">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
