---
title: locationManagementCondition リソースの種類
description: 場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 85d3b638c81990a98623501b8dcb3ad0705f2e6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832635"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="8032d-103">locationManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8032d-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="8032d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8032d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8032d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8032d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8032d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8032d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8032d-107">場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8032d-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="8032d-108">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8032d-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8032d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8032d-109">Methods</span></span>
|<span data-ttu-id="8032d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="8032d-110">Method</span></span>|<span data-ttu-id="8032d-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8032d-111">Return Type</span></span>|<span data-ttu-id="8032d-112">説明</span><span class="sxs-lookup"><span data-stu-id="8032d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8032d-113">リスト locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="8032d-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="8032d-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8032d-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="8032d-115">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8032d-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="8032d-116">LocationManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="8032d-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="8032d-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="8032d-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="8032d-118">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8032d-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8032d-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8032d-119">Properties</span></span>
|<span data-ttu-id="8032d-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8032d-120">Property</span></span>|<span data-ttu-id="8032d-121">種類</span><span class="sxs-lookup"><span data-stu-id="8032d-121">Type</span></span>|<span data-ttu-id="8032d-122">説明</span><span class="sxs-lookup"><span data-stu-id="8032d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8032d-123">ID</span><span class="sxs-lookup"><span data-stu-id="8032d-123">id</span></span>|<span data-ttu-id="8032d-124">String</span><span class="sxs-lookup"><span data-stu-id="8032d-124">String</span></span>|<span data-ttu-id="8032d-125">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="8032d-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="8032d-126">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="8032d-126">System generated value assigned when created.</span></span> <span data-ttu-id="8032d-127">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-128">一意な名前</span><span class="sxs-lookup"><span data-stu-id="8032d-128">uniqueName</span></span>|<span data-ttu-id="8032d-129">String</span><span class="sxs-lookup"><span data-stu-id="8032d-129">String</span></span>|<span data-ttu-id="8032d-130">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="8032d-130">Unique name for the management condition.</span></span> <span data-ttu-id="8032d-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8032d-131">Used in management condition expressions.</span></span> <span data-ttu-id="8032d-132">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8032d-133">displayName</span></span>|<span data-ttu-id="8032d-134">String</span><span class="sxs-lookup"><span data-stu-id="8032d-134">String</span></span>|<span data-ttu-id="8032d-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="8032d-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="8032d-136">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-137">説明</span><span class="sxs-lookup"><span data-stu-id="8032d-137">description</span></span>|<span data-ttu-id="8032d-138">String</span><span class="sxs-lookup"><span data-stu-id="8032d-138">String</span></span>|<span data-ttu-id="8032d-139">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="8032d-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="8032d-140">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8032d-141">createdDateTime</span></span>|<span data-ttu-id="8032d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8032d-142">DateTimeOffset</span></span>|<span data-ttu-id="8032d-143">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="8032d-143">The time the management condition was created.</span></span> <span data-ttu-id="8032d-144">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="8032d-144">Generated service side.</span></span> <span data-ttu-id="8032d-145">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-146">変更された日時</span><span class="sxs-lookup"><span data-stu-id="8032d-146">modifiedDateTime</span></span>|<span data-ttu-id="8032d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8032d-147">DateTimeOffset</span></span>|<span data-ttu-id="8032d-148">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="8032d-148">The time the management condition was last modified.</span></span> <span data-ttu-id="8032d-149">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="8032d-149">Updated service side.</span></span> <span data-ttu-id="8032d-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-151">eTag</span><span class="sxs-lookup"><span data-stu-id="8032d-151">eTag</span></span>|<span data-ttu-id="8032d-152">String</span><span class="sxs-lookup"><span data-stu-id="8032d-152">String</span></span>|<span data-ttu-id="8032d-153">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="8032d-153">ETag of the management condition.</span></span> <span data-ttu-id="8032d-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="8032d-154">Updated service side.</span></span> <span data-ttu-id="8032d-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8032d-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="8032d-156">applicablePlatforms</span></span>|<span data-ttu-id="8032d-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8032d-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="8032d-158">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="8032d-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="8032d-159">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8032d-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8032d-160">Relationships</span></span>
|<span data-ttu-id="8032d-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8032d-161">Relationship</span></span>|<span data-ttu-id="8032d-162">型</span><span class="sxs-lookup"><span data-stu-id="8032d-162">Type</span></span>|<span data-ttu-id="8032d-163">説明</span><span class="sxs-lookup"><span data-stu-id="8032d-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8032d-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="8032d-164">managementConditionStatements</span></span>|<span data-ttu-id="8032d-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8032d-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="8032d-166">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="8032d-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="8032d-167">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8032d-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8032d-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8032d-168">JSON Representation</span></span>
<span data-ttu-id="8032d-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8032d-169">Here is a JSON representation of the resource.</span></span>
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





