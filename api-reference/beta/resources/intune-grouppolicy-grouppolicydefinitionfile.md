---
title: groupPolicyDefinitionFile リソースの種類
description: エンティティでは、ADMX (管理テンプレート) の XML ファイルを表します。 ADMX ファイルには、カテゴリへのパスでのグループ ポリシーの定義のコレクションとその場所が含まれています。 グループ ポリシー定義ファイルには、言語依存の ADML (管理テンプレート) の言語ファイルでサポートされる言語も含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431621"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="b707e-105">groupPolicyDefinitionFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b707e-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="b707e-106">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b707e-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b707e-107">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b707e-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b707e-108">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b707e-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b707e-109">エンティティでは、ADMX (管理テンプレート) の XML ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="b707e-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="b707e-110">ADMX ファイルには、カテゴリへのパスでのグループ ポリシーの定義のコレクションとその場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b707e-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="b707e-111">グループ ポリシー定義ファイルには、言語依存の ADML (管理テンプレート) の言語ファイルでサポートされる言語も含まれています。</span><span class="sxs-lookup"><span data-stu-id="b707e-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="b707e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="b707e-112">Methods</span></span>
|<span data-ttu-id="b707e-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="b707e-113">Method</span></span>|<span data-ttu-id="b707e-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b707e-114">Return Type</span></span>|<span data-ttu-id="b707e-115">説明</span><span class="sxs-lookup"><span data-stu-id="b707e-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b707e-116">GroupPolicyDefinitionFile を取得します。</span><span class="sxs-lookup"><span data-stu-id="b707e-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="b707e-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="b707e-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="b707e-118">[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b707e-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="b707e-119">GroupPolicyDefinitionFile を更新します。</span><span class="sxs-lookup"><span data-stu-id="b707e-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="b707e-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="b707e-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="b707e-121">[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b707e-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b707e-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b707e-122">Properties</span></span>
|<span data-ttu-id="b707e-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b707e-123">Property</span></span>|<span data-ttu-id="b707e-124">型</span><span class="sxs-lookup"><span data-stu-id="b707e-124">Type</span></span>|<span data-ttu-id="b707e-125">説明</span><span class="sxs-lookup"><span data-stu-id="b707e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b707e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="b707e-126">displayName</span></span>|<span data-ttu-id="b707e-127">String</span><span class="sxs-lookup"><span data-stu-id="b707e-127">String</span></span>|<span data-ttu-id="b707e-128">ADMX ファイルのローカライズされた表示名です。</span><span class="sxs-lookup"><span data-stu-id="b707e-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="b707e-129">説明</span><span class="sxs-lookup"><span data-stu-id="b707e-129">description</span></span>|<span data-ttu-id="b707e-130">String</span><span class="sxs-lookup"><span data-stu-id="b707e-130">String</span></span>|<span data-ttu-id="b707e-131">ADMX ファイル内のポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="b707e-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="b707e-132">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="b707e-132">The default value is empty.</span></span>|
|<span data-ttu-id="b707e-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="b707e-133">languageCodes</span></span>|<span data-ttu-id="b707e-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b707e-134">String collection</span></span>|<span data-ttu-id="b707e-135">ADMX ファイルのサポートされている言語コードです。</span><span class="sxs-lookup"><span data-stu-id="b707e-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="b707e-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="b707e-136">targetPrefix</span></span>|<span data-ttu-id="b707e-137">String</span><span class="sxs-lookup"><span data-stu-id="b707e-137">String</span></span>|<span data-ttu-id="b707e-138">ADMX ファイル内で名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="b707e-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b707e-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="b707e-139">targetNamespace</span></span>|<span data-ttu-id="b707e-140">String</span><span class="sxs-lookup"><span data-stu-id="b707e-140">String</span></span>|<span data-ttu-id="b707e-141">ADMX ファイル内で名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="b707e-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b707e-142">policyType</span><span class="sxs-lookup"><span data-stu-id="b707e-142">policyType</span></span>|[<span data-ttu-id="b707e-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b707e-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b707e-144">グループ ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b707e-144">Specifies the type of group policy.</span></span> <span data-ttu-id="b707e-145">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="b707e-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b707e-146">id</span><span class="sxs-lookup"><span data-stu-id="b707e-146">id</span></span>|<span data-ttu-id="b707e-147">String</span><span class="sxs-lookup"><span data-stu-id="b707e-147">String</span></span>|<span data-ttu-id="b707e-148">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b707e-148">Key of the entity.</span></span>|
|<span data-ttu-id="b707e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b707e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b707e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b707e-150">DateTimeOffset</span></span>|<span data-ttu-id="b707e-151">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="b707e-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b707e-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b707e-152">Relationships</span></span>
|<span data-ttu-id="b707e-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b707e-153">Relationship</span></span>|<span data-ttu-id="b707e-154">型</span><span class="sxs-lookup"><span data-stu-id="b707e-154">Type</span></span>|<span data-ttu-id="b707e-155">説明</span><span class="sxs-lookup"><span data-stu-id="b707e-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b707e-156">定義</span><span class="sxs-lookup"><span data-stu-id="b707e-156">definitions</span></span>|<span data-ttu-id="b707e-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b707e-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="b707e-158">ファイルに関連付けられているグループ ポリシーの定義です。</span><span class="sxs-lookup"><span data-stu-id="b707e-158">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b707e-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b707e-159">JSON Representation</span></span>
<span data-ttu-id="b707e-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b707e-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




