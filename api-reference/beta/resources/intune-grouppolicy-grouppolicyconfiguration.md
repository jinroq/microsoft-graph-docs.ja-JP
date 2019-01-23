---
title: groupPolicyConfiguration リソースの種類
description: グループ ポリシーの構成エンティティには、1 つまたは複数のグループ ポリシーの定義の設定値が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431665"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="051df-103">groupPolicyConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="051df-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="051df-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="051df-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="051df-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="051df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="051df-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="051df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="051df-107">グループ ポリシーの構成エンティティには、1 つまたは複数のグループ ポリシーの定義の設定値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="051df-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="051df-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="051df-108">Methods</span></span>
|<span data-ttu-id="051df-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="051df-109">Method</span></span>|<span data-ttu-id="051df-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="051df-110">Return Type</span></span>|<span data-ttu-id="051df-111">説明</span><span class="sxs-lookup"><span data-stu-id="051df-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="051df-112">リスト groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="051df-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="051df-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="051df-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="051df-114">[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="051df-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="051df-115">GroupPolicyConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="051df-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="051df-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="051df-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="051df-117">[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="051df-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="051df-118">GroupPolicyConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="051df-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="051df-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="051df-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="051df-120">新しい[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="051df-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="051df-121">GroupPolicyConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="051df-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="051df-122">なし</span><span class="sxs-lookup"><span data-stu-id="051df-122">None</span></span>|<span data-ttu-id="051df-123">の[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="051df-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="051df-124">GroupPolicyConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="051df-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="051df-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="051df-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="051df-126">[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="051df-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="051df-127">assign action</span><span class="sxs-lookup"><span data-stu-id="051df-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="051df-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="051df-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="051df-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="051df-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="051df-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="051df-130">Properties</span></span>
|<span data-ttu-id="051df-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="051df-131">Property</span></span>|<span data-ttu-id="051df-132">型</span><span class="sxs-lookup"><span data-stu-id="051df-132">Type</span></span>|<span data-ttu-id="051df-133">説明</span><span class="sxs-lookup"><span data-stu-id="051df-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="051df-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="051df-134">createdDateTime</span></span>|<span data-ttu-id="051df-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="051df-135">DateTimeOffset</span></span>|<span data-ttu-id="051df-136">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="051df-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="051df-137">displayName</span><span class="sxs-lookup"><span data-stu-id="051df-137">displayName</span></span>|<span data-ttu-id="051df-138">String</span><span class="sxs-lookup"><span data-stu-id="051df-138">String</span></span>|<span data-ttu-id="051df-139">リソース オブジェクトの名前をユーザーに提供されます。</span><span class="sxs-lookup"><span data-stu-id="051df-139">User provided name for the resource object.</span></span>|
|<span data-ttu-id="051df-140">説明</span><span class="sxs-lookup"><span data-stu-id="051df-140">description</span></span>|<span data-ttu-id="051df-141">String</span><span class="sxs-lookup"><span data-stu-id="051df-141">String</span></span>|<span data-ttu-id="051df-142">ユーザーは、リソース オブジェクトの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="051df-142">User provided description for the resource object.</span></span>|
|<span data-ttu-id="051df-143">id</span><span class="sxs-lookup"><span data-stu-id="051df-143">id</span></span>|<span data-ttu-id="051df-144">String</span><span class="sxs-lookup"><span data-stu-id="051df-144">String</span></span>|<span data-ttu-id="051df-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="051df-145">Key of the entity.</span></span>|
|<span data-ttu-id="051df-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="051df-146">lastModifiedDateTime</span></span>|<span data-ttu-id="051df-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="051df-147">DateTimeOffset</span></span>|<span data-ttu-id="051df-148">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="051df-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="051df-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="051df-149">Relationships</span></span>
|<span data-ttu-id="051df-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="051df-150">Relationship</span></span>|<span data-ttu-id="051df-151">型</span><span class="sxs-lookup"><span data-stu-id="051df-151">Type</span></span>|<span data-ttu-id="051df-152">説明</span><span class="sxs-lookup"><span data-stu-id="051df-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="051df-153">definitionValues</span><span class="sxs-lookup"><span data-stu-id="051df-153">definitionValues</span></span>|<span data-ttu-id="051df-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="051df-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="051df-155">一覧は、有効または、構成のグループ ポリシーの定義の値を無効にします。</span><span class="sxs-lookup"><span data-stu-id="051df-155">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="051df-156">assignments</span><span class="sxs-lookup"><span data-stu-id="051df-156">assignments</span></span>|<span data-ttu-id="051df-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="051df-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="051df-158">構成のグループの割り当ての一覧です。</span><span class="sxs-lookup"><span data-stu-id="051df-158">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="051df-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="051df-159">JSON Representation</span></span>
<span data-ttu-id="051df-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="051df-160">Here is a JSON representation of the resource.</span></span>
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




