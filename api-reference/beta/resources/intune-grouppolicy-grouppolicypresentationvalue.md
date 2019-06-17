---
title: groupPolicyPresentationValue リソースの種類
description: 単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0403695c738cff5c709102859196deb510867246
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964774"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="842d1-103">groupPolicyPresentationValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="842d1-103">groupPolicyPresentationValue resource type</span></span>

> <span data-ttu-id="842d1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="842d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="842d1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="842d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="842d1-106">単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。</span><span class="sxs-lookup"><span data-stu-id="842d1-106">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="842d1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="842d1-107">Methods</span></span>
|<span data-ttu-id="842d1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="842d1-108">Method</span></span>|<span data-ttu-id="842d1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="842d1-109">Return Type</span></span>|<span data-ttu-id="842d1-110">説明</span><span class="sxs-lookup"><span data-stu-id="842d1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="842d1-111">GroupPolicyPresentationValues を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="842d1-111">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="842d1-112">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="842d1-112">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="842d1-113">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="842d1-113">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="842d1-114">GroupPolicyPresentationValue の取得</span><span class="sxs-lookup"><span data-stu-id="842d1-114">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="842d1-115">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="842d1-115">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="842d1-116">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="842d1-116">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="842d1-117">GroupPolicyPresentationValue の作成</span><span class="sxs-lookup"><span data-stu-id="842d1-117">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="842d1-118">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="842d1-118">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="842d1-119">新しい[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="842d1-119">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="842d1-120">GroupPolicyPresentationValue の削除</span><span class="sxs-lookup"><span data-stu-id="842d1-120">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="842d1-121">None</span><span class="sxs-lookup"><span data-stu-id="842d1-121">None</span></span>|<span data-ttu-id="842d1-122">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="842d1-122">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="842d1-123">GroupPolicyPresentationValue の更新</span><span class="sxs-lookup"><span data-stu-id="842d1-123">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="842d1-124">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="842d1-124">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="842d1-125">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="842d1-125">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="842d1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842d1-126">Properties</span></span>
|<span data-ttu-id="842d1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842d1-127">Property</span></span>|<span data-ttu-id="842d1-128">型</span><span class="sxs-lookup"><span data-stu-id="842d1-128">Type</span></span>|<span data-ttu-id="842d1-129">説明</span><span class="sxs-lookup"><span data-stu-id="842d1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842d1-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="842d1-130">lastModifiedDateTime</span></span>|<span data-ttu-id="842d1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842d1-131">DateTimeOffset</span></span>|<span data-ttu-id="842d1-132">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="842d1-132">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="842d1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="842d1-133">createdDateTime</span></span>|<span data-ttu-id="842d1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842d1-134">DateTimeOffset</span></span>|<span data-ttu-id="842d1-135">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="842d1-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="842d1-136">id</span><span class="sxs-lookup"><span data-stu-id="842d1-136">id</span></span>|<span data-ttu-id="842d1-137">String</span><span class="sxs-lookup"><span data-stu-id="842d1-137">String</span></span>|<span data-ttu-id="842d1-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="842d1-138">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="842d1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="842d1-139">Relationships</span></span>
|<span data-ttu-id="842d1-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="842d1-140">Relationship</span></span>|<span data-ttu-id="842d1-141">型</span><span class="sxs-lookup"><span data-stu-id="842d1-141">Type</span></span>|<span data-ttu-id="842d1-142">説明</span><span class="sxs-lookup"><span data-stu-id="842d1-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842d1-143">definitionValue</span><span class="sxs-lookup"><span data-stu-id="842d1-143">definitionValue</span></span>|[<span data-ttu-id="842d1-144">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="842d1-144">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="842d1-145">プレゼンテーション値に関連付けられているグループポリシー定義の値。</span><span class="sxs-lookup"><span data-stu-id="842d1-145">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="842d1-146">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="842d1-146">presentation</span></span>|[<span data-ttu-id="842d1-147">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="842d1-147">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="842d1-148">プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="842d1-148">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="842d1-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="842d1-149">JSON Representation</span></span>
<span data-ttu-id="842d1-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="842d1-150">Here is a JSON representation of the resource.</span></span>
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





