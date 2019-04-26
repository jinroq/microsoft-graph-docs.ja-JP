---
title: managementcondition リソースの種類
description: 管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b10442832d08507c3d33b71dd38928bc1be895d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568739"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="78e13-103">managementcondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78e13-103">managementCondition resource type</span></span>

> <span data-ttu-id="78e13-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78e13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e13-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78e13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e13-106">管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。</span><span class="sxs-lookup"><span data-stu-id="78e13-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="78e13-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e13-107">Methods</span></span>
|<span data-ttu-id="78e13-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e13-108">Method</span></span>|<span data-ttu-id="78e13-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78e13-109">Return Type</span></span>|<span data-ttu-id="78e13-110">説明</span><span class="sxs-lookup"><span data-stu-id="78e13-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78e13-111">managementconditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="78e13-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="78e13-112">[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78e13-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="78e13-113">[managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="78e13-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="78e13-114">managementcondition の取得</span><span class="sxs-lookup"><span data-stu-id="78e13-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="78e13-115">managementcondition</span><span class="sxs-lookup"><span data-stu-id="78e13-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="78e13-116">[managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="78e13-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="78e13-117">getmanagementconditionsforplatform 関数</span><span class="sxs-lookup"><span data-stu-id="78e13-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="78e13-118">[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78e13-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="78e13-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="78e13-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="78e13-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e13-120">Properties</span></span>
|<span data-ttu-id="78e13-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e13-121">Property</span></span>|<span data-ttu-id="78e13-122">型</span><span class="sxs-lookup"><span data-stu-id="78e13-122">Type</span></span>|<span data-ttu-id="78e13-123">説明</span><span class="sxs-lookup"><span data-stu-id="78e13-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e13-124">id</span><span class="sxs-lookup"><span data-stu-id="78e13-124">id</span></span>|<span data-ttu-id="78e13-125">String</span><span class="sxs-lookup"><span data-stu-id="78e13-125">String</span></span>|<span data-ttu-id="78e13-126">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="78e13-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="78e13-127">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="78e13-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="78e13-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="78e13-128">uniqueName</span></span>|<span data-ttu-id="78e13-129">String</span><span class="sxs-lookup"><span data-stu-id="78e13-129">String</span></span>|<span data-ttu-id="78e13-130">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="78e13-130">Unique name for the management condition.</span></span> <span data-ttu-id="78e13-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="78e13-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="78e13-132">displayName</span><span class="sxs-lookup"><span data-stu-id="78e13-132">displayName</span></span>|<span data-ttu-id="78e13-133">String</span><span class="sxs-lookup"><span data-stu-id="78e13-133">String</span></span>|<span data-ttu-id="78e13-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="78e13-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="78e13-135">説明</span><span class="sxs-lookup"><span data-stu-id="78e13-135">description</span></span>|<span data-ttu-id="78e13-136">String</span><span class="sxs-lookup"><span data-stu-id="78e13-136">String</span></span>|<span data-ttu-id="78e13-137">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="78e13-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="78e13-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78e13-138">createdDateTime</span></span>|<span data-ttu-id="78e13-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e13-139">DateTimeOffset</span></span>|<span data-ttu-id="78e13-140">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="78e13-140">The time the management condition was created.</span></span> <span data-ttu-id="78e13-141">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="78e13-141">Generated service side.</span></span>|
|<span data-ttu-id="78e13-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78e13-142">modifiedDateTime</span></span>|<span data-ttu-id="78e13-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e13-143">DateTimeOffset</span></span>|<span data-ttu-id="78e13-144">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="78e13-144">The time the management condition was last modified.</span></span> <span data-ttu-id="78e13-145">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="78e13-145">Updated service side.</span></span>|
|<span data-ttu-id="78e13-146">eTag</span><span class="sxs-lookup"><span data-stu-id="78e13-146">eTag</span></span>|<span data-ttu-id="78e13-147">String</span><span class="sxs-lookup"><span data-stu-id="78e13-147">String</span></span>|<span data-ttu-id="78e13-148">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="78e13-148">ETag of the management condition.</span></span> <span data-ttu-id="78e13-149">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="78e13-149">Updated service side.</span></span>|
|<span data-ttu-id="78e13-150">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="78e13-150">applicablePlatforms</span></span>|<span data-ttu-id="78e13-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78e13-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="78e13-152">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="78e13-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e13-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78e13-153">Relationships</span></span>
|<span data-ttu-id="78e13-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78e13-154">Relationship</span></span>|<span data-ttu-id="78e13-155">型</span><span class="sxs-lookup"><span data-stu-id="78e13-155">Type</span></span>|<span data-ttu-id="78e13-156">説明</span><span class="sxs-lookup"><span data-stu-id="78e13-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e13-157">managementconditionstatements</span><span class="sxs-lookup"><span data-stu-id="78e13-157">managementConditionStatements</span></span>|<span data-ttu-id="78e13-158">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78e13-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="78e13-159">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="78e13-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78e13-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78e13-160">JSON Representation</span></span>
<span data-ttu-id="78e13-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78e13-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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





