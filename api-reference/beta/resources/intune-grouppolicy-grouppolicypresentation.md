---
title: groupPolicyPresentation リソースの種類
description: グループポリシー定義の追加オプションを表示するための基本エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d6abbcde241059a15969236b3ab7bcb0825d67d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166879"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="dddc3-103">groupPolicyPresentation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dddc3-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="dddc3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dddc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dddc3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dddc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dddc3-106">グループポリシー定義の追加オプションを表示するための基本エンティティ。</span><span class="sxs-lookup"><span data-stu-id="dddc3-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="dddc3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dddc3-107">Methods</span></span>
|<span data-ttu-id="dddc3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dddc3-108">Method</span></span>|<span data-ttu-id="dddc3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dddc3-109">Return Type</span></span>|<span data-ttu-id="dddc3-110">説明</span><span class="sxs-lookup"><span data-stu-id="dddc3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dddc3-111">groupPolicyPresentation を取得する</span><span class="sxs-lookup"><span data-stu-id="dddc3-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="dddc3-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="dddc3-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="dddc3-113">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dddc3-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="dddc3-114">groupPolicyPresentation の更新</span><span class="sxs-lookup"><span data-stu-id="dddc3-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="dddc3-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="dddc3-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="dddc3-116">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dddc3-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dddc3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dddc3-117">Properties</span></span>
|<span data-ttu-id="dddc3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dddc3-118">Property</span></span>|<span data-ttu-id="dddc3-119">型</span><span class="sxs-lookup"><span data-stu-id="dddc3-119">Type</span></span>|<span data-ttu-id="dddc3-120">説明</span><span class="sxs-lookup"><span data-stu-id="dddc3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddc3-121">label</span><span class="sxs-lookup"><span data-stu-id="dddc3-121">label</span></span>|<span data-ttu-id="dddc3-122">String</span><span class="sxs-lookup"><span data-stu-id="dddc3-122">String</span></span>|<span data-ttu-id="dddc3-123">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="dddc3-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="dddc3-124">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="dddc3-124">The default value is empty.</span></span>|
|<span data-ttu-id="dddc3-125">id</span><span class="sxs-lookup"><span data-stu-id="dddc3-125">id</span></span>|<span data-ttu-id="dddc3-126">String</span><span class="sxs-lookup"><span data-stu-id="dddc3-126">String</span></span>|<span data-ttu-id="dddc3-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dddc3-127">Key of the entity.</span></span>|
|<span data-ttu-id="dddc3-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dddc3-128">lastModifiedDateTime</span></span>|<span data-ttu-id="dddc3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dddc3-129">DateTimeOffset</span></span>|<span data-ttu-id="dddc3-130">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="dddc3-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dddc3-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dddc3-131">Relationships</span></span>
|<span data-ttu-id="dddc3-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dddc3-132">Relationship</span></span>|<span data-ttu-id="dddc3-133">型</span><span class="sxs-lookup"><span data-stu-id="dddc3-133">Type</span></span>|<span data-ttu-id="dddc3-134">説明</span><span class="sxs-lookup"><span data-stu-id="dddc3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddc3-135">definition</span><span class="sxs-lookup"><span data-stu-id="dddc3-135">definition</span></span>|[<span data-ttu-id="dddc3-136">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="dddc3-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="dddc3-137">プレゼンテーションに関連付けられたグループポリシーの定義。</span><span class="sxs-lookup"><span data-stu-id="dddc3-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dddc3-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dddc3-138">JSON Representation</span></span>
<span data-ttu-id="dddc3-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dddc3-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




