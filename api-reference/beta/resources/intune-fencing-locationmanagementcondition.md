---
title: locationManagementCondition リソースの種類
description: 場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 541cf74decad641f6dc7751945e1d0ffceee1366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922978"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="0c843-103">locationManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c843-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="0c843-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c843-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c843-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c843-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c843-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c843-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c843-107">場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c843-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="0c843-108">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c843-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0c843-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c843-109">Methods</span></span>
|<span data-ttu-id="0c843-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c843-110">Method</span></span>|<span data-ttu-id="0c843-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c843-111">Return Type</span></span>|<span data-ttu-id="0c843-112">説明</span><span class="sxs-lookup"><span data-stu-id="0c843-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c843-113">リスト locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="0c843-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="0c843-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c843-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="0c843-115">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0c843-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0c843-116">LocationManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="0c843-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="0c843-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0c843-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="0c843-118">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c843-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c843-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c843-119">Properties</span></span>
|<span data-ttu-id="0c843-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c843-120">Property</span></span>|<span data-ttu-id="0c843-121">種類</span><span class="sxs-lookup"><span data-stu-id="0c843-121">Type</span></span>|<span data-ttu-id="0c843-122">説明</span><span class="sxs-lookup"><span data-stu-id="0c843-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c843-123">ID</span><span class="sxs-lookup"><span data-stu-id="0c843-123">id</span></span>|<span data-ttu-id="0c843-124">String</span><span class="sxs-lookup"><span data-stu-id="0c843-124">String</span></span>|<span data-ttu-id="0c843-125">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0c843-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="0c843-126">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0c843-126">System generated value assigned when created.</span></span> <span data-ttu-id="0c843-127">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-128">一意な名前</span><span class="sxs-lookup"><span data-stu-id="0c843-128">uniqueName</span></span>|<span data-ttu-id="0c843-129">String</span><span class="sxs-lookup"><span data-stu-id="0c843-129">String</span></span>|<span data-ttu-id="0c843-130">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="0c843-130">Unique name for the management condition.</span></span> <span data-ttu-id="0c843-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0c843-131">Used in management condition expressions.</span></span> <span data-ttu-id="0c843-132">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0c843-133">displayName</span></span>|<span data-ttu-id="0c843-134">String</span><span class="sxs-lookup"><span data-stu-id="0c843-134">String</span></span>|<span data-ttu-id="0c843-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="0c843-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="0c843-136">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-137">説明</span><span class="sxs-lookup"><span data-stu-id="0c843-137">description</span></span>|<span data-ttu-id="0c843-138">String</span><span class="sxs-lookup"><span data-stu-id="0c843-138">String</span></span>|<span data-ttu-id="0c843-139">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="0c843-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="0c843-140">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c843-141">createdDateTime</span></span>|<span data-ttu-id="0c843-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c843-142">DateTimeOffset</span></span>|<span data-ttu-id="0c843-143">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0c843-143">The time the management condition was created.</span></span> <span data-ttu-id="0c843-144">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0c843-144">Generated service side.</span></span> <span data-ttu-id="0c843-145">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-146">変更された日時</span><span class="sxs-lookup"><span data-stu-id="0c843-146">modifiedDateTime</span></span>|<span data-ttu-id="0c843-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c843-147">DateTimeOffset</span></span>|<span data-ttu-id="0c843-148">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="0c843-148">The time the management condition was last modified.</span></span> <span data-ttu-id="0c843-149">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0c843-149">Updated service side.</span></span> <span data-ttu-id="0c843-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-151">eTag</span><span class="sxs-lookup"><span data-stu-id="0c843-151">eTag</span></span>|<span data-ttu-id="0c843-152">String</span><span class="sxs-lookup"><span data-stu-id="0c843-152">String</span></span>|<span data-ttu-id="0c843-153">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="0c843-153">ETag of the management condition.</span></span> <span data-ttu-id="0c843-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0c843-154">Updated service side.</span></span> <span data-ttu-id="0c843-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c843-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0c843-156">applicablePlatforms</span></span>|<span data-ttu-id="0c843-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c843-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0c843-158">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="0c843-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0c843-159">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c843-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c843-160">Relationships</span></span>
|<span data-ttu-id="0c843-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c843-161">Relationship</span></span>|<span data-ttu-id="0c843-162">型</span><span class="sxs-lookup"><span data-stu-id="0c843-162">Type</span></span>|<span data-ttu-id="0c843-163">説明</span><span class="sxs-lookup"><span data-stu-id="0c843-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c843-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0c843-164">managementConditionStatements</span></span>|<span data-ttu-id="0c843-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c843-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0c843-166">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="0c843-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0c843-167">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c843-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c843-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c843-168">JSON Representation</span></span>
<span data-ttu-id="0c843-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c843-169">Here is a JSON representation of the resource.</span></span>
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





