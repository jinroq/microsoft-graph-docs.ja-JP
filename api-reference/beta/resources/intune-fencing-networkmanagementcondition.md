---
title: networkmanagementcondition リソースの種類
description: ネットワーク管理条件を定義するための情報が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61b5165fb57080bc8568c7f09f1ee9e601d24297
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780120"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="68933-103">networkmanagementcondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68933-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="68933-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68933-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68933-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68933-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68933-106">ネットワーク管理条件を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68933-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="68933-107">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="68933-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="68933-108">Methods</span></span>
|<span data-ttu-id="68933-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="68933-109">Method</span></span>|<span data-ttu-id="68933-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68933-110">Return Type</span></span>|<span data-ttu-id="68933-111">説明</span><span class="sxs-lookup"><span data-stu-id="68933-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68933-112">networkmanagementconditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="68933-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="68933-113">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68933-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="68933-114">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="68933-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="68933-115">networkmanagementcondition の取得</span><span class="sxs-lookup"><span data-stu-id="68933-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="68933-116">networkmanagementcondition</span><span class="sxs-lookup"><span data-stu-id="68933-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="68933-117">[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68933-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68933-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68933-118">Properties</span></span>
|<span data-ttu-id="68933-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68933-119">Property</span></span>|<span data-ttu-id="68933-120">型</span><span class="sxs-lookup"><span data-stu-id="68933-120">Type</span></span>|<span data-ttu-id="68933-121">説明</span><span class="sxs-lookup"><span data-stu-id="68933-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68933-122">id</span><span class="sxs-lookup"><span data-stu-id="68933-122">id</span></span>|<span data-ttu-id="68933-123">文字列</span><span class="sxs-lookup"><span data-stu-id="68933-123">String</span></span>|<span data-ttu-id="68933-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="68933-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="68933-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="68933-125">System generated value assigned when created.</span></span> <span data-ttu-id="68933-126">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="68933-127">uniqueName</span></span>|<span data-ttu-id="68933-128">文字列</span><span class="sxs-lookup"><span data-stu-id="68933-128">String</span></span>|<span data-ttu-id="68933-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="68933-129">Unique name for the management condition.</span></span> <span data-ttu-id="68933-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="68933-130">Used in management condition expressions.</span></span> <span data-ttu-id="68933-131">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-132">displayName</span><span class="sxs-lookup"><span data-stu-id="68933-132">displayName</span></span>|<span data-ttu-id="68933-133">String</span><span class="sxs-lookup"><span data-stu-id="68933-133">String</span></span>|<span data-ttu-id="68933-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="68933-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="68933-135">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-136">説明</span><span class="sxs-lookup"><span data-stu-id="68933-136">description</span></span>|<span data-ttu-id="68933-137">String</span><span class="sxs-lookup"><span data-stu-id="68933-137">String</span></span>|<span data-ttu-id="68933-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="68933-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="68933-139">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68933-140">createdDateTime</span></span>|<span data-ttu-id="68933-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68933-141">DateTimeOffset</span></span>|<span data-ttu-id="68933-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="68933-142">The time the management condition was created.</span></span> <span data-ttu-id="68933-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="68933-143">Generated service side.</span></span> <span data-ttu-id="68933-144">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68933-145">modifiedDateTime</span></span>|<span data-ttu-id="68933-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68933-146">DateTimeOffset</span></span>|<span data-ttu-id="68933-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="68933-147">The time the management condition was last modified.</span></span> <span data-ttu-id="68933-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="68933-148">Updated service side.</span></span> <span data-ttu-id="68933-149">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-150">eTag</span><span class="sxs-lookup"><span data-stu-id="68933-150">eTag</span></span>|<span data-ttu-id="68933-151">String</span><span class="sxs-lookup"><span data-stu-id="68933-151">String</span></span>|<span data-ttu-id="68933-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="68933-152">ETag of the management condition.</span></span> <span data-ttu-id="68933-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="68933-153">Updated service side.</span></span> <span data-ttu-id="68933-154">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="68933-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="68933-155">applicablePlatforms</span></span>|<span data-ttu-id="68933-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68933-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="68933-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="68933-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="68933-158">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="68933-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68933-159">Relationships</span></span>
|<span data-ttu-id="68933-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68933-160">Relationship</span></span>|<span data-ttu-id="68933-161">型</span><span class="sxs-lookup"><span data-stu-id="68933-161">Type</span></span>|<span data-ttu-id="68933-162">説明</span><span class="sxs-lookup"><span data-stu-id="68933-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68933-163">managementconditionstatements</span><span class="sxs-lookup"><span data-stu-id="68933-163">managementConditionStatements</span></span>|<span data-ttu-id="68933-164">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68933-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="68933-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="68933-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="68933-166">[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="68933-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68933-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68933-167">JSON Representation</span></span>
<span data-ttu-id="68933-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68933-168">Here is a JSON representation of the resource.</span></span>
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





