---
title: locationmanagementcondition リソースの種類
description: 監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2560309e937bb1b2e6ffd436cec5988fd38dbf2c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773148"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="8bd87-103">locationmanagementcondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bd87-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="8bd87-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bd87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bd87-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bd87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bd87-106">監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8bd87-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="8bd87-107">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8bd87-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8bd87-108">Methods</span></span>
|<span data-ttu-id="8bd87-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8bd87-109">Method</span></span>|<span data-ttu-id="8bd87-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8bd87-110">Return Type</span></span>|<span data-ttu-id="8bd87-111">説明</span><span class="sxs-lookup"><span data-stu-id="8bd87-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8bd87-112">locationmanagementconditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8bd87-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="8bd87-113">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8bd87-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="8bd87-114">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8bd87-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="8bd87-115">locationmanagementcondition の取得</span><span class="sxs-lookup"><span data-stu-id="8bd87-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="8bd87-116">locationmanagementcondition</span><span class="sxs-lookup"><span data-stu-id="8bd87-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="8bd87-117">[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8bd87-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bd87-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bd87-118">Properties</span></span>
|<span data-ttu-id="8bd87-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bd87-119">Property</span></span>|<span data-ttu-id="8bd87-120">型</span><span class="sxs-lookup"><span data-stu-id="8bd87-120">Type</span></span>|<span data-ttu-id="8bd87-121">説明</span><span class="sxs-lookup"><span data-stu-id="8bd87-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bd87-122">id</span><span class="sxs-lookup"><span data-stu-id="8bd87-122">id</span></span>|<span data-ttu-id="8bd87-123">文字列</span><span class="sxs-lookup"><span data-stu-id="8bd87-123">String</span></span>|<span data-ttu-id="8bd87-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8bd87-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="8bd87-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="8bd87-125">System generated value assigned when created.</span></span> <span data-ttu-id="8bd87-126">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="8bd87-127">uniqueName</span></span>|<span data-ttu-id="8bd87-128">文字列</span><span class="sxs-lookup"><span data-stu-id="8bd87-128">String</span></span>|<span data-ttu-id="8bd87-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="8bd87-129">Unique name for the management condition.</span></span> <span data-ttu-id="8bd87-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8bd87-130">Used in management condition expressions.</span></span> <span data-ttu-id="8bd87-131">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8bd87-132">displayName</span></span>|<span data-ttu-id="8bd87-133">String</span><span class="sxs-lookup"><span data-stu-id="8bd87-133">String</span></span>|<span data-ttu-id="8bd87-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="8bd87-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="8bd87-135">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-136">説明</span><span class="sxs-lookup"><span data-stu-id="8bd87-136">description</span></span>|<span data-ttu-id="8bd87-137">String</span><span class="sxs-lookup"><span data-stu-id="8bd87-137">String</span></span>|<span data-ttu-id="8bd87-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="8bd87-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="8bd87-139">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bd87-140">createdDateTime</span></span>|<span data-ttu-id="8bd87-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bd87-141">DateTimeOffset</span></span>|<span data-ttu-id="8bd87-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="8bd87-142">The time the management condition was created.</span></span> <span data-ttu-id="8bd87-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="8bd87-143">Generated service side.</span></span> <span data-ttu-id="8bd87-144">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bd87-145">modifiedDateTime</span></span>|<span data-ttu-id="8bd87-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bd87-146">DateTimeOffset</span></span>|<span data-ttu-id="8bd87-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="8bd87-147">The time the management condition was last modified.</span></span> <span data-ttu-id="8bd87-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8bd87-148">Updated service side.</span></span> <span data-ttu-id="8bd87-149">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-150">eTag</span><span class="sxs-lookup"><span data-stu-id="8bd87-150">eTag</span></span>|<span data-ttu-id="8bd87-151">String</span><span class="sxs-lookup"><span data-stu-id="8bd87-151">String</span></span>|<span data-ttu-id="8bd87-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="8bd87-152">ETag of the management condition.</span></span> <span data-ttu-id="8bd87-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8bd87-153">Updated service side.</span></span> <span data-ttu-id="8bd87-154">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8bd87-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="8bd87-155">applicablePlatforms</span></span>|<span data-ttu-id="8bd87-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8bd87-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="8bd87-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="8bd87-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="8bd87-158">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bd87-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8bd87-159">Relationships</span></span>
|<span data-ttu-id="8bd87-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8bd87-160">Relationship</span></span>|<span data-ttu-id="8bd87-161">型</span><span class="sxs-lookup"><span data-stu-id="8bd87-161">Type</span></span>|<span data-ttu-id="8bd87-162">説明</span><span class="sxs-lookup"><span data-stu-id="8bd87-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bd87-163">managementconditionstatements</span><span class="sxs-lookup"><span data-stu-id="8bd87-163">managementConditionStatements</span></span>|<span data-ttu-id="8bd87-164">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8bd87-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="8bd87-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="8bd87-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="8bd87-166">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="8bd87-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bd87-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bd87-167">JSON Representation</span></span>
<span data-ttu-id="8bd87-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8bd87-168">Here is a JSON representation of the resource.</span></span>
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





