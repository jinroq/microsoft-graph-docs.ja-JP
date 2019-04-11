---
title: grouppolicydefinitionfile リソースの種類
description: エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。 ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。 グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ecccc683187b592c422d26a6f41bfd15b9d805b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804138"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="e25fd-105">grouppolicydefinitionfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e25fd-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="e25fd-106">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e25fd-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e25fd-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e25fd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e25fd-108">エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="e25fd-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="e25fd-109">ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e25fd-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="e25fd-110">グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。</span><span class="sxs-lookup"><span data-stu-id="e25fd-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="e25fd-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="e25fd-111">Methods</span></span>
|<span data-ttu-id="e25fd-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="e25fd-112">Method</span></span>|<span data-ttu-id="e25fd-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e25fd-113">Return Type</span></span>|<span data-ttu-id="e25fd-114">説明</span><span class="sxs-lookup"><span data-stu-id="e25fd-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e25fd-115">grouppolicydefinitionfile の取得</span><span class="sxs-lookup"><span data-stu-id="e25fd-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="e25fd-116">grouppolicydefinitionfile</span><span class="sxs-lookup"><span data-stu-id="e25fd-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="e25fd-117">[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e25fd-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="e25fd-118">grouppolicydefinitionfile の更新</span><span class="sxs-lookup"><span data-stu-id="e25fd-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="e25fd-119">grouppolicydefinitionfile</span><span class="sxs-lookup"><span data-stu-id="e25fd-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="e25fd-120">[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e25fd-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e25fd-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e25fd-121">Properties</span></span>
|<span data-ttu-id="e25fd-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e25fd-122">Property</span></span>|<span data-ttu-id="e25fd-123">型</span><span class="sxs-lookup"><span data-stu-id="e25fd-123">Type</span></span>|<span data-ttu-id="e25fd-124">説明</span><span class="sxs-lookup"><span data-stu-id="e25fd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e25fd-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e25fd-125">displayName</span></span>|<span data-ttu-id="e25fd-126">String</span><span class="sxs-lookup"><span data-stu-id="e25fd-126">String</span></span>|<span data-ttu-id="e25fd-127">ADMX ファイルのローカライズされたフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="e25fd-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="e25fd-128">説明</span><span class="sxs-lookup"><span data-stu-id="e25fd-128">description</span></span>|<span data-ttu-id="e25fd-129">String</span><span class="sxs-lookup"><span data-stu-id="e25fd-129">String</span></span>|<span data-ttu-id="e25fd-130">ADMX ファイルのポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="e25fd-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="e25fd-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="e25fd-131">The default value is empty.</span></span>|
|<span data-ttu-id="e25fd-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="e25fd-132">languageCodes</span></span>|<span data-ttu-id="e25fd-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e25fd-133">String collection</span></span>|<span data-ttu-id="e25fd-134">ADMX ファイルでサポートされている言語コード。</span><span class="sxs-lookup"><span data-stu-id="e25fd-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="e25fd-135">targetprefix</span><span class="sxs-lookup"><span data-stu-id="e25fd-135">targetPrefix</span></span>|<span data-ttu-id="e25fd-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e25fd-136">String</span></span>|<span data-ttu-id="e25fd-137">ADMX ファイル内の名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="e25fd-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="e25fd-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="e25fd-138">targetNamespace</span></span>|<span data-ttu-id="e25fd-139">文字列</span><span class="sxs-lookup"><span data-stu-id="e25fd-139">String</span></span>|<span data-ttu-id="e25fd-140">ADMX ファイル内の名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="e25fd-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="e25fd-141">msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="e25fd-141">policyType</span></span>|[<span data-ttu-id="e25fd-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e25fd-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e25fd-143">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="e25fd-143">Specifies the type of group policy.</span></span> <span data-ttu-id="e25fd-144">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="e25fd-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e25fd-145">id</span><span class="sxs-lookup"><span data-stu-id="e25fd-145">id</span></span>|<span data-ttu-id="e25fd-146">String</span><span class="sxs-lookup"><span data-stu-id="e25fd-146">String</span></span>|<span data-ttu-id="e25fd-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e25fd-147">Key of the entity.</span></span>|
|<span data-ttu-id="e25fd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e25fd-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e25fd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e25fd-149">DateTimeOffset</span></span>|<span data-ttu-id="e25fd-150">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="e25fd-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e25fd-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e25fd-151">Relationships</span></span>
|<span data-ttu-id="e25fd-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e25fd-152">Relationship</span></span>|<span data-ttu-id="e25fd-153">型</span><span class="sxs-lookup"><span data-stu-id="e25fd-153">Type</span></span>|<span data-ttu-id="e25fd-154">説明</span><span class="sxs-lookup"><span data-stu-id="e25fd-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e25fd-155">構造</span><span class="sxs-lookup"><span data-stu-id="e25fd-155">definitions</span></span>|<span data-ttu-id="e25fd-156">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e25fd-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="e25fd-157">ファイルに関連付けられたグループポリシーの定義。</span><span class="sxs-lookup"><span data-stu-id="e25fd-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e25fd-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e25fd-158">JSON Representation</span></span>
<span data-ttu-id="e25fd-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e25fd-159">Here is a JSON representation of the resource.</span></span>
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





