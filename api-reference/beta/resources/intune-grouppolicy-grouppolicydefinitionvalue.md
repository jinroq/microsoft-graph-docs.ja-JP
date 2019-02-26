---
title: grouppolicydefinitionvalue リソースの種類
description: 定義値エンティティは、1つのグループポリシー定義の値を格納します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e822cb4ce46a0fa9492f7624904588fd1b10a7c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142617"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="67274-103">grouppolicydefinitionvalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67274-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="67274-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67274-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67274-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67274-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67274-106">定義値エンティティは、1つのグループポリシー定義の値を格納します。</span><span class="sxs-lookup"><span data-stu-id="67274-106">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="67274-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="67274-107">Methods</span></span>
|<span data-ttu-id="67274-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="67274-108">Method</span></span>|<span data-ttu-id="67274-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67274-109">Return Type</span></span>|<span data-ttu-id="67274-110">説明</span><span class="sxs-lookup"><span data-stu-id="67274-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67274-111">grouppolicydefinitionvalues のリスト</span><span class="sxs-lookup"><span data-stu-id="67274-111">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="67274-112">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="67274-112">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="67274-113">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="67274-113">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="67274-114">grouppolicydefinitionvalue の取得</span><span class="sxs-lookup"><span data-stu-id="67274-114">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="67274-115">grouppolicydefinitionvalue</span><span class="sxs-lookup"><span data-stu-id="67274-115">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="67274-116">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="67274-116">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="67274-117">grouppolicydefinitionvalue の作成</span><span class="sxs-lookup"><span data-stu-id="67274-117">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="67274-118">grouppolicydefinitionvalue</span><span class="sxs-lookup"><span data-stu-id="67274-118">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="67274-119">新しい[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67274-119">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="67274-120">grouppolicydefinitionvalue の削除</span><span class="sxs-lookup"><span data-stu-id="67274-120">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="67274-121">なし</span><span class="sxs-lookup"><span data-stu-id="67274-121">None</span></span>|<span data-ttu-id="67274-122">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="67274-122">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="67274-123">grouppolicydefinitionvalue の更新</span><span class="sxs-lookup"><span data-stu-id="67274-123">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="67274-124">grouppolicydefinitionvalue</span><span class="sxs-lookup"><span data-stu-id="67274-124">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="67274-125">[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67274-125">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="67274-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67274-126">Properties</span></span>
|<span data-ttu-id="67274-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67274-127">Property</span></span>|<span data-ttu-id="67274-128">型</span><span class="sxs-lookup"><span data-stu-id="67274-128">Type</span></span>|<span data-ttu-id="67274-129">説明</span><span class="sxs-lookup"><span data-stu-id="67274-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67274-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67274-130">createdDateTime</span></span>|<span data-ttu-id="67274-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67274-131">DateTimeOffset</span></span>|<span data-ttu-id="67274-132">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="67274-132">The date and time the object was created.</span></span>|
|<span data-ttu-id="67274-133">enabled</span><span class="sxs-lookup"><span data-stu-id="67274-133">enabled</span></span>|<span data-ttu-id="67274-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="67274-134">Boolean</span></span>|<span data-ttu-id="67274-135">関連付けられたグループポリシー定義を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="67274-135">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="67274-136">configurationType</span><span class="sxs-lookup"><span data-stu-id="67274-136">configurationType</span></span>|[<span data-ttu-id="67274-137">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="67274-137">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="67274-138">値の構成方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="67274-138">Specifies how the value should be configured.</span></span> <span data-ttu-id="67274-139">これは、ポリシーとして、または設定することができます。</span><span class="sxs-lookup"><span data-stu-id="67274-139">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="67274-140">使用可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="67274-140">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="67274-141">id</span><span class="sxs-lookup"><span data-stu-id="67274-141">id</span></span>|<span data-ttu-id="67274-142">String</span><span class="sxs-lookup"><span data-stu-id="67274-142">String</span></span>|<span data-ttu-id="67274-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67274-143">Key of the entity.</span></span>|
|<span data-ttu-id="67274-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67274-144">lastModifiedDateTime</span></span>|<span data-ttu-id="67274-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67274-145">DateTimeOffset</span></span>|<span data-ttu-id="67274-146">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="67274-146">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67274-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67274-147">Relationships</span></span>
|<span data-ttu-id="67274-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67274-148">Relationship</span></span>|<span data-ttu-id="67274-149">型</span><span class="sxs-lookup"><span data-stu-id="67274-149">Type</span></span>|<span data-ttu-id="67274-150">説明</span><span class="sxs-lookup"><span data-stu-id="67274-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67274-151">プレゼンテーションの値</span><span class="sxs-lookup"><span data-stu-id="67274-151">presentationValues</span></span>|<span data-ttu-id="67274-152">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="67274-152">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="67274-153">関連付けられたグループポリシーの値が定義値と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="67274-153">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="67274-154">definition</span><span class="sxs-lookup"><span data-stu-id="67274-154">definition</span></span>|[<span data-ttu-id="67274-155">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="67274-155">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="67274-156">関連付けられたグループポリシー定義の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="67274-156">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67274-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67274-157">JSON Representation</span></span>
<span data-ttu-id="67274-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67274-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




