---
title: groupPolicyPresentationValueList リソースの種類
description: エンティティは、ポリシー定義のリストボックスプレゼンテーションの名前と値のペアのコレクションを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6e0821ed276657fae6469cd4eb6541569df1b3f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941031"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a><span data-ttu-id="b9357-103">groupPolicyPresentationValueList リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9357-103">groupPolicyPresentationValueList resource type</span></span>

> <span data-ttu-id="b9357-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9357-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9357-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9357-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9357-106">エンティティは、ポリシー定義のリストボックスプレゼンテーションの名前と値のペアのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="b9357-106">The entity represents a collection of name/value pairs of a list box presentation on a policy definition.</span></span>


<span data-ttu-id="b9357-107">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b9357-107">Inherits from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b9357-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9357-108">Methods</span></span>
|<span data-ttu-id="b9357-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9357-109">Method</span></span>|<span data-ttu-id="b9357-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b9357-110">Return Type</span></span>|<span data-ttu-id="b9357-111">説明</span><span class="sxs-lookup"><span data-stu-id="b9357-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9357-112">GroupPolicyPresentationValueLists のリスト</span><span class="sxs-lookup"><span data-stu-id="b9357-112">List groupPolicyPresentationValueLists</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|<span data-ttu-id="b9357-113">[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b9357-113">[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) collection</span></span>|<span data-ttu-id="b9357-114">[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b9357-114">List properties and relationships of the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) objects.</span></span>|
|[<span data-ttu-id="b9357-115">GroupPolicyPresentationValueList の取得</span><span class="sxs-lookup"><span data-stu-id="b9357-115">Get groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[<span data-ttu-id="b9357-116">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b9357-116">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b9357-117">[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b9357-117">Read properties and relationships of the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|
|[<span data-ttu-id="b9357-118">GroupPolicyPresentationValueList の作成</span><span class="sxs-lookup"><span data-stu-id="b9357-118">Create groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[<span data-ttu-id="b9357-119">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b9357-119">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b9357-120">新しい[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b9357-120">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|
|[<span data-ttu-id="b9357-121">GroupPolicyPresentationValueList の削除</span><span class="sxs-lookup"><span data-stu-id="b9357-121">Delete groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|<span data-ttu-id="b9357-122">None</span><span class="sxs-lookup"><span data-stu-id="b9357-122">None</span></span>|<span data-ttu-id="b9357-123">[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b9357-123">Deletes a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>|
|[<span data-ttu-id="b9357-124">GroupPolicyPresentationValueList の更新</span><span class="sxs-lookup"><span data-stu-id="b9357-124">Update groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[<span data-ttu-id="b9357-125">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b9357-125">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b9357-126">[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9357-126">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9357-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9357-127">Properties</span></span>
|<span data-ttu-id="b9357-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9357-128">Property</span></span>|<span data-ttu-id="b9357-129">種類</span><span class="sxs-lookup"><span data-stu-id="b9357-129">Type</span></span>|<span data-ttu-id="b9357-130">説明</span><span class="sxs-lookup"><span data-stu-id="b9357-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9357-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9357-131">lastModifiedDateTime</span></span>|<span data-ttu-id="b9357-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9357-132">DateTimeOffset</span></span>|<span data-ttu-id="b9357-133">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="b9357-133">The date and time the object was last modified.</span></span> <span data-ttu-id="b9357-134">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b9357-134">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9357-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9357-135">createdDateTime</span></span>|<span data-ttu-id="b9357-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9357-136">DateTimeOffset</span></span>|<span data-ttu-id="b9357-137">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="b9357-137">The date and time the object was created.</span></span> <span data-ttu-id="b9357-138">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b9357-138">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9357-139">id</span><span class="sxs-lookup"><span data-stu-id="b9357-139">id</span></span>|<span data-ttu-id="b9357-140">String</span><span class="sxs-lookup"><span data-stu-id="b9357-140">String</span></span>|<span data-ttu-id="b9357-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b9357-141">Key of the entity.</span></span> <span data-ttu-id="b9357-142">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b9357-142">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9357-143">values</span><span class="sxs-lookup"><span data-stu-id="b9357-143">values</span></span>|<span data-ttu-id="b9357-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b9357-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b9357-145">関連付けられているプレゼンテーションのペアのリスト。</span><span class="sxs-lookup"><span data-stu-id="b9357-145">A list of pairs for the associated presentation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9357-146">関係</span><span class="sxs-lookup"><span data-stu-id="b9357-146">Relationships</span></span>
|<span data-ttu-id="b9357-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9357-147">Relationship</span></span>|<span data-ttu-id="b9357-148">型</span><span class="sxs-lookup"><span data-stu-id="b9357-148">Type</span></span>|<span data-ttu-id="b9357-149">説明</span><span class="sxs-lookup"><span data-stu-id="b9357-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9357-150">definitionValue</span><span class="sxs-lookup"><span data-stu-id="b9357-150">definitionValue</span></span>|[<span data-ttu-id="b9357-151">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="b9357-151">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="b9357-152">プレゼンテーション値に関連付けられているグループポリシー定義の値。</span><span class="sxs-lookup"><span data-stu-id="b9357-152">The group policy definition value associated with the presentation value.</span></span> <span data-ttu-id="b9357-153">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b9357-153">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9357-154">プレゼンテーション</span><span class="sxs-lookup"><span data-stu-id="b9357-154">presentation</span></span>|[<span data-ttu-id="b9357-155">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="b9357-155">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="b9357-156">プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。</span><span class="sxs-lookup"><span data-stu-id="b9357-156">The group policy presentation associated with the presentation value.</span></span> <span data-ttu-id="b9357-157">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b9357-157">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9357-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9357-158">JSON Representation</span></span>
<span data-ttu-id="b9357-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9357-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




