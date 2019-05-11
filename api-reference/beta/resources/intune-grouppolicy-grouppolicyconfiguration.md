---
title: groupPolicyConfiguration リソースの種類
description: グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d910bf8bdef34c60ca6bb66e1ce87ca9cf1d51ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941178"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="0fc1a-103">groupPolicyConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fc1a-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="0fc1a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fc1a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fc1a-106">グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="0fc1a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fc1a-107">Methods</span></span>
|<span data-ttu-id="0fc1a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fc1a-108">Method</span></span>|<span data-ttu-id="0fc1a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0fc1a-109">Return Type</span></span>|<span data-ttu-id="0fc1a-110">説明</span><span class="sxs-lookup"><span data-stu-id="0fc1a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fc1a-111">GroupPolicyConfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0fc1a-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="0fc1a-112">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fc1a-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="0fc1a-113">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0fc1a-114">GroupPolicyConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="0fc1a-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="0fc1a-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fc1a-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0fc1a-116">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0fc1a-117">GroupPolicyConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="0fc1a-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="0fc1a-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fc1a-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0fc1a-119">新しい[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0fc1a-120">GroupPolicyConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="0fc1a-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="0fc1a-121">None</span><span class="sxs-lookup"><span data-stu-id="0fc1a-121">None</span></span>|<span data-ttu-id="0fc1a-122">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="0fc1a-123">GroupPolicyConfiguration を更新する</span><span class="sxs-lookup"><span data-stu-id="0fc1a-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="0fc1a-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fc1a-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0fc1a-125">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0fc1a-126">assign アクション</span><span class="sxs-lookup"><span data-stu-id="0fc1a-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="0fc1a-127">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fc1a-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0fc1a-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0fc1a-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0fc1a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fc1a-129">Properties</span></span>
|<span data-ttu-id="0fc1a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fc1a-130">Property</span></span>|<span data-ttu-id="0fc1a-131">種類</span><span class="sxs-lookup"><span data-stu-id="0fc1a-131">Type</span></span>|<span data-ttu-id="0fc1a-132">説明</span><span class="sxs-lookup"><span data-stu-id="0fc1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc1a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc1a-133">createdDateTime</span></span>|<span data-ttu-id="0fc1a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc1a-134">DateTimeOffset</span></span>|<span data-ttu-id="0fc1a-135">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="0fc1a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0fc1a-136">displayName</span></span>|<span data-ttu-id="0fc1a-137">String</span><span class="sxs-lookup"><span data-stu-id="0fc1a-137">String</span></span>|<span data-ttu-id="0fc1a-138">ユーザーが指定した resource オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="0fc1a-139">description</span><span class="sxs-lookup"><span data-stu-id="0fc1a-139">description</span></span>|<span data-ttu-id="0fc1a-140">String</span><span class="sxs-lookup"><span data-stu-id="0fc1a-140">String</span></span>|<span data-ttu-id="0fc1a-141">ユーザーが指定した resource オブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="0fc1a-142">id</span><span class="sxs-lookup"><span data-stu-id="0fc1a-142">id</span></span>|<span data-ttu-id="0fc1a-143">文字列</span><span class="sxs-lookup"><span data-stu-id="0fc1a-143">String</span></span>|<span data-ttu-id="0fc1a-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-144">Key of the entity.</span></span>|
|<span data-ttu-id="0fc1a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc1a-145">lastModifiedDateTime</span></span>|<span data-ttu-id="0fc1a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc1a-146">DateTimeOffset</span></span>|<span data-ttu-id="0fc1a-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fc1a-148">関係</span><span class="sxs-lookup"><span data-stu-id="0fc1a-148">Relationships</span></span>
|<span data-ttu-id="0fc1a-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0fc1a-149">Relationship</span></span>|<span data-ttu-id="0fc1a-150">型</span><span class="sxs-lookup"><span data-stu-id="0fc1a-150">Type</span></span>|<span data-ttu-id="0fc1a-151">説明</span><span class="sxs-lookup"><span data-stu-id="0fc1a-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc1a-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="0fc1a-152">definitionValues</span></span>|<span data-ttu-id="0fc1a-153">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fc1a-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="0fc1a-154">構成に対して有効または無効にされたグループポリシー定義の値のリスト。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="0fc1a-155">assignments</span><span class="sxs-lookup"><span data-stu-id="0fc1a-155">assignments</span></span>|<span data-ttu-id="0fc1a-156">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fc1a-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0fc1a-157">構成のグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fc1a-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fc1a-158">JSON Representation</span></span>
<span data-ttu-id="0fc1a-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fc1a-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




