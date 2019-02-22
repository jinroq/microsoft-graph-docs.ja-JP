---
title: grouppolicypresentationvalue リソースの種類
description: 単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7449ba37fe1ce747d698b01979ae4c88525dad7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156932"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="8fff4-103">grouppolicypresentationvalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fff4-103">groupPolicyPresentationValue resource type</span></span>

> <span data-ttu-id="8fff4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fff4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fff4-106">単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。</span><span class="sxs-lookup"><span data-stu-id="8fff4-106">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="8fff4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fff4-107">Methods</span></span>
|<span data-ttu-id="8fff4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8fff4-108">Method</span></span>|<span data-ttu-id="8fff4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8fff4-109">Return Type</span></span>|<span data-ttu-id="8fff4-110">説明</span><span class="sxs-lookup"><span data-stu-id="8fff4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8fff4-111">grouppolicypresentationvalues を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8fff4-111">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="8fff4-112">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8fff4-112">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="8fff4-113">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8fff4-113">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="8fff4-114">grouppolicypresentationvalue の取得</span><span class="sxs-lookup"><span data-stu-id="8fff4-114">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="8fff4-115">grouppolicypresentationvalue</span><span class="sxs-lookup"><span data-stu-id="8fff4-115">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="8fff4-116">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8fff4-116">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="8fff4-117">grouppolicypresentationvalue の作成</span><span class="sxs-lookup"><span data-stu-id="8fff4-117">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="8fff4-118">grouppolicypresentationvalue</span><span class="sxs-lookup"><span data-stu-id="8fff4-118">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="8fff4-119">新しい[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8fff4-119">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="8fff4-120">grouppolicypresentationvalue の削除</span><span class="sxs-lookup"><span data-stu-id="8fff4-120">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="8fff4-121">なし</span><span class="sxs-lookup"><span data-stu-id="8fff4-121">None</span></span>|<span data-ttu-id="8fff4-122">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fff4-122">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="8fff4-123">grouppolicypresentationvalue の更新</span><span class="sxs-lookup"><span data-stu-id="8fff4-123">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="8fff4-124">grouppolicypresentationvalue</span><span class="sxs-lookup"><span data-stu-id="8fff4-124">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="8fff4-125">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8fff4-125">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fff4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fff4-126">Properties</span></span>
|<span data-ttu-id="8fff4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fff4-127">Property</span></span>|<span data-ttu-id="8fff4-128">型</span><span class="sxs-lookup"><span data-stu-id="8fff4-128">Type</span></span>|<span data-ttu-id="8fff4-129">説明</span><span class="sxs-lookup"><span data-stu-id="8fff4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fff4-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fff4-130">lastModifiedDateTime</span></span>|<span data-ttu-id="8fff4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fff4-131">DateTimeOffset</span></span>|<span data-ttu-id="8fff4-132">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8fff4-132">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="8fff4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fff4-133">createdDateTime</span></span>|<span data-ttu-id="8fff4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fff4-134">DateTimeOffset</span></span>|<span data-ttu-id="8fff4-135">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8fff4-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="8fff4-136">id</span><span class="sxs-lookup"><span data-stu-id="8fff4-136">id</span></span>|<span data-ttu-id="8fff4-137">String</span><span class="sxs-lookup"><span data-stu-id="8fff4-137">String</span></span>|<span data-ttu-id="8fff4-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8fff4-138">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fff4-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fff4-139">Relationships</span></span>
|<span data-ttu-id="8fff4-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fff4-140">Relationship</span></span>|<span data-ttu-id="8fff4-141">型</span><span class="sxs-lookup"><span data-stu-id="8fff4-141">Type</span></span>|<span data-ttu-id="8fff4-142">説明</span><span class="sxs-lookup"><span data-stu-id="8fff4-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fff4-143">definitionvalue</span><span class="sxs-lookup"><span data-stu-id="8fff4-143">definitionValue</span></span>|[<span data-ttu-id="8fff4-144">grouppolicydefinitionvalue</span><span class="sxs-lookup"><span data-stu-id="8fff4-144">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="8fff4-145">プレゼンテーション値に関連付けられているグループポリシー定義の値。</span><span class="sxs-lookup"><span data-stu-id="8fff4-145">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="8fff4-146">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="8fff4-146">presentation</span></span>|[<span data-ttu-id="8fff4-147">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="8fff4-147">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="8fff4-148">プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="8fff4-148">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fff4-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fff4-149">JSON Representation</span></span>
<span data-ttu-id="8fff4-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fff4-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




