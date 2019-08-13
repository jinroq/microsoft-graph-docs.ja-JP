---
title: groupPolicyDefinitionValue リソースの種類
description: 定義値エンティティは、1つのグループポリシー定義の値を格納します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 406c7107418255c00e123a4a4c21b9ae446eea5d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331449"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="8cdb1-103">groupPolicyDefinitionValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cdb1-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="8cdb1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cdb1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cdb1-106">定義値エンティティは、1つのグループポリシー定義の値を格納します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-106">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="8cdb1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cdb1-107">Methods</span></span>
|<span data-ttu-id="8cdb1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cdb1-108">Method</span></span>|<span data-ttu-id="8cdb1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8cdb1-109">Return Type</span></span>|<span data-ttu-id="8cdb1-110">説明</span><span class="sxs-lookup"><span data-stu-id="8cdb1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8cdb1-111">GroupPolicyDefinitionValues のリスト</span><span class="sxs-lookup"><span data-stu-id="8cdb1-111">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="8cdb1-112">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8cdb1-112">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="8cdb1-113">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-113">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="8cdb1-114">GroupPolicyDefinitionValue の取得</span><span class="sxs-lookup"><span data-stu-id="8cdb1-114">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="8cdb1-115">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="8cdb1-115">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="8cdb1-116">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-116">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="8cdb1-117">GroupPolicyDefinitionValue の作成</span><span class="sxs-lookup"><span data-stu-id="8cdb1-117">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="8cdb1-118">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="8cdb1-118">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="8cdb1-119">新しい[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-119">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="8cdb1-120">GroupPolicyDefinitionValue の削除</span><span class="sxs-lookup"><span data-stu-id="8cdb1-120">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="8cdb1-121">None</span><span class="sxs-lookup"><span data-stu-id="8cdb1-121">None</span></span>|<span data-ttu-id="8cdb1-122">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-122">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="8cdb1-123">GroupPolicyDefinitionValue の更新</span><span class="sxs-lookup"><span data-stu-id="8cdb1-123">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="8cdb1-124">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="8cdb1-124">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="8cdb1-125">[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-125">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cdb1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdb1-126">Properties</span></span>
|<span data-ttu-id="8cdb1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdb1-127">Property</span></span>|<span data-ttu-id="8cdb1-128">型</span><span class="sxs-lookup"><span data-stu-id="8cdb1-128">Type</span></span>|<span data-ttu-id="8cdb1-129">説明</span><span class="sxs-lookup"><span data-stu-id="8cdb1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdb1-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cdb1-130">createdDateTime</span></span>|<span data-ttu-id="8cdb1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cdb1-131">DateTimeOffset</span></span>|<span data-ttu-id="8cdb1-132">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-132">The date and time the object was created.</span></span>|
|<span data-ttu-id="8cdb1-133">enabled</span><span class="sxs-lookup"><span data-stu-id="8cdb1-133">enabled</span></span>|<span data-ttu-id="8cdb1-134">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8cdb1-134">Boolean</span></span>|<span data-ttu-id="8cdb1-135">関連付けられたグループポリシー定義を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-135">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="8cdb1-136">configurationType</span><span class="sxs-lookup"><span data-stu-id="8cdb1-136">configurationType</span></span>|[<span data-ttu-id="8cdb1-137">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="8cdb1-137">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="8cdb1-138">値の構成方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-138">Specifies how the value should be configured.</span></span> <span data-ttu-id="8cdb1-139">これは、ポリシーとして、または設定することができます。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-139">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="8cdb1-140">可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-140">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="8cdb1-141">id</span><span class="sxs-lookup"><span data-stu-id="8cdb1-141">id</span></span>|<span data-ttu-id="8cdb1-142">String</span><span class="sxs-lookup"><span data-stu-id="8cdb1-142">String</span></span>|<span data-ttu-id="8cdb1-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-143">Key of the entity.</span></span>|
|<span data-ttu-id="8cdb1-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cdb1-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8cdb1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cdb1-145">DateTimeOffset</span></span>|<span data-ttu-id="8cdb1-146">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-146">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cdb1-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cdb1-147">Relationships</span></span>
|<span data-ttu-id="8cdb1-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cdb1-148">Relationship</span></span>|<span data-ttu-id="8cdb1-149">型</span><span class="sxs-lookup"><span data-stu-id="8cdb1-149">Type</span></span>|<span data-ttu-id="8cdb1-150">説明</span><span class="sxs-lookup"><span data-stu-id="8cdb1-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdb1-151">プレゼンテーションの値</span><span class="sxs-lookup"><span data-stu-id="8cdb1-151">presentationValues</span></span>|<span data-ttu-id="8cdb1-152">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8cdb1-152">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="8cdb1-153">関連付けられたグループポリシーの値が定義値と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-153">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="8cdb1-154">definition</span><span class="sxs-lookup"><span data-stu-id="8cdb1-154">definition</span></span>|[<span data-ttu-id="8cdb1-155">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="8cdb1-155">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="8cdb1-156">関連付けられたグループポリシー定義の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-156">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cdb1-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cdb1-157">JSON Representation</span></span>
<span data-ttu-id="8cdb1-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cdb1-158">Here is a JSON representation of the resource.</span></span>
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



