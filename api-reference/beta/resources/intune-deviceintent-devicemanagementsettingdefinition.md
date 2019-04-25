---
title: devicemanagementsettingdefinition リソースの種類
description: 指定した設定の定義を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2e06522680085502e3007dd4863bd703c4bed44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550547"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a><span data-ttu-id="37944-103">devicemanagementsettingdefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37944-103">deviceManagementSettingDefinition resource type</span></span>

> <span data-ttu-id="37944-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37944-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37944-106">指定した設定の定義を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="37944-106">Entity representing the defintion for a given setting</span></span>

## <a name="methods"></a><span data-ttu-id="37944-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="37944-107">Methods</span></span>
|<span data-ttu-id="37944-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="37944-108">Method</span></span>|<span data-ttu-id="37944-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="37944-109">Return Type</span></span>|<span data-ttu-id="37944-110">説明</span><span class="sxs-lookup"><span data-stu-id="37944-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37944-111">devicemanagementsettingdefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="37944-111">List deviceManagementSettingDefinitions</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|<span data-ttu-id="37944-112">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37944-112">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="37944-113">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="37944-113">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>|
|[<span data-ttu-id="37944-114">devicemanagementsettingdefinition の取得</span><span class="sxs-lookup"><span data-stu-id="37944-114">Get deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[<span data-ttu-id="37944-115">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="37944-115">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="37944-116">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="37944-116">Read properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|
|[<span data-ttu-id="37944-117">devicemanagementsettingdefinition の作成</span><span class="sxs-lookup"><span data-stu-id="37944-117">Create deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[<span data-ttu-id="37944-118">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="37944-118">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="37944-119">新しい[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="37944-119">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|
|[<span data-ttu-id="37944-120">devicemanagementsettingdefinition の削除</span><span class="sxs-lookup"><span data-stu-id="37944-120">Delete deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|<span data-ttu-id="37944-121">なし</span><span class="sxs-lookup"><span data-stu-id="37944-121">None</span></span>|<span data-ttu-id="37944-122">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="37944-122">Deletes a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>|
|[<span data-ttu-id="37944-123">devicemanagementsettingdefinition の更新</span><span class="sxs-lookup"><span data-stu-id="37944-123">Update deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[<span data-ttu-id="37944-124">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="37944-124">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="37944-125">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="37944-125">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37944-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37944-126">Properties</span></span>
|<span data-ttu-id="37944-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37944-127">Property</span></span>|<span data-ttu-id="37944-128">型</span><span class="sxs-lookup"><span data-stu-id="37944-128">Type</span></span>|<span data-ttu-id="37944-129">説明</span><span class="sxs-lookup"><span data-stu-id="37944-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37944-130">id</span><span class="sxs-lookup"><span data-stu-id="37944-130">id</span></span>|<span data-ttu-id="37944-131">String</span><span class="sxs-lookup"><span data-stu-id="37944-131">String</span></span>|<span data-ttu-id="37944-132">設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="37944-132">The ID of the setting definition</span></span>|
|<span data-ttu-id="37944-133">valueType</span><span class="sxs-lookup"><span data-stu-id="37944-133">valueType</span></span>|[<span data-ttu-id="37944-134">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="37944-134">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="37944-135">値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="37944-135">The data type of the value.</span></span> <span data-ttu-id="37944-136">可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。</span><span class="sxs-lookup"><span data-stu-id="37944-136">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="37944-137">displayName</span><span class="sxs-lookup"><span data-stu-id="37944-137">displayName</span></span>|<span data-ttu-id="37944-138">String</span><span class="sxs-lookup"><span data-stu-id="37944-138">String</span></span>|<span data-ttu-id="37944-139">設定の表示名</span><span class="sxs-lookup"><span data-stu-id="37944-139">The setting's display name</span></span>|
|<span data-ttu-id="37944-140">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="37944-140">isTopLevel</span></span>|<span data-ttu-id="37944-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="37944-141">Boolean</span></span>|<span data-ttu-id="37944-142">設定が最上位レベルの場合は、コレクションまたは複雑な設定でラップする必要がなく構成できます。</span><span class="sxs-lookup"><span data-stu-id="37944-142">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="37944-143">description</span><span class="sxs-lookup"><span data-stu-id="37944-143">description</span></span>|<span data-ttu-id="37944-144">String</span><span class="sxs-lookup"><span data-stu-id="37944-144">String</span></span>|<span data-ttu-id="37944-145">設定の説明</span><span class="sxs-lookup"><span data-stu-id="37944-145">The setting's description</span></span>|
|<span data-ttu-id="37944-146">documentation url</span><span class="sxs-lookup"><span data-stu-id="37944-146">documentationUrl</span></span>|<span data-ttu-id="37944-147">String</span><span class="sxs-lookup"><span data-stu-id="37944-147">String</span></span>|<span data-ttu-id="37944-148">ドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="37944-148">Url to setting documentation</span></span>|
|<span data-ttu-id="37944-149">keywords</span><span class="sxs-lookup"><span data-stu-id="37944-149">keywords</span></span>|<span data-ttu-id="37944-150">String collection</span><span class="sxs-lookup"><span data-stu-id="37944-150">String collection</span></span>|<span data-ttu-id="37944-151">設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="37944-151">Keywords associated with the setting</span></span>|
|<span data-ttu-id="37944-152">式</span><span class="sxs-lookup"><span data-stu-id="37944-152">constraints</span></span>|<span data-ttu-id="37944-153">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37944-153">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="37944-154">設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="37944-154">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="37944-155">ヲ</span><span class="sxs-lookup"><span data-stu-id="37944-155">dependencies</span></span>|<span data-ttu-id="37944-156">[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37944-156">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="37944-157">他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="37944-157">Collection of dependencies on other settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="37944-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37944-158">Relationships</span></span>
<span data-ttu-id="37944-159">なし</span><span class="sxs-lookup"><span data-stu-id="37944-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37944-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37944-160">JSON Representation</span></span>
<span data-ttu-id="37944-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37944-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```





