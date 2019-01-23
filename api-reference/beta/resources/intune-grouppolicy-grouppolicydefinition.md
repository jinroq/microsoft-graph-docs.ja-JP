---
title: groupPolicyDefinition リソースの種類
description: エンティティでは、すべての単一のグループ ポリシーに関する情報について説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430491"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="9ec19-103">groupPolicyDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ec19-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="9ec19-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ec19-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ec19-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ec19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ec19-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ec19-107">エンティティでは、すべての単一のグループ ポリシーに関する情報について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9ec19-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ec19-108">Methods</span></span>
|<span data-ttu-id="9ec19-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ec19-109">Method</span></span>|<span data-ttu-id="9ec19-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9ec19-110">Return Type</span></span>|<span data-ttu-id="9ec19-111">説明</span><span class="sxs-lookup"><span data-stu-id="9ec19-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ec19-112">GroupPolicyDefinition を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="9ec19-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9ec19-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9ec19-114">[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ec19-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="9ec19-115">GroupPolicyDefinition を更新します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="9ec19-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9ec19-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9ec19-117">[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ec19-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ec19-118">Properties</span></span>
|<span data-ttu-id="9ec19-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ec19-119">Property</span></span>|<span data-ttu-id="9ec19-120">型</span><span class="sxs-lookup"><span data-stu-id="9ec19-120">Type</span></span>|<span data-ttu-id="9ec19-121">説明</span><span class="sxs-lookup"><span data-stu-id="9ec19-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec19-122">classType</span><span class="sxs-lookup"><span data-stu-id="9ec19-122">classType</span></span>|[<span data-ttu-id="9ec19-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="9ec19-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="9ec19-124">ポリシーを適用できるグループの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="9ec19-125">可能な値は、`user`、`machine`、`both` です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-125">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="9ec19-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9ec19-126">displayName</span></span>|<span data-ttu-id="9ec19-127">String</span><span class="sxs-lookup"><span data-stu-id="9ec19-127">String</span></span>|<span data-ttu-id="9ec19-128">ローカライズされたポリシーの名前です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-128">The localized policy name.</span></span>|
|<span data-ttu-id="9ec19-129">説明</span><span class="sxs-lookup"><span data-stu-id="9ec19-129">explainText</span></span>|<span data-ttu-id="9ec19-130">String</span><span class="sxs-lookup"><span data-stu-id="9ec19-130">String</span></span>|<span data-ttu-id="9ec19-131">ローカライズされた説明またはヘルプ テキスト、ポリシーに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="9ec19-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="9ec19-132">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-132">The default value is empty.</span></span>|
|<span data-ttu-id="9ec19-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="9ec19-133">categoryPath</span></span>|<span data-ttu-id="9ec19-134">String</span><span class="sxs-lookup"><span data-stu-id="9ec19-134">String</span></span>|<span data-ttu-id="9ec19-135">ポリシーのすべてのローカライズされたカテゴリのパスです。</span><span class="sxs-lookup"><span data-stu-id="9ec19-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="9ec19-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="9ec19-136">supportedOn</span></span>|<span data-ttu-id="9ec19-137">String</span><span class="sxs-lookup"><span data-stu-id="9ec19-137">String</span></span>|<span data-ttu-id="9ec19-138">どのようなオペレーティング システムまたはアプリケーションのバージョンを指定するために使用するローカライズされた文字列は、ポリシーの影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="9ec19-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="9ec19-139">policyType</span><span class="sxs-lookup"><span data-stu-id="9ec19-139">policyType</span></span>|[<span data-ttu-id="9ec19-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9ec19-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9ec19-141">グループ ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ec19-141">Specifies the type of group policy.</span></span> <span data-ttu-id="9ec19-142">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9ec19-143">id</span><span class="sxs-lookup"><span data-stu-id="9ec19-143">id</span></span>|<span data-ttu-id="9ec19-144">String</span><span class="sxs-lookup"><span data-stu-id="9ec19-144">String</span></span>|<span data-ttu-id="9ec19-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ec19-145">Key of the entity.</span></span>|
|<span data-ttu-id="9ec19-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec19-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9ec19-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec19-147">DateTimeOffset</span></span>|<span data-ttu-id="9ec19-148">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="9ec19-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ec19-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ec19-149">Relationships</span></span>
|<span data-ttu-id="9ec19-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ec19-150">Relationship</span></span>|<span data-ttu-id="9ec19-151">型</span><span class="sxs-lookup"><span data-stu-id="9ec19-151">Type</span></span>|<span data-ttu-id="9ec19-152">説明</span><span class="sxs-lookup"><span data-stu-id="9ec19-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec19-153">-definitionfile</span><span class="sxs-lookup"><span data-stu-id="9ec19-153">definitionFile</span></span>|[<span data-ttu-id="9ec19-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9ec19-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9ec19-155">定義に関連付けられているグループ ポリシー ファイルです。</span><span class="sxs-lookup"><span data-stu-id="9ec19-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="9ec19-156">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="9ec19-156">presentations</span></span>|<span data-ttu-id="9ec19-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9ec19-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="9ec19-158">定義に関連付けられているグループ ポリシーのプレゼンテーションです。</span><span class="sxs-lookup"><span data-stu-id="9ec19-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ec19-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ec19-159">JSON Representation</span></span>
<span data-ttu-id="9ec19-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ec19-160">Here is a JSON representation of the resource.</span></span>
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




