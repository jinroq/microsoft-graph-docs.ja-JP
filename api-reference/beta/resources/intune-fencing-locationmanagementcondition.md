---
title: locationManagementCondition リソースの種類
description: 場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c2eddf43696bd9300cc8dcd3408dbcd6fc5a9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422797"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="0569c-103">locationManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0569c-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="0569c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0569c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0569c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0569c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0569c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0569c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0569c-107">場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0569c-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="0569c-108">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0569c-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0569c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0569c-109">Methods</span></span>
|<span data-ttu-id="0569c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0569c-110">Method</span></span>|<span data-ttu-id="0569c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0569c-111">Return Type</span></span>|<span data-ttu-id="0569c-112">説明</span><span class="sxs-lookup"><span data-stu-id="0569c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0569c-113">リスト locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="0569c-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="0569c-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0569c-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="0569c-115">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0569c-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0569c-116">LocationManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="0569c-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="0569c-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0569c-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="0569c-118">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0569c-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0569c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0569c-119">Properties</span></span>
|<span data-ttu-id="0569c-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0569c-120">Property</span></span>|<span data-ttu-id="0569c-121">型</span><span class="sxs-lookup"><span data-stu-id="0569c-121">Type</span></span>|<span data-ttu-id="0569c-122">説明</span><span class="sxs-lookup"><span data-stu-id="0569c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0569c-123">id</span><span class="sxs-lookup"><span data-stu-id="0569c-123">id</span></span>|<span data-ttu-id="0569c-124">String</span><span class="sxs-lookup"><span data-stu-id="0569c-124">String</span></span>|<span data-ttu-id="0569c-125">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0569c-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="0569c-126">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0569c-126">System generated value assigned when created.</span></span> <span data-ttu-id="0569c-127">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-128">一意な名前</span><span class="sxs-lookup"><span data-stu-id="0569c-128">uniqueName</span></span>|<span data-ttu-id="0569c-129">String</span><span class="sxs-lookup"><span data-stu-id="0569c-129">String</span></span>|<span data-ttu-id="0569c-130">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="0569c-130">Unique name for the management condition.</span></span> <span data-ttu-id="0569c-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0569c-131">Used in management condition expressions.</span></span> <span data-ttu-id="0569c-132">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0569c-133">displayName</span></span>|<span data-ttu-id="0569c-134">String</span><span class="sxs-lookup"><span data-stu-id="0569c-134">String</span></span>|<span data-ttu-id="0569c-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="0569c-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="0569c-136">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-137">説明</span><span class="sxs-lookup"><span data-stu-id="0569c-137">description</span></span>|<span data-ttu-id="0569c-138">String</span><span class="sxs-lookup"><span data-stu-id="0569c-138">String</span></span>|<span data-ttu-id="0569c-139">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="0569c-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="0569c-140">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0569c-141">createdDateTime</span></span>|<span data-ttu-id="0569c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0569c-142">DateTimeOffset</span></span>|<span data-ttu-id="0569c-143">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0569c-143">The time the management condition was created.</span></span> <span data-ttu-id="0569c-144">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0569c-144">Generated service side.</span></span> <span data-ttu-id="0569c-145">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-146">変更された日時</span><span class="sxs-lookup"><span data-stu-id="0569c-146">modifiedDateTime</span></span>|<span data-ttu-id="0569c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0569c-147">DateTimeOffset</span></span>|<span data-ttu-id="0569c-148">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="0569c-148">The time the management condition was last modified.</span></span> <span data-ttu-id="0569c-149">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0569c-149">Updated service side.</span></span> <span data-ttu-id="0569c-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-151">eTag</span><span class="sxs-lookup"><span data-stu-id="0569c-151">eTag</span></span>|<span data-ttu-id="0569c-152">String</span><span class="sxs-lookup"><span data-stu-id="0569c-152">String</span></span>|<span data-ttu-id="0569c-153">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="0569c-153">ETag of the management condition.</span></span> <span data-ttu-id="0569c-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0569c-154">Updated service side.</span></span> <span data-ttu-id="0569c-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0569c-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0569c-156">applicablePlatforms</span></span>|<span data-ttu-id="0569c-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0569c-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0569c-158">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="0569c-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0569c-159">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0569c-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0569c-160">Relationships</span></span>
|<span data-ttu-id="0569c-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0569c-161">Relationship</span></span>|<span data-ttu-id="0569c-162">型</span><span class="sxs-lookup"><span data-stu-id="0569c-162">Type</span></span>|<span data-ttu-id="0569c-163">説明</span><span class="sxs-lookup"><span data-stu-id="0569c-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0569c-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0569c-164">managementConditionStatements</span></span>|<span data-ttu-id="0569c-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0569c-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0569c-166">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="0569c-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0569c-167">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0569c-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0569c-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0569c-168">JSON Representation</span></span>
<span data-ttu-id="0569c-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0569c-169">Here is a JSON representation of the resource.</span></span>
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




