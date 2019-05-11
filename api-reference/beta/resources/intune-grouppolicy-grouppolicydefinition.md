---
title: groupPolicyDefinition リソースの種類
description: エンティティは、1つのグループポリシーに関するすべての情報を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17fef49d7d08f94f5ebafd02636d9536a05b87f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941171"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="c43d9-103">groupPolicyDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c43d9-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="c43d9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c43d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c43d9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c43d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c43d9-106">エンティティは、1つのグループポリシーに関するすべての情報を記述します。</span><span class="sxs-lookup"><span data-stu-id="c43d9-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="c43d9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c43d9-107">Methods</span></span>
|<span data-ttu-id="c43d9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c43d9-108">Method</span></span>|<span data-ttu-id="c43d9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c43d9-109">Return Type</span></span>|<span data-ttu-id="c43d9-110">説明</span><span class="sxs-lookup"><span data-stu-id="c43d9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c43d9-111">GroupPolicyDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="c43d9-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="c43d9-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c43d9-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="c43d9-113">[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c43d9-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="c43d9-114">GroupPolicyDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="c43d9-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="c43d9-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c43d9-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="c43d9-116">[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c43d9-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c43d9-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c43d9-117">Properties</span></span>
|<span data-ttu-id="c43d9-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c43d9-118">Property</span></span>|<span data-ttu-id="c43d9-119">種類</span><span class="sxs-lookup"><span data-stu-id="c43d9-119">Type</span></span>|<span data-ttu-id="c43d9-120">説明</span><span class="sxs-lookup"><span data-stu-id="c43d9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43d9-121">classType</span><span class="sxs-lookup"><span data-stu-id="c43d9-121">classType</span></span>|[<span data-ttu-id="c43d9-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="c43d9-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="c43d9-123">ポリシーを適用できるグループの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c43d9-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="c43d9-124">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="c43d9-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c43d9-125">displayName</span><span class="sxs-lookup"><span data-stu-id="c43d9-125">displayName</span></span>|<span data-ttu-id="c43d9-126">String</span><span class="sxs-lookup"><span data-stu-id="c43d9-126">String</span></span>|<span data-ttu-id="c43d9-127">ローカライズされたポリシー名。</span><span class="sxs-lookup"><span data-stu-id="c43d9-127">The localized policy name.</span></span>|
|<span data-ttu-id="c43d9-128">explainText</span><span class="sxs-lookup"><span data-stu-id="c43d9-128">explainText</span></span>|<span data-ttu-id="c43d9-129">String</span><span class="sxs-lookup"><span data-stu-id="c43d9-129">String</span></span>|<span data-ttu-id="c43d9-130">ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="c43d9-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="c43d9-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="c43d9-131">The default value is empty.</span></span>|
|<span data-ttu-id="c43d9-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="c43d9-132">categoryPath</span></span>|<span data-ttu-id="c43d9-133">String</span><span class="sxs-lookup"><span data-stu-id="c43d9-133">String</span></span>|<span data-ttu-id="c43d9-134">ポリシーのローカライズされた完全なカテゴリのパス。</span><span class="sxs-lookup"><span data-stu-id="c43d9-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="c43d9-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="c43d9-135">supportedOn</span></span>|<span data-ttu-id="c43d9-136">String</span><span class="sxs-lookup"><span data-stu-id="c43d9-136">String</span></span>|<span data-ttu-id="c43d9-137">ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。</span><span class="sxs-lookup"><span data-stu-id="c43d9-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="c43d9-138">Msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="c43d9-138">policyType</span></span>|[<span data-ttu-id="c43d9-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c43d9-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c43d9-140">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c43d9-140">Specifies the type of group policy.</span></span> <span data-ttu-id="c43d9-141">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="c43d9-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c43d9-142">id</span><span class="sxs-lookup"><span data-stu-id="c43d9-142">id</span></span>|<span data-ttu-id="c43d9-143">文字列</span><span class="sxs-lookup"><span data-stu-id="c43d9-143">String</span></span>|<span data-ttu-id="c43d9-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c43d9-144">Key of the entity.</span></span>|
|<span data-ttu-id="c43d9-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c43d9-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c43d9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c43d9-146">DateTimeOffset</span></span>|<span data-ttu-id="c43d9-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c43d9-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43d9-148">関係</span><span class="sxs-lookup"><span data-stu-id="c43d9-148">Relationships</span></span>
|<span data-ttu-id="c43d9-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c43d9-149">Relationship</span></span>|<span data-ttu-id="c43d9-150">型</span><span class="sxs-lookup"><span data-stu-id="c43d9-150">Type</span></span>|<span data-ttu-id="c43d9-151">説明</span><span class="sxs-lookup"><span data-stu-id="c43d9-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43d9-152">definitionFile</span><span class="sxs-lookup"><span data-stu-id="c43d9-152">definitionFile</span></span>|[<span data-ttu-id="c43d9-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c43d9-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="c43d9-154">定義に関連付けられているグループポリシーファイル。</span><span class="sxs-lookup"><span data-stu-id="c43d9-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="c43d9-155">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="c43d9-155">presentations</span></span>|<span data-ttu-id="c43d9-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c43d9-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="c43d9-157">定義に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="c43d9-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c43d9-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c43d9-158">JSON Representation</span></span>
<span data-ttu-id="c43d9-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c43d9-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




