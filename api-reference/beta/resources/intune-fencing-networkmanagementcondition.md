---
title: networkManagementCondition リソースの種類
description: ネットワーク管理の条件を定義するための情報が含まれています。
ms.openlocfilehash: 0a514d079b7b5737c4ee4514920a203d8a4b3ae1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070108"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="bb520-103">networkManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb520-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="bb520-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bb520-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb520-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb520-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb520-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb520-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb520-107">ネットワーク管理の条件を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb520-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="bb520-108">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb520-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bb520-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb520-109">Methods</span></span>
|<span data-ttu-id="bb520-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb520-110">Method</span></span>|<span data-ttu-id="bb520-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb520-111">Return Type</span></span>|<span data-ttu-id="bb520-112">説明</span><span class="sxs-lookup"><span data-stu-id="bb520-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb520-113">リスト networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="bb520-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="bb520-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb520-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="bb520-115">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bb520-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="bb520-116">NetworkManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb520-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="bb520-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="bb520-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="bb520-118">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb520-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb520-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb520-119">Properties</span></span>
|<span data-ttu-id="bb520-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb520-120">Property</span></span>|<span data-ttu-id="bb520-121">型</span><span class="sxs-lookup"><span data-stu-id="bb520-121">Type</span></span>|<span data-ttu-id="bb520-122">説明</span><span class="sxs-lookup"><span data-stu-id="bb520-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb520-123">id</span><span class="sxs-lookup"><span data-stu-id="bb520-123">id</span></span>|<span data-ttu-id="bb520-124">String</span><span class="sxs-lookup"><span data-stu-id="bb520-124">String</span></span>|<span data-ttu-id="bb520-125">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bb520-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="bb520-126">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="bb520-126">System generated value assigned when created.</span></span> <span data-ttu-id="bb520-127">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-128">一意な名前</span><span class="sxs-lookup"><span data-stu-id="bb520-128">uniqueName</span></span>|<span data-ttu-id="bb520-129">String</span><span class="sxs-lookup"><span data-stu-id="bb520-129">String</span></span>|<span data-ttu-id="bb520-130">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="bb520-130">Unique name for the management condition.</span></span> <span data-ttu-id="bb520-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bb520-131">Used in management condition expressions.</span></span> <span data-ttu-id="bb520-132">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bb520-133">displayName</span></span>|<span data-ttu-id="bb520-134">String</span><span class="sxs-lookup"><span data-stu-id="bb520-134">String</span></span>|<span data-ttu-id="bb520-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb520-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="bb520-136">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-137">説明</span><span class="sxs-lookup"><span data-stu-id="bb520-137">description</span></span>|<span data-ttu-id="bb520-138">String</span><span class="sxs-lookup"><span data-stu-id="bb520-138">String</span></span>|<span data-ttu-id="bb520-139">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb520-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="bb520-140">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb520-141">createdDateTime</span></span>|<span data-ttu-id="bb520-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb520-142">DateTimeOffset</span></span>|<span data-ttu-id="bb520-143">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="bb520-143">The time the management condition was created.</span></span> <span data-ttu-id="bb520-144">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="bb520-144">Generated service side.</span></span> <span data-ttu-id="bb520-145">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-146">変更された日時</span><span class="sxs-lookup"><span data-stu-id="bb520-146">modifiedDateTime</span></span>|<span data-ttu-id="bb520-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb520-147">DateTimeOffset</span></span>|<span data-ttu-id="bb520-148">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="bb520-148">The time the management condition was last modified.</span></span> <span data-ttu-id="bb520-149">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb520-149">Updated service side.</span></span> <span data-ttu-id="bb520-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-151">eTag</span><span class="sxs-lookup"><span data-stu-id="bb520-151">eTag</span></span>|<span data-ttu-id="bb520-152">String</span><span class="sxs-lookup"><span data-stu-id="bb520-152">String</span></span>|<span data-ttu-id="bb520-153">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="bb520-153">ETag of the management condition.</span></span> <span data-ttu-id="bb520-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb520-154">Updated service side.</span></span> <span data-ttu-id="bb520-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb520-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="bb520-156">applicablePlatforms</span></span>|<span data-ttu-id="bb520-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb520-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="bb520-158">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="bb520-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="bb520-159">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb520-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb520-160">Relationships</span></span>
|<span data-ttu-id="bb520-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb520-161">Relationship</span></span>|<span data-ttu-id="bb520-162">型</span><span class="sxs-lookup"><span data-stu-id="bb520-162">Type</span></span>|<span data-ttu-id="bb520-163">説明</span><span class="sxs-lookup"><span data-stu-id="bb520-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb520-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="bb520-164">managementConditionStatements</span></span>|<span data-ttu-id="bb520-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb520-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="bb520-166">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="bb520-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="bb520-167">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bb520-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb520-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb520-168">JSON Representation</span></span>
<span data-ttu-id="bb520-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb520-169">Here is a JSON representation of the resource.</span></span>
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





