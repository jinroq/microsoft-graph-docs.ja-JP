---
title: grouppolicydefinition リソースの種類
description: エンティティは、1つのグループポリシーに関するすべての情報を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9e411c2672650e3e603bfa0e64fde1c4db53607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575773"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="a1314-103">grouppolicydefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1314-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="a1314-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1314-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1314-106">エンティティは、1つのグループポリシーに関するすべての情報を記述します。</span><span class="sxs-lookup"><span data-stu-id="a1314-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="a1314-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1314-107">Methods</span></span>
|<span data-ttu-id="a1314-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1314-108">Method</span></span>|<span data-ttu-id="a1314-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1314-109">Return Type</span></span>|<span data-ttu-id="a1314-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1314-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1314-111">grouppolicydefinition の取得</span><span class="sxs-lookup"><span data-stu-id="a1314-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="a1314-112">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="a1314-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="a1314-113">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1314-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="a1314-114">grouppolicydefinition の更新</span><span class="sxs-lookup"><span data-stu-id="a1314-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="a1314-115">grouppolicydefinition</span><span class="sxs-lookup"><span data-stu-id="a1314-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="a1314-116">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1314-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1314-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1314-117">Properties</span></span>
|<span data-ttu-id="a1314-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1314-118">Property</span></span>|<span data-ttu-id="a1314-119">型</span><span class="sxs-lookup"><span data-stu-id="a1314-119">Type</span></span>|<span data-ttu-id="a1314-120">説明</span><span class="sxs-lookup"><span data-stu-id="a1314-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1314-121">classType</span><span class="sxs-lookup"><span data-stu-id="a1314-121">classType</span></span>|[<span data-ttu-id="a1314-122">grouppolicydefinitionclasstype</span><span class="sxs-lookup"><span data-stu-id="a1314-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="a1314-123">ポリシーを適用できるグループの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1314-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="a1314-124">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="a1314-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="a1314-125">displayName</span><span class="sxs-lookup"><span data-stu-id="a1314-125">displayName</span></span>|<span data-ttu-id="a1314-126">String</span><span class="sxs-lookup"><span data-stu-id="a1314-126">String</span></span>|<span data-ttu-id="a1314-127">ローカライズされたポリシー名。</span><span class="sxs-lookup"><span data-stu-id="a1314-127">The localized policy name.</span></span>|
|<span data-ttu-id="a1314-128">explainText</span><span class="sxs-lookup"><span data-stu-id="a1314-128">explainText</span></span>|<span data-ttu-id="a1314-129">String</span><span class="sxs-lookup"><span data-stu-id="a1314-129">String</span></span>|<span data-ttu-id="a1314-130">ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="a1314-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="a1314-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="a1314-131">The default value is empty.</span></span>|
|<span data-ttu-id="a1314-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="a1314-132">categoryPath</span></span>|<span data-ttu-id="a1314-133">String</span><span class="sxs-lookup"><span data-stu-id="a1314-133">String</span></span>|<span data-ttu-id="a1314-134">ポリシーのローカライズされた完全なカテゴリのパス。</span><span class="sxs-lookup"><span data-stu-id="a1314-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="a1314-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="a1314-135">supportedOn</span></span>|<span data-ttu-id="a1314-136">String</span><span class="sxs-lookup"><span data-stu-id="a1314-136">String</span></span>|<span data-ttu-id="a1314-137">ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。</span><span class="sxs-lookup"><span data-stu-id="a1314-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="a1314-138">msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="a1314-138">policyType</span></span>|[<span data-ttu-id="a1314-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="a1314-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="a1314-140">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1314-140">Specifies the type of group policy.</span></span> <span data-ttu-id="a1314-141">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="a1314-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="a1314-142">id</span><span class="sxs-lookup"><span data-stu-id="a1314-142">id</span></span>|<span data-ttu-id="a1314-143">String</span><span class="sxs-lookup"><span data-stu-id="a1314-143">String</span></span>|<span data-ttu-id="a1314-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a1314-144">Key of the entity.</span></span>|
|<span data-ttu-id="a1314-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1314-145">lastModifiedDateTime</span></span>|<span data-ttu-id="a1314-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1314-146">DateTimeOffset</span></span>|<span data-ttu-id="a1314-147">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a1314-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1314-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1314-148">Relationships</span></span>
|<span data-ttu-id="a1314-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1314-149">Relationship</span></span>|<span data-ttu-id="a1314-150">型</span><span class="sxs-lookup"><span data-stu-id="a1314-150">Type</span></span>|<span data-ttu-id="a1314-151">説明</span><span class="sxs-lookup"><span data-stu-id="a1314-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1314-152">definitionfile</span><span class="sxs-lookup"><span data-stu-id="a1314-152">definitionFile</span></span>|[<span data-ttu-id="a1314-153">grouppolicydefinitionfile</span><span class="sxs-lookup"><span data-stu-id="a1314-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="a1314-154">定義に関連付けられているグループポリシーファイル。</span><span class="sxs-lookup"><span data-stu-id="a1314-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="a1314-155">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="a1314-155">presentations</span></span>|<span data-ttu-id="a1314-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1314-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="a1314-157">定義に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="a1314-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1314-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1314-158">JSON Representation</span></span>
<span data-ttu-id="a1314-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1314-159">Here is a JSON representation of the resource.</span></span>
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





