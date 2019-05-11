---
title: locationManagementCondition リソースの種類
description: 監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d679ef9353bbb0dd0fcedc342b793afeade158c1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941297"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="f3c81-103">locationManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3c81-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="f3c81-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3c81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3c81-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3c81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c81-106">監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3c81-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="f3c81-107">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f3c81-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3c81-108">Methods</span></span>
|<span data-ttu-id="f3c81-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3c81-109">Method</span></span>|<span data-ttu-id="f3c81-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f3c81-110">Return Type</span></span>|<span data-ttu-id="f3c81-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3c81-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3c81-112">LocationManagementConditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f3c81-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="f3c81-113">[Locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3c81-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="f3c81-114">[Locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f3c81-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="f3c81-115">LocationManagementCondition の取得</span><span class="sxs-lookup"><span data-stu-id="f3c81-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="f3c81-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f3c81-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="f3c81-117">[Locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f3c81-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3c81-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3c81-118">Properties</span></span>
|<span data-ttu-id="f3c81-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3c81-119">Property</span></span>|<span data-ttu-id="f3c81-120">種類</span><span class="sxs-lookup"><span data-stu-id="f3c81-120">Type</span></span>|<span data-ttu-id="f3c81-121">説明</span><span class="sxs-lookup"><span data-stu-id="f3c81-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c81-122">id</span><span class="sxs-lookup"><span data-stu-id="f3c81-122">id</span></span>|<span data-ttu-id="f3c81-123">文字列</span><span class="sxs-lookup"><span data-stu-id="f3c81-123">String</span></span>|<span data-ttu-id="f3c81-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f3c81-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="f3c81-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="f3c81-125">System generated value assigned when created.</span></span> <span data-ttu-id="f3c81-126">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f3c81-127">uniqueName</span></span>|<span data-ttu-id="f3c81-128">String</span><span class="sxs-lookup"><span data-stu-id="f3c81-128">String</span></span>|<span data-ttu-id="f3c81-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="f3c81-129">Unique name for the management condition.</span></span> <span data-ttu-id="f3c81-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f3c81-130">Used in management condition expressions.</span></span> <span data-ttu-id="f3c81-131">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f3c81-132">displayName</span></span>|<span data-ttu-id="f3c81-133">String</span><span class="sxs-lookup"><span data-stu-id="f3c81-133">String</span></span>|<span data-ttu-id="f3c81-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="f3c81-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="f3c81-135">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-136">description</span><span class="sxs-lookup"><span data-stu-id="f3c81-136">description</span></span>|<span data-ttu-id="f3c81-137">String</span><span class="sxs-lookup"><span data-stu-id="f3c81-137">String</span></span>|<span data-ttu-id="f3c81-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="f3c81-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="f3c81-139">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c81-140">createdDateTime</span></span>|<span data-ttu-id="f3c81-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c81-141">DateTimeOffset</span></span>|<span data-ttu-id="f3c81-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="f3c81-142">The time the management condition was created.</span></span> <span data-ttu-id="f3c81-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="f3c81-143">Generated service side.</span></span> <span data-ttu-id="f3c81-144">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c81-145">modifiedDateTime</span></span>|<span data-ttu-id="f3c81-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c81-146">DateTimeOffset</span></span>|<span data-ttu-id="f3c81-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="f3c81-147">The time the management condition was last modified.</span></span> <span data-ttu-id="f3c81-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f3c81-148">Updated service side.</span></span> <span data-ttu-id="f3c81-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-150">eTag</span><span class="sxs-lookup"><span data-stu-id="f3c81-150">eTag</span></span>|<span data-ttu-id="f3c81-151">String</span><span class="sxs-lookup"><span data-stu-id="f3c81-151">String</span></span>|<span data-ttu-id="f3c81-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="f3c81-152">ETag of the management condition.</span></span> <span data-ttu-id="f3c81-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f3c81-153">Updated service side.</span></span> <span data-ttu-id="f3c81-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f3c81-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="f3c81-155">applicablePlatforms</span></span>|<span data-ttu-id="f3c81-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3c81-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f3c81-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="f3c81-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f3c81-158">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3c81-159">関係</span><span class="sxs-lookup"><span data-stu-id="f3c81-159">Relationships</span></span>
|<span data-ttu-id="f3c81-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3c81-160">Relationship</span></span>|<span data-ttu-id="f3c81-161">型</span><span class="sxs-lookup"><span data-stu-id="f3c81-161">Type</span></span>|<span data-ttu-id="f3c81-162">説明</span><span class="sxs-lookup"><span data-stu-id="f3c81-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c81-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="f3c81-163">managementConditionStatements</span></span>|<span data-ttu-id="f3c81-164">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3c81-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="f3c81-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="f3c81-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="f3c81-166">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3c81-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3c81-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3c81-167">JSON Representation</span></span>
<span data-ttu-id="f3c81-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3c81-168">Here is a JSON representation of the resource.</span></span>
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




