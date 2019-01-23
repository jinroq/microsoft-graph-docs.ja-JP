---
title: networkManagementCondition リソースの種類
description: ネットワーク管理の条件を定義するための情報が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4eadaf4e67b7ffe5551fc82376c3a4bb58255f61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415762"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="2db08-103">networkManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2db08-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="2db08-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2db08-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2db08-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2db08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2db08-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2db08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2db08-107">ネットワーク管理の条件を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2db08-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="2db08-108">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2db08-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2db08-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2db08-109">Methods</span></span>
|<span data-ttu-id="2db08-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2db08-110">Method</span></span>|<span data-ttu-id="2db08-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2db08-111">Return Type</span></span>|<span data-ttu-id="2db08-112">説明</span><span class="sxs-lookup"><span data-stu-id="2db08-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2db08-113">リスト networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="2db08-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="2db08-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2db08-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="2db08-115">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2db08-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="2db08-116">NetworkManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="2db08-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="2db08-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="2db08-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="2db08-118">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2db08-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2db08-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2db08-119">Properties</span></span>
|<span data-ttu-id="2db08-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2db08-120">Property</span></span>|<span data-ttu-id="2db08-121">型</span><span class="sxs-lookup"><span data-stu-id="2db08-121">Type</span></span>|<span data-ttu-id="2db08-122">説明</span><span class="sxs-lookup"><span data-stu-id="2db08-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2db08-123">id</span><span class="sxs-lookup"><span data-stu-id="2db08-123">id</span></span>|<span data-ttu-id="2db08-124">String</span><span class="sxs-lookup"><span data-stu-id="2db08-124">String</span></span>|<span data-ttu-id="2db08-125">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="2db08-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="2db08-126">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="2db08-126">System generated value assigned when created.</span></span> <span data-ttu-id="2db08-127">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-128">一意な名前</span><span class="sxs-lookup"><span data-stu-id="2db08-128">uniqueName</span></span>|<span data-ttu-id="2db08-129">String</span><span class="sxs-lookup"><span data-stu-id="2db08-129">String</span></span>|<span data-ttu-id="2db08-130">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="2db08-130">Unique name for the management condition.</span></span> <span data-ttu-id="2db08-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2db08-131">Used in management condition expressions.</span></span> <span data-ttu-id="2db08-132">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2db08-133">displayName</span></span>|<span data-ttu-id="2db08-134">String</span><span class="sxs-lookup"><span data-stu-id="2db08-134">String</span></span>|<span data-ttu-id="2db08-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="2db08-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="2db08-136">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-137">説明</span><span class="sxs-lookup"><span data-stu-id="2db08-137">description</span></span>|<span data-ttu-id="2db08-138">String</span><span class="sxs-lookup"><span data-stu-id="2db08-138">String</span></span>|<span data-ttu-id="2db08-139">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="2db08-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="2db08-140">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2db08-141">createdDateTime</span></span>|<span data-ttu-id="2db08-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2db08-142">DateTimeOffset</span></span>|<span data-ttu-id="2db08-143">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="2db08-143">The time the management condition was created.</span></span> <span data-ttu-id="2db08-144">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="2db08-144">Generated service side.</span></span> <span data-ttu-id="2db08-145">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-146">変更された日時</span><span class="sxs-lookup"><span data-stu-id="2db08-146">modifiedDateTime</span></span>|<span data-ttu-id="2db08-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2db08-147">DateTimeOffset</span></span>|<span data-ttu-id="2db08-148">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="2db08-148">The time the management condition was last modified.</span></span> <span data-ttu-id="2db08-149">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="2db08-149">Updated service side.</span></span> <span data-ttu-id="2db08-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-151">eTag</span><span class="sxs-lookup"><span data-stu-id="2db08-151">eTag</span></span>|<span data-ttu-id="2db08-152">String</span><span class="sxs-lookup"><span data-stu-id="2db08-152">String</span></span>|<span data-ttu-id="2db08-153">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="2db08-153">ETag of the management condition.</span></span> <span data-ttu-id="2db08-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="2db08-154">Updated service side.</span></span> <span data-ttu-id="2db08-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2db08-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="2db08-156">applicablePlatforms</span></span>|<span data-ttu-id="2db08-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2db08-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="2db08-158">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="2db08-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="2db08-159">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2db08-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2db08-160">Relationships</span></span>
|<span data-ttu-id="2db08-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2db08-161">Relationship</span></span>|<span data-ttu-id="2db08-162">型</span><span class="sxs-lookup"><span data-stu-id="2db08-162">Type</span></span>|<span data-ttu-id="2db08-163">説明</span><span class="sxs-lookup"><span data-stu-id="2db08-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2db08-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="2db08-164">managementConditionStatements</span></span>|<span data-ttu-id="2db08-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2db08-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="2db08-166">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="2db08-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="2db08-167">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2db08-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2db08-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2db08-168">JSON Representation</span></span>
<span data-ttu-id="2db08-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2db08-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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




