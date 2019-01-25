---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 onPremisesSyncEnabled ユーザーの場合、このプロパティ セットはオンプレミスの Active Directory でマスター管理され、Azure AD に同期され、読み取り専用となります。 クラウド専用ユーザー (onPremisesSyncEnabled が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518241"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="1c2eb-105">onPremisesExtensionAttributes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c2eb-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c2eb-106">[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="1c2eb-107">onPremisesSyncEnabled ユーザーの場合、このプロパティ セットはオンプレミスの Active Directory でマスター管理され、Azure AD に同期され、読み取り専用となります。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="1c2eb-108">クラウド専用ユーザー (onPremisesSyncEnabled が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="1c2eb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c2eb-109">Properties</span></span>
| <span data-ttu-id="1c2eb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c2eb-110">Property</span></span>     | <span data-ttu-id="1c2eb-111">型</span><span class="sxs-lookup"><span data-stu-id="1c2eb-111">Type</span></span>   |<span data-ttu-id="1c2eb-112">説明</span><span class="sxs-lookup"><span data-stu-id="1c2eb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c2eb-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="1c2eb-113">extensionAttribute1</span></span>|<span data-ttu-id="1c2eb-114">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-114">String</span></span>| <span data-ttu-id="1c2eb-115">最初の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="1c2eb-116">extensionAttribute2</span></span>|<span data-ttu-id="1c2eb-117">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-117">String</span></span>| <span data-ttu-id="1c2eb-118">2 つ目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="1c2eb-119">extensionAttribute3</span></span>|<span data-ttu-id="1c2eb-120">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-120">String</span></span>| <span data-ttu-id="1c2eb-121">3 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="1c2eb-122">extensionAttribute4</span></span>|<span data-ttu-id="1c2eb-123">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-123">String</span></span>| <span data-ttu-id="1c2eb-124">4 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="1c2eb-125">extensionAttribute5</span></span>|<span data-ttu-id="1c2eb-126">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-126">String</span></span>| <span data-ttu-id="1c2eb-127">5 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="1c2eb-128">extensionAttribute6</span></span>|<span data-ttu-id="1c2eb-129">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-129">String</span></span>| <span data-ttu-id="1c2eb-130">6 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="1c2eb-131">extensionAttribute7</span></span>|<span data-ttu-id="1c2eb-132">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-132">String</span></span>| <span data-ttu-id="1c2eb-133">7 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="1c2eb-134">extensionAttribute8</span></span>|<span data-ttu-id="1c2eb-135">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-135">String</span></span>| <span data-ttu-id="1c2eb-136">8 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="1c2eb-137">extensionAttribute9</span></span>|<span data-ttu-id="1c2eb-138">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-138">String</span></span>| <span data-ttu-id="1c2eb-139">9 番目の拡張機能のカスタマイズ可能な属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="1c2eb-140">extensionAttribute10</span></span>|<span data-ttu-id="1c2eb-141">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-141">String</span></span>| <span data-ttu-id="1c2eb-142">10 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="1c2eb-143">extensionAttribute11</span></span>|<span data-ttu-id="1c2eb-144">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-144">String</span></span>| <span data-ttu-id="1c2eb-145">11 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="1c2eb-146">extensionAttribute12</span></span>|<span data-ttu-id="1c2eb-147">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-147">String</span></span>| <span data-ttu-id="1c2eb-148">12 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="1c2eb-149">extensionAttribute13</span></span>|<span data-ttu-id="1c2eb-150">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-150">String</span></span>| <span data-ttu-id="1c2eb-151">13 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="1c2eb-152">extensionAttribute14</span></span>|<span data-ttu-id="1c2eb-153">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-153">String</span></span>| <span data-ttu-id="1c2eb-154">14 番目にカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1c2eb-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="1c2eb-155">extensionAttribute15</span></span>|<span data-ttu-id="1c2eb-156">String</span><span class="sxs-lookup"><span data-stu-id="1c2eb-156">String</span></span>| <span data-ttu-id="1c2eb-157">15 番目のカスタマイズ可能な拡張機能の属性です。</span><span class="sxs-lookup"><span data-stu-id="1c2eb-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c2eb-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c2eb-158">JSON representation</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
