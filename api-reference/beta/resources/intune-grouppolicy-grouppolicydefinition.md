---
title: grouppolicydefinition リソースの種類
description: エンティティは、1つのグループポリシーに関するすべての情報を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5062fda984dbe1dda518e77ff271750d30adb8
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644287"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="ddb33-103">grouppolicydefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddb33-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="ddb33-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddb33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb33-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ddb33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb33-106">エンティティは、1つのグループポリシーに関するすべての情報を記述します。</span><span class="sxs-lookup"><span data-stu-id="ddb33-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="ddb33-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddb33-107">Methods</span></span>
|<span data-ttu-id="ddb33-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddb33-108">Method</span></span>|<span data-ttu-id="ddb33-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ddb33-109">Return Type</span></span>|<span data-ttu-id="ddb33-110">説明</span><span class="sxs-lookup"><span data-stu-id="ddb33-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddb33-111">grouppolicydefinition の取得</span><span class="sxs-lookup"><span data-stu-id="ddb33-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="ddb33-112">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="ddb33-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="ddb33-113">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ddb33-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="ddb33-114">grouppolicydefinition の更新</span><span class="sxs-lookup"><span data-stu-id="ddb33-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="ddb33-115">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="ddb33-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="ddb33-116">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ddb33-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddb33-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb33-117">Properties</span></span>
|<span data-ttu-id="ddb33-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb33-118">Property</span></span>|<span data-ttu-id="ddb33-119">型</span><span class="sxs-lookup"><span data-stu-id="ddb33-119">Type</span></span>|<span data-ttu-id="ddb33-120">説明</span><span class="sxs-lookup"><span data-stu-id="ddb33-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb33-121">classType</span><span class="sxs-lookup"><span data-stu-id="ddb33-121">classType</span></span>|[<span data-ttu-id="ddb33-122">grouppolicydefinitionclasstype</span><span class="sxs-lookup"><span data-stu-id="ddb33-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="ddb33-123">ポリシーを適用できるグループの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ddb33-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="ddb33-124">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="ddb33-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ddb33-125">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb33-125">displayName</span></span>|<span data-ttu-id="ddb33-126">String</span><span class="sxs-lookup"><span data-stu-id="ddb33-126">String</span></span>|<span data-ttu-id="ddb33-127">ローカライズされたポリシー名。</span><span class="sxs-lookup"><span data-stu-id="ddb33-127">The localized policy name.</span></span>|
|<span data-ttu-id="ddb33-128">explainText</span><span class="sxs-lookup"><span data-stu-id="ddb33-128">explainText</span></span>|<span data-ttu-id="ddb33-129">String</span><span class="sxs-lookup"><span data-stu-id="ddb33-129">String</span></span>|<span data-ttu-id="ddb33-130">ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="ddb33-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="ddb33-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="ddb33-131">The default value is empty.</span></span>|
|<span data-ttu-id="ddb33-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="ddb33-132">categoryPath</span></span>|<span data-ttu-id="ddb33-133">String</span><span class="sxs-lookup"><span data-stu-id="ddb33-133">String</span></span>|<span data-ttu-id="ddb33-134">ポリシーのローカライズされた完全なカテゴリのパス。</span><span class="sxs-lookup"><span data-stu-id="ddb33-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="ddb33-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="ddb33-135">supportedOn</span></span>|<span data-ttu-id="ddb33-136">String</span><span class="sxs-lookup"><span data-stu-id="ddb33-136">String</span></span>|<span data-ttu-id="ddb33-137">ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。</span><span class="sxs-lookup"><span data-stu-id="ddb33-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="ddb33-138">msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="ddb33-138">policyType</span></span>|[<span data-ttu-id="ddb33-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="ddb33-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="ddb33-140">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ddb33-140">Specifies the type of group policy.</span></span> <span data-ttu-id="ddb33-141">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="ddb33-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="ddb33-142">id</span><span class="sxs-lookup"><span data-stu-id="ddb33-142">id</span></span>|<span data-ttu-id="ddb33-143">String</span><span class="sxs-lookup"><span data-stu-id="ddb33-143">String</span></span>|<span data-ttu-id="ddb33-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ddb33-144">Key of the entity.</span></span>|
|<span data-ttu-id="ddb33-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb33-145">lastModifiedDateTime</span></span>|<span data-ttu-id="ddb33-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb33-146">DateTimeOffset</span></span>|<span data-ttu-id="ddb33-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="ddb33-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddb33-148">関係</span><span class="sxs-lookup"><span data-stu-id="ddb33-148">Relationships</span></span>
|<span data-ttu-id="ddb33-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddb33-149">Relationship</span></span>|<span data-ttu-id="ddb33-150">型</span><span class="sxs-lookup"><span data-stu-id="ddb33-150">Type</span></span>|<span data-ttu-id="ddb33-151">説明</span><span class="sxs-lookup"><span data-stu-id="ddb33-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb33-152">definitionfile</span><span class="sxs-lookup"><span data-stu-id="ddb33-152">definitionFile</span></span>|[<span data-ttu-id="ddb33-153">grouppolicydefinitionfile</span><span class="sxs-lookup"><span data-stu-id="ddb33-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="ddb33-154">定義に関連付けられているグループポリシーファイル。</span><span class="sxs-lookup"><span data-stu-id="ddb33-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="ddb33-155">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="ddb33-155">presentations</span></span>|<span data-ttu-id="ddb33-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ddb33-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="ddb33-157">定義に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="ddb33-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddb33-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddb33-158">JSON Representation</span></span>
<span data-ttu-id="ddb33-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddb33-159">Here is a JSON representation of the resource.</span></span>
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




