---
title: locationmanagementcondition リソースの種類
description: 監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07bf05fa8ab6f7f7f1ce6e1978645f289ea57a2f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143310"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="165d4-103">locationmanagementcondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="165d4-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="165d4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="165d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="165d4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="165d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="165d4-106">監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="165d4-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="165d4-107">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="165d4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="165d4-108">Methods</span></span>
|<span data-ttu-id="165d4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="165d4-109">Method</span></span>|<span data-ttu-id="165d4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="165d4-110">Return Type</span></span>|<span data-ttu-id="165d4-111">説明</span><span class="sxs-lookup"><span data-stu-id="165d4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="165d4-112">locationmanagementconditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="165d4-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="165d4-113">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="165d4-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="165d4-114">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="165d4-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="165d4-115">locationmanagementcondition の取得</span><span class="sxs-lookup"><span data-stu-id="165d4-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="165d4-116">locationmanagementcondition</span><span class="sxs-lookup"><span data-stu-id="165d4-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="165d4-117">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="165d4-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="165d4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="165d4-118">Properties</span></span>
|<span data-ttu-id="165d4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="165d4-119">Property</span></span>|<span data-ttu-id="165d4-120">型</span><span class="sxs-lookup"><span data-stu-id="165d4-120">Type</span></span>|<span data-ttu-id="165d4-121">説明</span><span class="sxs-lookup"><span data-stu-id="165d4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165d4-122">id</span><span class="sxs-lookup"><span data-stu-id="165d4-122">id</span></span>|<span data-ttu-id="165d4-123">文字列</span><span class="sxs-lookup"><span data-stu-id="165d4-123">String</span></span>|<span data-ttu-id="165d4-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="165d4-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="165d4-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="165d4-125">System generated value assigned when created.</span></span> <span data-ttu-id="165d4-126">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="165d4-127">uniqueName</span></span>|<span data-ttu-id="165d4-128">String</span><span class="sxs-lookup"><span data-stu-id="165d4-128">String</span></span>|<span data-ttu-id="165d4-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="165d4-129">Unique name for the management condition.</span></span> <span data-ttu-id="165d4-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="165d4-130">Used in management condition expressions.</span></span> <span data-ttu-id="165d4-131">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="165d4-132">displayName</span></span>|<span data-ttu-id="165d4-133">String</span><span class="sxs-lookup"><span data-stu-id="165d4-133">String</span></span>|<span data-ttu-id="165d4-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="165d4-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="165d4-135">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-136">説明</span><span class="sxs-lookup"><span data-stu-id="165d4-136">description</span></span>|<span data-ttu-id="165d4-137">String</span><span class="sxs-lookup"><span data-stu-id="165d4-137">String</span></span>|<span data-ttu-id="165d4-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="165d4-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="165d4-139">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="165d4-140">createdDateTime</span></span>|<span data-ttu-id="165d4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="165d4-141">DateTimeOffset</span></span>|<span data-ttu-id="165d4-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="165d4-142">The time the management condition was created.</span></span> <span data-ttu-id="165d4-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="165d4-143">Generated service side.</span></span> <span data-ttu-id="165d4-144">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-145">変更された日時</span><span class="sxs-lookup"><span data-stu-id="165d4-145">modifiedDateTime</span></span>|<span data-ttu-id="165d4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="165d4-146">DateTimeOffset</span></span>|<span data-ttu-id="165d4-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="165d4-147">The time the management condition was last modified.</span></span> <span data-ttu-id="165d4-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="165d4-148">Updated service side.</span></span> <span data-ttu-id="165d4-149">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-150">eTag</span><span class="sxs-lookup"><span data-stu-id="165d4-150">eTag</span></span>|<span data-ttu-id="165d4-151">String</span><span class="sxs-lookup"><span data-stu-id="165d4-151">String</span></span>|<span data-ttu-id="165d4-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="165d4-152">ETag of the management condition.</span></span> <span data-ttu-id="165d4-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="165d4-153">Updated service side.</span></span> <span data-ttu-id="165d4-154">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="165d4-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="165d4-155">applicablePlatforms</span></span>|<span data-ttu-id="165d4-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="165d4-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="165d4-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="165d4-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="165d4-158">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="165d4-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="165d4-159">Relationships</span></span>
|<span data-ttu-id="165d4-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="165d4-160">Relationship</span></span>|<span data-ttu-id="165d4-161">型</span><span class="sxs-lookup"><span data-stu-id="165d4-161">Type</span></span>|<span data-ttu-id="165d4-162">説明</span><span class="sxs-lookup"><span data-stu-id="165d4-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165d4-163">managementconditionstatements</span><span class="sxs-lookup"><span data-stu-id="165d4-163">managementConditionStatements</span></span>|<span data-ttu-id="165d4-164">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="165d4-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="165d4-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="165d4-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="165d4-166">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="165d4-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="165d4-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="165d4-167">JSON Representation</span></span>
<span data-ttu-id="165d4-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="165d4-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




