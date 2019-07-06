---
title: groupPolicyDefinitionFile リソースの種類
description: エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。 ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。 グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 384b59a2c9e1b669cd71b294c6420c13b95d1102
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576488"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="9561b-105">groupPolicyDefinitionFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9561b-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="9561b-106">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9561b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9561b-107">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9561b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9561b-108">エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="9561b-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="9561b-109">ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9561b-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="9561b-110">グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。</span><span class="sxs-lookup"><span data-stu-id="9561b-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="9561b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9561b-111">Methods</span></span>
|<span data-ttu-id="9561b-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="9561b-112">Method</span></span>|<span data-ttu-id="9561b-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9561b-113">Return Type</span></span>|<span data-ttu-id="9561b-114">説明</span><span class="sxs-lookup"><span data-stu-id="9561b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9561b-115">GroupPolicyDefinitionFile の取得</span><span class="sxs-lookup"><span data-stu-id="9561b-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="9561b-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9561b-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9561b-117">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9561b-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="9561b-118">GroupPolicyDefinitionFile の更新</span><span class="sxs-lookup"><span data-stu-id="9561b-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="9561b-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9561b-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9561b-120">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9561b-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9561b-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9561b-121">Properties</span></span>
|<span data-ttu-id="9561b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9561b-122">Property</span></span>|<span data-ttu-id="9561b-123">型</span><span class="sxs-lookup"><span data-stu-id="9561b-123">Type</span></span>|<span data-ttu-id="9561b-124">説明</span><span class="sxs-lookup"><span data-stu-id="9561b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9561b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="9561b-125">displayName</span></span>|<span data-ttu-id="9561b-126">String</span><span class="sxs-lookup"><span data-stu-id="9561b-126">String</span></span>|<span data-ttu-id="9561b-127">ADMX ファイルのローカライズされたフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="9561b-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="9561b-128">description</span><span class="sxs-lookup"><span data-stu-id="9561b-128">description</span></span>|<span data-ttu-id="9561b-129">String</span><span class="sxs-lookup"><span data-stu-id="9561b-129">String</span></span>|<span data-ttu-id="9561b-130">ADMX ファイルのポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="9561b-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="9561b-131">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="9561b-131">The default value is empty.</span></span>|
|<span data-ttu-id="9561b-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="9561b-132">languageCodes</span></span>|<span data-ttu-id="9561b-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9561b-133">String collection</span></span>|<span data-ttu-id="9561b-134">ADMX ファイルでサポートされている言語コード。</span><span class="sxs-lookup"><span data-stu-id="9561b-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="9561b-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="9561b-135">targetPrefix</span></span>|<span data-ttu-id="9561b-136">String</span><span class="sxs-lookup"><span data-stu-id="9561b-136">String</span></span>|<span data-ttu-id="9561b-137">ADMX ファイル内の名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="9561b-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="9561b-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="9561b-138">targetNamespace</span></span>|<span data-ttu-id="9561b-139">String</span><span class="sxs-lookup"><span data-stu-id="9561b-139">String</span></span>|<span data-ttu-id="9561b-140">ADMX ファイル内の名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="9561b-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="9561b-141">Msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="9561b-141">policyType</span></span>|[<span data-ttu-id="9561b-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9561b-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9561b-143">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="9561b-143">Specifies the type of group policy.</span></span> <span data-ttu-id="9561b-144">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="9561b-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9561b-145">改訂</span><span class="sxs-lookup"><span data-stu-id="9561b-145">revision</span></span>|<span data-ttu-id="9561b-146">String</span><span class="sxs-lookup"><span data-stu-id="9561b-146">String</span></span>|<span data-ttu-id="9561b-147">ファイルに関連付けられているリビジョンバージョン。</span><span class="sxs-lookup"><span data-stu-id="9561b-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="9561b-148">id</span><span class="sxs-lookup"><span data-stu-id="9561b-148">id</span></span>|<span data-ttu-id="9561b-149">文字列</span><span class="sxs-lookup"><span data-stu-id="9561b-149">String</span></span>|<span data-ttu-id="9561b-150">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9561b-150">Key of the entity.</span></span>|
|<span data-ttu-id="9561b-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9561b-151">lastModifiedDateTime</span></span>|<span data-ttu-id="9561b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9561b-152">DateTimeOffset</span></span>|<span data-ttu-id="9561b-153">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="9561b-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9561b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9561b-154">Relationships</span></span>
|<span data-ttu-id="9561b-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9561b-155">Relationship</span></span>|<span data-ttu-id="9561b-156">型</span><span class="sxs-lookup"><span data-stu-id="9561b-156">Type</span></span>|<span data-ttu-id="9561b-157">説明</span><span class="sxs-lookup"><span data-stu-id="9561b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9561b-158">構造</span><span class="sxs-lookup"><span data-stu-id="9561b-158">definitions</span></span>|<span data-ttu-id="9561b-159">[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9561b-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="9561b-160">ファイルに関連付けられたグループポリシーの定義。</span><span class="sxs-lookup"><span data-stu-id="9561b-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9561b-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9561b-161">JSON Representation</span></span>
<span data-ttu-id="9561b-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9561b-162">Here is a JSON representation of the resource.</span></span>
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
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



