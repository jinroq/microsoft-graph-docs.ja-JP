---
title: onPremisesExtensionAttributes リソースの種類
description: User エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。 **OnPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。 クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c97e3bdc8f6c9a0a7558372288bfec4b9fb59593
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035757"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="92d6c-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92d6c-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="92d6c-106">[User](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92d6c-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="92d6c-107">**OnPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="92d6c-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="92d6c-108">クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。</span><span class="sxs-lookup"><span data-stu-id="92d6c-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="92d6c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92d6c-109">Properties</span></span>
| <span data-ttu-id="92d6c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92d6c-110">Property</span></span>     | <span data-ttu-id="92d6c-111">型</span><span class="sxs-lookup"><span data-stu-id="92d6c-111">Type</span></span>   |<span data-ttu-id="92d6c-112">説明</span><span class="sxs-lookup"><span data-stu-id="92d6c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d6c-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="92d6c-113">extensionAttribute1</span></span>|<span data-ttu-id="92d6c-114">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-114">String</span></span>| <span data-ttu-id="92d6c-115">最初のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="92d6c-116">extensionAttribute2</span></span>|<span data-ttu-id="92d6c-117">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-117">String</span></span>| <span data-ttu-id="92d6c-118">2番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="92d6c-119">extensionAttribute3</span></span>|<span data-ttu-id="92d6c-120">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-120">String</span></span>| <span data-ttu-id="92d6c-121">3番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="92d6c-122">extensionAttribute4</span></span>|<span data-ttu-id="92d6c-123">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-123">String</span></span>| <span data-ttu-id="92d6c-124">4番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="92d6c-125">extensionAttribute5</span></span>|<span data-ttu-id="92d6c-126">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-126">String</span></span>| <span data-ttu-id="92d6c-127">5番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="92d6c-128">extensionAttribute6</span></span>|<span data-ttu-id="92d6c-129">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-129">String</span></span>| <span data-ttu-id="92d6c-130">6番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="92d6c-131">extensionAttribute7</span></span>|<span data-ttu-id="92d6c-132">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-132">String</span></span>| <span data-ttu-id="92d6c-133">7番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="92d6c-134">extensionAttribute8</span></span>|<span data-ttu-id="92d6c-135">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-135">String</span></span>| <span data-ttu-id="92d6c-136">8番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="92d6c-137">extensionAttribute9</span></span>|<span data-ttu-id="92d6c-138">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-138">String</span></span>| <span data-ttu-id="92d6c-139">9番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="92d6c-140">extensionAttribute10</span></span>|<span data-ttu-id="92d6c-141">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-141">String</span></span>| <span data-ttu-id="92d6c-142">10番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="92d6c-143">extensionAttribute11</span></span>|<span data-ttu-id="92d6c-144">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-144">String</span></span>| <span data-ttu-id="92d6c-145">11番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="92d6c-146">extensionAttribute12</span></span>|<span data-ttu-id="92d6c-147">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-147">String</span></span>| <span data-ttu-id="92d6c-148">12番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="92d6c-149">extensionAttribute13</span></span>|<span data-ttu-id="92d6c-150">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-150">String</span></span>| <span data-ttu-id="92d6c-151">13番目にカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="92d6c-152">extensionAttribute14</span></span>|<span data-ttu-id="92d6c-153">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-153">String</span></span>| <span data-ttu-id="92d6c-154">14番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="92d6c-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="92d6c-155">extensionAttribute15</span></span>|<span data-ttu-id="92d6c-156">String</span><span class="sxs-lookup"><span data-stu-id="92d6c-156">String</span></span>| <span data-ttu-id="92d6c-157">15番目のカスタマイズ可能な拡張属性。</span><span class="sxs-lookup"><span data-stu-id="92d6c-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92d6c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92d6c-158">JSON representation</span></span>

<span data-ttu-id="92d6c-159">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="92d6c-159">Here is a JSON representation of the resource</span></span>

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
