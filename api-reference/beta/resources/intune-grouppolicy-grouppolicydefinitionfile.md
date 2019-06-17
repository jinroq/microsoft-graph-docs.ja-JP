---
title: groupPolicyDefinitionFile リソースの種類
description: エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。 ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。 グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a872671186e55524002b2d0a5f85b2ce1bbf2466
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975939"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="cc991-105">groupPolicyDefinitionFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc991-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="cc991-106">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc991-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc991-107">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc991-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc991-108">エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="cc991-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="cc991-109">ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc991-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="cc991-110">グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc991-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="cc991-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc991-111">Methods</span></span>
|<span data-ttu-id="cc991-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc991-112">Method</span></span>|<span data-ttu-id="cc991-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc991-113">Return Type</span></span>|<span data-ttu-id="cc991-114">説明</span><span class="sxs-lookup"><span data-stu-id="cc991-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc991-115">GroupPolicyDefinitionFile の取得</span><span class="sxs-lookup"><span data-stu-id="cc991-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="cc991-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="cc991-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="cc991-117">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cc991-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="cc991-118">GroupPolicyDefinitionFile の更新</span><span class="sxs-lookup"><span data-stu-id="cc991-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="cc991-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="cc991-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="cc991-120">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc991-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc991-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc991-121">Properties</span></span>
|<span data-ttu-id="cc991-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc991-122">Property</span></span>|<span data-ttu-id="cc991-123">型</span><span class="sxs-lookup"><span data-stu-id="cc991-123">Type</span></span>|<span data-ttu-id="cc991-124">説明</span><span class="sxs-lookup"><span data-stu-id="cc991-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc991-125">displayName</span><span class="sxs-lookup"><span data-stu-id="cc991-125">displayName</span></span>|<span data-ttu-id="cc991-126">String</span><span class="sxs-lookup"><span data-stu-id="cc991-126">String</span></span>|<span data-ttu-id="cc991-127">ADMX ファイルのローカライズされたフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="cc991-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="cc991-128">description</span><span class="sxs-lookup"><span data-stu-id="cc991-128">description</span></span>|<span data-ttu-id="cc991-129">String</span><span class="sxs-lookup"><span data-stu-id="cc991-129">String</span></span>|<span data-ttu-id="cc991-130">ADMX ファイルのポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="cc991-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="cc991-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="cc991-131">The default value is empty.</span></span>|
|<span data-ttu-id="cc991-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="cc991-132">languageCodes</span></span>|<span data-ttu-id="cc991-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="cc991-133">String collection</span></span>|<span data-ttu-id="cc991-134">ADMX ファイルでサポートされている言語コード。</span><span class="sxs-lookup"><span data-stu-id="cc991-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="cc991-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="cc991-135">targetPrefix</span></span>|<span data-ttu-id="cc991-136">String</span><span class="sxs-lookup"><span data-stu-id="cc991-136">String</span></span>|<span data-ttu-id="cc991-137">ADMX ファイル内の名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc991-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="cc991-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="cc991-138">targetNamespace</span></span>|<span data-ttu-id="cc991-139">String</span><span class="sxs-lookup"><span data-stu-id="cc991-139">String</span></span>|<span data-ttu-id="cc991-140">ADMX ファイル内の名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc991-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="cc991-141">Msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="cc991-141">policyType</span></span>|[<span data-ttu-id="cc991-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="cc991-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="cc991-143">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc991-143">Specifies the type of group policy.</span></span> <span data-ttu-id="cc991-144">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="cc991-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="cc991-145">id</span><span class="sxs-lookup"><span data-stu-id="cc991-145">id</span></span>|<span data-ttu-id="cc991-146">文字列</span><span class="sxs-lookup"><span data-stu-id="cc991-146">String</span></span>|<span data-ttu-id="cc991-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cc991-147">Key of the entity.</span></span>|
|<span data-ttu-id="cc991-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc991-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cc991-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc991-149">DateTimeOffset</span></span>|<span data-ttu-id="cc991-150">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="cc991-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc991-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc991-151">Relationships</span></span>
|<span data-ttu-id="cc991-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc991-152">Relationship</span></span>|<span data-ttu-id="cc991-153">型</span><span class="sxs-lookup"><span data-stu-id="cc991-153">Type</span></span>|<span data-ttu-id="cc991-154">説明</span><span class="sxs-lookup"><span data-stu-id="cc991-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc991-155">構造</span><span class="sxs-lookup"><span data-stu-id="cc991-155">definitions</span></span>|<span data-ttu-id="cc991-156">[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc991-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="cc991-157">ファイルに関連付けられたグループポリシーの定義。</span><span class="sxs-lookup"><span data-stu-id="cc991-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc991-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc991-158">JSON Representation</span></span>
<span data-ttu-id="cc991-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc991-159">Here is a JSON representation of the resource.</span></span>
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





