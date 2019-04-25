---
title: networkmanagementcondition リソースの種類
description: ネットワーク管理条件を定義するための情報が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61b5165fb57080bc8568c7f09f1ee9e601d24297
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580840"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="be57a-103">networkmanagementcondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be57a-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="be57a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be57a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be57a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be57a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be57a-106">ネットワーク管理条件を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="be57a-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="be57a-107">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="be57a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="be57a-108">Methods</span></span>
|<span data-ttu-id="be57a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="be57a-109">Method</span></span>|<span data-ttu-id="be57a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be57a-110">Return Type</span></span>|<span data-ttu-id="be57a-111">説明</span><span class="sxs-lookup"><span data-stu-id="be57a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be57a-112">networkmanagementconditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="be57a-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="be57a-113">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be57a-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="be57a-114">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="be57a-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="be57a-115">networkmanagementcondition の取得</span><span class="sxs-lookup"><span data-stu-id="be57a-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="be57a-116">networkmanagementcondition</span><span class="sxs-lookup"><span data-stu-id="be57a-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="be57a-117">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="be57a-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be57a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be57a-118">Properties</span></span>
|<span data-ttu-id="be57a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be57a-119">Property</span></span>|<span data-ttu-id="be57a-120">型</span><span class="sxs-lookup"><span data-stu-id="be57a-120">Type</span></span>|<span data-ttu-id="be57a-121">説明</span><span class="sxs-lookup"><span data-stu-id="be57a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be57a-122">id</span><span class="sxs-lookup"><span data-stu-id="be57a-122">id</span></span>|<span data-ttu-id="be57a-123">String</span><span class="sxs-lookup"><span data-stu-id="be57a-123">String</span></span>|<span data-ttu-id="be57a-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="be57a-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="be57a-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="be57a-125">System generated value assigned when created.</span></span> <span data-ttu-id="be57a-126">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="be57a-127">uniqueName</span></span>|<span data-ttu-id="be57a-128">String</span><span class="sxs-lookup"><span data-stu-id="be57a-128">String</span></span>|<span data-ttu-id="be57a-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="be57a-129">Unique name for the management condition.</span></span> <span data-ttu-id="be57a-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="be57a-130">Used in management condition expressions.</span></span> <span data-ttu-id="be57a-131">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="be57a-132">displayName</span></span>|<span data-ttu-id="be57a-133">String</span><span class="sxs-lookup"><span data-stu-id="be57a-133">String</span></span>|<span data-ttu-id="be57a-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="be57a-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="be57a-135">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-136">説明</span><span class="sxs-lookup"><span data-stu-id="be57a-136">description</span></span>|<span data-ttu-id="be57a-137">String</span><span class="sxs-lookup"><span data-stu-id="be57a-137">String</span></span>|<span data-ttu-id="be57a-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="be57a-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="be57a-139">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be57a-140">createdDateTime</span></span>|<span data-ttu-id="be57a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be57a-141">DateTimeOffset</span></span>|<span data-ttu-id="be57a-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="be57a-142">The time the management condition was created.</span></span> <span data-ttu-id="be57a-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="be57a-143">Generated service side.</span></span> <span data-ttu-id="be57a-144">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be57a-145">modifiedDateTime</span></span>|<span data-ttu-id="be57a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be57a-146">DateTimeOffset</span></span>|<span data-ttu-id="be57a-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="be57a-147">The time the management condition was last modified.</span></span> <span data-ttu-id="be57a-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="be57a-148">Updated service side.</span></span> <span data-ttu-id="be57a-149">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-150">eTag</span><span class="sxs-lookup"><span data-stu-id="be57a-150">eTag</span></span>|<span data-ttu-id="be57a-151">String</span><span class="sxs-lookup"><span data-stu-id="be57a-151">String</span></span>|<span data-ttu-id="be57a-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="be57a-152">ETag of the management condition.</span></span> <span data-ttu-id="be57a-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="be57a-153">Updated service side.</span></span> <span data-ttu-id="be57a-154">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="be57a-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="be57a-155">applicablePlatforms</span></span>|<span data-ttu-id="be57a-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be57a-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="be57a-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="be57a-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="be57a-158">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="be57a-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be57a-159">Relationships</span></span>
|<span data-ttu-id="be57a-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be57a-160">Relationship</span></span>|<span data-ttu-id="be57a-161">型</span><span class="sxs-lookup"><span data-stu-id="be57a-161">Type</span></span>|<span data-ttu-id="be57a-162">説明</span><span class="sxs-lookup"><span data-stu-id="be57a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be57a-163">managementconditionstatements</span><span class="sxs-lookup"><span data-stu-id="be57a-163">managementConditionStatements</span></span>|<span data-ttu-id="be57a-164">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be57a-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="be57a-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="be57a-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="be57a-166">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be57a-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be57a-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be57a-167">JSON Representation</span></span>
<span data-ttu-id="be57a-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be57a-168">Here is a JSON representation of the resource.</span></span>
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





