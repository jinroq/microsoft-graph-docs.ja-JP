---
title: groupPolicyConfiguration リソースの種類
description: グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 544b743ab690521fee48e3609e2c62582131d6ef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994245"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="a2f9e-103">groupPolicyConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2f9e-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="a2f9e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2f9e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2f9e-106">グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="a2f9e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2f9e-107">Methods</span></span>
|<span data-ttu-id="a2f9e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2f9e-108">Method</span></span>|<span data-ttu-id="a2f9e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2f9e-109">Return Type</span></span>|<span data-ttu-id="a2f9e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a2f9e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2f9e-111">GroupPolicyConfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2f9e-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="a2f9e-112">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2f9e-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="a2f9e-113">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a2f9e-114">GroupPolicyConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="a2f9e-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="a2f9e-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2f9e-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="a2f9e-116">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a2f9e-117">GroupPolicyConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a2f9e-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="a2f9e-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2f9e-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="a2f9e-119">新しい[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a2f9e-120">GroupPolicyConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="a2f9e-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="a2f9e-121">None</span><span class="sxs-lookup"><span data-stu-id="a2f9e-121">None</span></span>|<span data-ttu-id="a2f9e-122">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="a2f9e-123">GroupPolicyConfiguration を更新する</span><span class="sxs-lookup"><span data-stu-id="a2f9e-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="a2f9e-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2f9e-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="a2f9e-125">[Grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a2f9e-126">assign アクション</span><span class="sxs-lookup"><span data-stu-id="a2f9e-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="a2f9e-127">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2f9e-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a2f9e-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a2f9e-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a2f9e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f9e-129">Properties</span></span>
|<span data-ttu-id="a2f9e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f9e-130">Property</span></span>|<span data-ttu-id="a2f9e-131">型</span><span class="sxs-lookup"><span data-stu-id="a2f9e-131">Type</span></span>|<span data-ttu-id="a2f9e-132">説明</span><span class="sxs-lookup"><span data-stu-id="a2f9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f9e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f9e-133">createdDateTime</span></span>|<span data-ttu-id="a2f9e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f9e-134">DateTimeOffset</span></span>|<span data-ttu-id="a2f9e-135">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="a2f9e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a2f9e-136">displayName</span></span>|<span data-ttu-id="a2f9e-137">String</span><span class="sxs-lookup"><span data-stu-id="a2f9e-137">String</span></span>|<span data-ttu-id="a2f9e-138">ユーザーが指定した resource オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="a2f9e-139">description</span><span class="sxs-lookup"><span data-stu-id="a2f9e-139">description</span></span>|<span data-ttu-id="a2f9e-140">String</span><span class="sxs-lookup"><span data-stu-id="a2f9e-140">String</span></span>|<span data-ttu-id="a2f9e-141">ユーザーが指定した resource オブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="a2f9e-142">id</span><span class="sxs-lookup"><span data-stu-id="a2f9e-142">id</span></span>|<span data-ttu-id="a2f9e-143">文字列</span><span class="sxs-lookup"><span data-stu-id="a2f9e-143">String</span></span>|<span data-ttu-id="a2f9e-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-144">Key of the entity.</span></span>|
|<span data-ttu-id="a2f9e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f9e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="a2f9e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f9e-146">DateTimeOffset</span></span>|<span data-ttu-id="a2f9e-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2f9e-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2f9e-148">Relationships</span></span>
|<span data-ttu-id="a2f9e-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2f9e-149">Relationship</span></span>|<span data-ttu-id="a2f9e-150">型</span><span class="sxs-lookup"><span data-stu-id="a2f9e-150">Type</span></span>|<span data-ttu-id="a2f9e-151">説明</span><span class="sxs-lookup"><span data-stu-id="a2f9e-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f9e-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="a2f9e-152">definitionValues</span></span>|<span data-ttu-id="a2f9e-153">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2f9e-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="a2f9e-154">構成に対して有効または無効にされたグループポリシー定義の値のリスト。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="a2f9e-155">assignments</span><span class="sxs-lookup"><span data-stu-id="a2f9e-155">assignments</span></span>|<span data-ttu-id="a2f9e-156">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2f9e-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a2f9e-157">構成のグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2f9e-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2f9e-158">JSON Representation</span></span>
<span data-ttu-id="a2f9e-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2f9e-159">Here is a JSON representation of the resource.</span></span>
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





