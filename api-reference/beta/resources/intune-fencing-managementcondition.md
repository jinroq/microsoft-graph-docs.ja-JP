---
title: managementCondition リソースの種類
description: 管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 582af8906fe9948b87a5526ca53a1c2592a0d083
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331687"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="1ee0e-103">managementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ee0e-103">managementCondition resource type</span></span>

> <span data-ttu-id="1ee0e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ee0e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee0e-106">管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="1ee0e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ee0e-107">Methods</span></span>
|<span data-ttu-id="1ee0e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ee0e-108">Method</span></span>|<span data-ttu-id="1ee0e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1ee0e-109">Return Type</span></span>|<span data-ttu-id="1ee0e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1ee0e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ee0e-111">ManagementConditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1ee0e-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="1ee0e-112">[Managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ee0e-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1ee0e-113">[Managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1ee0e-114">ManagementCondition の取得</span><span class="sxs-lookup"><span data-stu-id="1ee0e-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="1ee0e-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="1ee0e-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="1ee0e-116">[Managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="1ee0e-117">getManagementConditionsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="1ee0e-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="1ee0e-118">[Managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ee0e-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1ee0e-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1ee0e-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1ee0e-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ee0e-120">Properties</span></span>
|<span data-ttu-id="1ee0e-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ee0e-121">Property</span></span>|<span data-ttu-id="1ee0e-122">型</span><span class="sxs-lookup"><span data-stu-id="1ee0e-122">Type</span></span>|<span data-ttu-id="1ee0e-123">説明</span><span class="sxs-lookup"><span data-stu-id="1ee0e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee0e-124">id</span><span class="sxs-lookup"><span data-stu-id="1ee0e-124">id</span></span>|<span data-ttu-id="1ee0e-125">文字列</span><span class="sxs-lookup"><span data-stu-id="1ee0e-125">String</span></span>|<span data-ttu-id="1ee0e-126">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="1ee0e-127">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1ee0e-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1ee0e-128">uniqueName</span></span>|<span data-ttu-id="1ee0e-129">String</span><span class="sxs-lookup"><span data-stu-id="1ee0e-129">String</span></span>|<span data-ttu-id="1ee0e-130">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-130">Unique name for the management condition.</span></span> <span data-ttu-id="1ee0e-131">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="1ee0e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1ee0e-132">displayName</span></span>|<span data-ttu-id="1ee0e-133">String</span><span class="sxs-lookup"><span data-stu-id="1ee0e-133">String</span></span>|<span data-ttu-id="1ee0e-134">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="1ee0e-135">description</span><span class="sxs-lookup"><span data-stu-id="1ee0e-135">description</span></span>|<span data-ttu-id="1ee0e-136">String</span><span class="sxs-lookup"><span data-stu-id="1ee0e-136">String</span></span>|<span data-ttu-id="1ee0e-137">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="1ee0e-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ee0e-138">createdDateTime</span></span>|<span data-ttu-id="1ee0e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ee0e-139">DateTimeOffset</span></span>|<span data-ttu-id="1ee0e-140">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-140">The time the management condition was created.</span></span> <span data-ttu-id="1ee0e-141">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-141">Generated service side.</span></span>|
|<span data-ttu-id="1ee0e-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ee0e-142">modifiedDateTime</span></span>|<span data-ttu-id="1ee0e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ee0e-143">DateTimeOffset</span></span>|<span data-ttu-id="1ee0e-144">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-144">The time the management condition was last modified.</span></span> <span data-ttu-id="1ee0e-145">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-145">Updated service side.</span></span>|
|<span data-ttu-id="1ee0e-146">eTag</span><span class="sxs-lookup"><span data-stu-id="1ee0e-146">eTag</span></span>|<span data-ttu-id="1ee0e-147">String</span><span class="sxs-lookup"><span data-stu-id="1ee0e-147">String</span></span>|<span data-ttu-id="1ee0e-148">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-148">ETag of the management condition.</span></span> <span data-ttu-id="1ee0e-149">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-149">Updated service side.</span></span>|
|<span data-ttu-id="1ee0e-150">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="1ee0e-150">applicablePlatforms</span></span>|<span data-ttu-id="1ee0e-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ee0e-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1ee0e-152">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ee0e-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ee0e-153">Relationships</span></span>
|<span data-ttu-id="1ee0e-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ee0e-154">Relationship</span></span>|<span data-ttu-id="1ee0e-155">型</span><span class="sxs-lookup"><span data-stu-id="1ee0e-155">Type</span></span>|<span data-ttu-id="1ee0e-156">説明</span><span class="sxs-lookup"><span data-stu-id="1ee0e-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee0e-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="1ee0e-157">managementConditionStatements</span></span>|<span data-ttu-id="1ee0e-158">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ee0e-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1ee0e-159">管理条件に関連付けられている管理条件ステートメント。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ee0e-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ee0e-160">JSON Representation</span></span>
<span data-ttu-id="1ee0e-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ee0e-161">Here is a JSON representation of the resource.</span></span>
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



