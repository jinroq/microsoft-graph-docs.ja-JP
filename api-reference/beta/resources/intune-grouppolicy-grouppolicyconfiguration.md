---
title: grouppolicyconfiguration リソースの種類
description: グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c925ba10b1dde26e51a64b912c33143d58def3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774443"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="df5a9-103">grouppolicyconfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df5a9-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="df5a9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df5a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df5a9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df5a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df5a9-106">グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="df5a9-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="df5a9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="df5a9-107">Methods</span></span>
|<span data-ttu-id="df5a9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="df5a9-108">Method</span></span>|<span data-ttu-id="df5a9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="df5a9-109">Return Type</span></span>|<span data-ttu-id="df5a9-110">説明</span><span class="sxs-lookup"><span data-stu-id="df5a9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df5a9-111">grouppolicyconfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="df5a9-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="df5a9-112">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="df5a9-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="df5a9-113">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="df5a9-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="df5a9-114">grouppolicyconfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="df5a9-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="df5a9-115">grouppolicyconfiguration</span><span class="sxs-lookup"><span data-stu-id="df5a9-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="df5a9-116">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="df5a9-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="df5a9-117">grouppolicyconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="df5a9-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="df5a9-118">grouppolicyconfiguration</span><span class="sxs-lookup"><span data-stu-id="df5a9-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="df5a9-119">新しい[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="df5a9-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="df5a9-120">grouppolicyconfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="df5a9-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="df5a9-121">なし</span><span class="sxs-lookup"><span data-stu-id="df5a9-121">None</span></span>|<span data-ttu-id="df5a9-122">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="df5a9-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="df5a9-123">grouppolicyconfiguration を更新する</span><span class="sxs-lookup"><span data-stu-id="df5a9-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="df5a9-124">grouppolicyconfiguration</span><span class="sxs-lookup"><span data-stu-id="df5a9-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="df5a9-125">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="df5a9-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="df5a9-126">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="df5a9-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="df5a9-127">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="df5a9-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="df5a9-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="df5a9-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="df5a9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df5a9-129">Properties</span></span>
|<span data-ttu-id="df5a9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df5a9-130">Property</span></span>|<span data-ttu-id="df5a9-131">型</span><span class="sxs-lookup"><span data-stu-id="df5a9-131">Type</span></span>|<span data-ttu-id="df5a9-132">説明</span><span class="sxs-lookup"><span data-stu-id="df5a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5a9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df5a9-133">createdDateTime</span></span>|<span data-ttu-id="df5a9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df5a9-134">DateTimeOffset</span></span>|<span data-ttu-id="df5a9-135">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="df5a9-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="df5a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="df5a9-136">displayName</span></span>|<span data-ttu-id="df5a9-137">String</span><span class="sxs-lookup"><span data-stu-id="df5a9-137">String</span></span>|<span data-ttu-id="df5a9-138">ユーザーが指定した resource オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="df5a9-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="df5a9-139">説明</span><span class="sxs-lookup"><span data-stu-id="df5a9-139">description</span></span>|<span data-ttu-id="df5a9-140">String</span><span class="sxs-lookup"><span data-stu-id="df5a9-140">String</span></span>|<span data-ttu-id="df5a9-141">ユーザーが指定した resource オブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="df5a9-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="df5a9-142">id</span><span class="sxs-lookup"><span data-stu-id="df5a9-142">id</span></span>|<span data-ttu-id="df5a9-143">String</span><span class="sxs-lookup"><span data-stu-id="df5a9-143">String</span></span>|<span data-ttu-id="df5a9-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="df5a9-144">Key of the entity.</span></span>|
|<span data-ttu-id="df5a9-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df5a9-145">lastModifiedDateTime</span></span>|<span data-ttu-id="df5a9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df5a9-146">DateTimeOffset</span></span>|<span data-ttu-id="df5a9-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="df5a9-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df5a9-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df5a9-148">Relationships</span></span>
|<span data-ttu-id="df5a9-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df5a9-149">Relationship</span></span>|<span data-ttu-id="df5a9-150">型</span><span class="sxs-lookup"><span data-stu-id="df5a9-150">Type</span></span>|<span data-ttu-id="df5a9-151">説明</span><span class="sxs-lookup"><span data-stu-id="df5a9-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5a9-152">definitionvalues</span><span class="sxs-lookup"><span data-stu-id="df5a9-152">definitionValues</span></span>|<span data-ttu-id="df5a9-153">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="df5a9-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="df5a9-154">構成に対して有効または無効にされたグループポリシー定義の値のリスト。</span><span class="sxs-lookup"><span data-stu-id="df5a9-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="df5a9-155">assignments</span><span class="sxs-lookup"><span data-stu-id="df5a9-155">assignments</span></span>|<span data-ttu-id="df5a9-156">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="df5a9-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="df5a9-157">構成のグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="df5a9-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df5a9-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df5a9-158">JSON Representation</span></span>
<span data-ttu-id="df5a9-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df5a9-159">Here is a JSON representation of the resource.</span></span>
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





