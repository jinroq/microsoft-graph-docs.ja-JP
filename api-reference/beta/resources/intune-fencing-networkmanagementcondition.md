---
title: networkManagementCondition リソースの種類
description: ネットワーク管理条件を定義するための情報が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7328f061ab459fd02c088e403c7c46a3bc827c60
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331589"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="651db-103">networkManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="651db-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="651db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="651db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="651db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="651db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="651db-106">ネットワーク管理条件を定義するための情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="651db-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="651db-107">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="651db-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="651db-108">Methods</span></span>
|<span data-ttu-id="651db-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="651db-109">Method</span></span>|<span data-ttu-id="651db-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="651db-110">Return Type</span></span>|<span data-ttu-id="651db-111">説明</span><span class="sxs-lookup"><span data-stu-id="651db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="651db-112">NetworkManagementConditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="651db-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="651db-113">[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="651db-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="651db-114">[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="651db-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="651db-115">NetworkManagementCondition の取得</span><span class="sxs-lookup"><span data-stu-id="651db-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="651db-116">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="651db-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="651db-117">[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="651db-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="651db-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="651db-118">Properties</span></span>
|<span data-ttu-id="651db-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="651db-119">Property</span></span>|<span data-ttu-id="651db-120">型</span><span class="sxs-lookup"><span data-stu-id="651db-120">Type</span></span>|<span data-ttu-id="651db-121">説明</span><span class="sxs-lookup"><span data-stu-id="651db-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="651db-122">id</span><span class="sxs-lookup"><span data-stu-id="651db-122">id</span></span>|<span data-ttu-id="651db-123">文字列</span><span class="sxs-lookup"><span data-stu-id="651db-123">String</span></span>|<span data-ttu-id="651db-124">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="651db-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="651db-125">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="651db-125">System generated value assigned when created.</span></span> <span data-ttu-id="651db-126">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="651db-127">uniqueName</span></span>|<span data-ttu-id="651db-128">String</span><span class="sxs-lookup"><span data-stu-id="651db-128">String</span></span>|<span data-ttu-id="651db-129">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="651db-129">Unique name for the management condition.</span></span> <span data-ttu-id="651db-130">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="651db-130">Used in management condition expressions.</span></span> <span data-ttu-id="651db-131">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-132">displayName</span><span class="sxs-lookup"><span data-stu-id="651db-132">displayName</span></span>|<span data-ttu-id="651db-133">String</span><span class="sxs-lookup"><span data-stu-id="651db-133">String</span></span>|<span data-ttu-id="651db-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="651db-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="651db-135">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-136">description</span><span class="sxs-lookup"><span data-stu-id="651db-136">description</span></span>|<span data-ttu-id="651db-137">String</span><span class="sxs-lookup"><span data-stu-id="651db-137">String</span></span>|<span data-ttu-id="651db-138">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="651db-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="651db-139">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="651db-140">createdDateTime</span></span>|<span data-ttu-id="651db-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="651db-141">DateTimeOffset</span></span>|<span data-ttu-id="651db-142">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="651db-142">The time the management condition was created.</span></span> <span data-ttu-id="651db-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="651db-143">Generated service side.</span></span> <span data-ttu-id="651db-144">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="651db-145">modifiedDateTime</span></span>|<span data-ttu-id="651db-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="651db-146">DateTimeOffset</span></span>|<span data-ttu-id="651db-147">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="651db-147">The time the management condition was last modified.</span></span> <span data-ttu-id="651db-148">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="651db-148">Updated service side.</span></span> <span data-ttu-id="651db-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-150">eTag</span><span class="sxs-lookup"><span data-stu-id="651db-150">eTag</span></span>|<span data-ttu-id="651db-151">String</span><span class="sxs-lookup"><span data-stu-id="651db-151">String</span></span>|<span data-ttu-id="651db-152">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="651db-152">ETag of the management condition.</span></span> <span data-ttu-id="651db-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="651db-153">Updated service side.</span></span> <span data-ttu-id="651db-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="651db-155">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="651db-155">applicablePlatforms</span></span>|<span data-ttu-id="651db-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="651db-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="651db-157">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="651db-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="651db-158">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="651db-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="651db-159">Relationships</span></span>
|<span data-ttu-id="651db-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="651db-160">Relationship</span></span>|<span data-ttu-id="651db-161">型</span><span class="sxs-lookup"><span data-stu-id="651db-161">Type</span></span>|<span data-ttu-id="651db-162">説明</span><span class="sxs-lookup"><span data-stu-id="651db-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="651db-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="651db-163">managementConditionStatements</span></span>|<span data-ttu-id="651db-164">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="651db-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="651db-165">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="651db-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="651db-166">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="651db-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="651db-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="651db-167">JSON Representation</span></span>
<span data-ttu-id="651db-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="651db-168">Here is a JSON representation of the resource.</span></span>
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



