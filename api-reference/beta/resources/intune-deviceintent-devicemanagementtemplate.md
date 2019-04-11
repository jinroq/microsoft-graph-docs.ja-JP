---
title: devicemanagementtemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a55e4426f37f0261f5adbd1ac4830de6ede3e3ed
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801877"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="fe83f-103">devicemanagementtemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe83f-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="fe83f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe83f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe83f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe83f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe83f-106">デバイス設定の定義済みコレクションを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="fe83f-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="fe83f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe83f-107">Methods</span></span>
|<span data-ttu-id="fe83f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe83f-108">Method</span></span>|<span data-ttu-id="fe83f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe83f-109">Return Type</span></span>|<span data-ttu-id="fe83f-110">説明</span><span class="sxs-lookup"><span data-stu-id="fe83f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe83f-111">devicemanagementtemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fe83f-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="fe83f-112">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="fe83f-113">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fe83f-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="fe83f-114">devicemanagementtemplate の取得</span><span class="sxs-lookup"><span data-stu-id="fe83f-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="fe83f-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="fe83f-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="fe83f-116">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fe83f-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="fe83f-117">devicemanagementtemplate の作成</span><span class="sxs-lookup"><span data-stu-id="fe83f-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="fe83f-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="fe83f-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="fe83f-119">新しい[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe83f-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="fe83f-120">devicemanagementtemplate の削除</span><span class="sxs-lookup"><span data-stu-id="fe83f-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="fe83f-121">なし</span><span class="sxs-lookup"><span data-stu-id="fe83f-121">None</span></span>|<span data-ttu-id="fe83f-122">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="fe83f-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="fe83f-123">devicemanagementtemplate の更新</span><span class="sxs-lookup"><span data-stu-id="fe83f-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="fe83f-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="fe83f-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="fe83f-125">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe83f-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="fe83f-126">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="fe83f-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="fe83f-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="fe83f-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fe83f-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fe83f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe83f-129">Properties</span></span>
|<span data-ttu-id="fe83f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe83f-130">Property</span></span>|<span data-ttu-id="fe83f-131">型</span><span class="sxs-lookup"><span data-stu-id="fe83f-131">Type</span></span>|<span data-ttu-id="fe83f-132">説明</span><span class="sxs-lookup"><span data-stu-id="fe83f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe83f-133">id</span><span class="sxs-lookup"><span data-stu-id="fe83f-133">id</span></span>|<span data-ttu-id="fe83f-134">文字列</span><span class="sxs-lookup"><span data-stu-id="fe83f-134">String</span></span>|<span data-ttu-id="fe83f-135">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="fe83f-135">The template ID</span></span>|
|<span data-ttu-id="fe83f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fe83f-136">displayName</span></span>|<span data-ttu-id="fe83f-137">String</span><span class="sxs-lookup"><span data-stu-id="fe83f-137">String</span></span>|<span data-ttu-id="fe83f-138">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="fe83f-138">The template's display name</span></span>|
|<span data-ttu-id="fe83f-139">説明</span><span class="sxs-lookup"><span data-stu-id="fe83f-139">description</span></span>|<span data-ttu-id="fe83f-140">String</span><span class="sxs-lookup"><span data-stu-id="fe83f-140">String</span></span>|<span data-ttu-id="fe83f-141">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="fe83f-141">The template's description</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe83f-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe83f-142">Relationships</span></span>
|<span data-ttu-id="fe83f-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe83f-143">Relationship</span></span>|<span data-ttu-id="fe83f-144">型</span><span class="sxs-lookup"><span data-stu-id="fe83f-144">Type</span></span>|<span data-ttu-id="fe83f-145">説明</span><span class="sxs-lookup"><span data-stu-id="fe83f-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe83f-146">settings</span><span class="sxs-lookup"><span data-stu-id="fe83f-146">settings</span></span>|<span data-ttu-id="fe83f-147">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-147">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="fe83f-148">このテンプレートに含まれるすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-148">Collection of all settings this template has</span></span>|
|<span data-ttu-id="fe83f-149">categories</span><span class="sxs-lookup"><span data-stu-id="fe83f-149">categories</span></span>|<span data-ttu-id="fe83f-150">[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-150">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="fe83f-151">テンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="fe83f-151">Collection of setting categories within the template</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe83f-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe83f-152">JSON Representation</span></span>
<span data-ttu-id="fe83f-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe83f-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





