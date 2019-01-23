---
title: groupPolicyDefinitionValue リソースの種類
description: 定義値のエンティティは、1 つのグループ ポリシーの定義の値を格納します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7e98a41409efba60ee1431fac82a49be2029039
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430510"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="5ebae-103">groupPolicyDefinitionValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ebae-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="5ebae-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ebae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5ebae-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ebae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ebae-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ebae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebae-107">定義値のエンティティは、1 つのグループ ポリシーの定義の値を格納します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-107">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="5ebae-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5ebae-108">Methods</span></span>
|<span data-ttu-id="5ebae-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5ebae-109">Method</span></span>|<span data-ttu-id="5ebae-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5ebae-110">Return Type</span></span>|<span data-ttu-id="5ebae-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ebae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ebae-112">リスト groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="5ebae-112">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="5ebae-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5ebae-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="5ebae-114">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-114">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="5ebae-115">GroupPolicyDefinitionValue を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-115">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="5ebae-116">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5ebae-116">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5ebae-117">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ebae-117">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="5ebae-118">GroupPolicyDefinitionValue を作成します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-118">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="5ebae-119">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5ebae-119">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5ebae-120">新しい[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-120">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="5ebae-121">GroupPolicyDefinitionValue を削除します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-121">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="5ebae-122">なし</span><span class="sxs-lookup"><span data-stu-id="5ebae-122">None</span></span>|<span data-ttu-id="5ebae-123">の[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-123">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="5ebae-124">GroupPolicyDefinitionValue を更新します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-124">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="5ebae-125">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5ebae-125">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5ebae-126">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-126">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ebae-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ebae-127">Properties</span></span>
|<span data-ttu-id="5ebae-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ebae-128">Property</span></span>|<span data-ttu-id="5ebae-129">型</span><span class="sxs-lookup"><span data-stu-id="5ebae-129">Type</span></span>|<span data-ttu-id="5ebae-130">説明</span><span class="sxs-lookup"><span data-stu-id="5ebae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebae-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebae-131">createdDateTime</span></span>|<span data-ttu-id="5ebae-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebae-132">DateTimeOffset</span></span>|<span data-ttu-id="5ebae-133">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-133">The date and time the object was created.</span></span>|
|<span data-ttu-id="5ebae-134">enabled</span><span class="sxs-lookup"><span data-stu-id="5ebae-134">enabled</span></span>|<span data-ttu-id="5ebae-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebae-135">Boolean</span></span>|<span data-ttu-id="5ebae-136">有効または、関連付けられているグループ ポリシーの定義を無効にします。</span><span class="sxs-lookup"><span data-stu-id="5ebae-136">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="5ebae-137">configurationType</span><span class="sxs-lookup"><span data-stu-id="5ebae-137">configurationType</span></span>|[<span data-ttu-id="5ebae-138">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="5ebae-138">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="5ebae-139">値を構成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ebae-139">Specifies how the value should be configured.</span></span> <span data-ttu-id="5ebae-140">ポリシーとして、または環境設定のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5ebae-140">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="5ebae-141">使用可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="5ebae-141">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="5ebae-142">id</span><span class="sxs-lookup"><span data-stu-id="5ebae-142">id</span></span>|<span data-ttu-id="5ebae-143">String</span><span class="sxs-lookup"><span data-stu-id="5ebae-143">String</span></span>|<span data-ttu-id="5ebae-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5ebae-144">Key of the entity.</span></span>|
|<span data-ttu-id="5ebae-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebae-145">lastModifiedDateTime</span></span>|<span data-ttu-id="5ebae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebae-146">DateTimeOffset</span></span>|<span data-ttu-id="5ebae-147">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="5ebae-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ebae-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ebae-148">Relationships</span></span>
|<span data-ttu-id="5ebae-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ebae-149">Relationship</span></span>|<span data-ttu-id="5ebae-150">型</span><span class="sxs-lookup"><span data-stu-id="5ebae-150">Type</span></span>|<span data-ttu-id="5ebae-151">説明</span><span class="sxs-lookup"><span data-stu-id="5ebae-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebae-152">presentationValues</span><span class="sxs-lookup"><span data-stu-id="5ebae-152">presentationValues</span></span>|<span data-ttu-id="5ebae-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5ebae-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="5ebae-154">定義の値に関連付けられたグループ ポリシー プレゼンテーション値です。</span><span class="sxs-lookup"><span data-stu-id="5ebae-154">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="5ebae-155">definition</span><span class="sxs-lookup"><span data-stu-id="5ebae-155">definition</span></span>|[<span data-ttu-id="5ebae-156">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebae-156">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="5ebae-157">値に関連付けられているグループ ポリシーの定義です。</span><span class="sxs-lookup"><span data-stu-id="5ebae-157">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ebae-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ebae-158">JSON Representation</span></span>
<span data-ttu-id="5ebae-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ebae-159">Here is a JSON representation of the resource.</span></span>
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




