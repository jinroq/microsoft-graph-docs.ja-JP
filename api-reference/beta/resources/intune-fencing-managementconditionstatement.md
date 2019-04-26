---
title: managementconditionstatement リソースの種類
description: 管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a90d17bd56a2fbb957bdde5ba8b159baeb3ae2e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568753"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="33307-103">managementconditionstatement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33307-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="33307-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33307-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33307-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33307-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33307-106">管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。</span><span class="sxs-lookup"><span data-stu-id="33307-106">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="33307-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="33307-107">Methods</span></span>
|<span data-ttu-id="33307-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="33307-108">Method</span></span>|<span data-ttu-id="33307-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="33307-109">Return Type</span></span>|<span data-ttu-id="33307-110">説明</span><span class="sxs-lookup"><span data-stu-id="33307-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33307-111">managementconditionstatements を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="33307-111">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="33307-112">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33307-112">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="33307-113">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="33307-113">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="33307-114">managementconditionstatement の取得</span><span class="sxs-lookup"><span data-stu-id="33307-114">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="33307-115">managementconditionstatement</span><span class="sxs-lookup"><span data-stu-id="33307-115">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="33307-116">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="33307-116">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="33307-117">managementconditionstatement の作成</span><span class="sxs-lookup"><span data-stu-id="33307-117">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="33307-118">managementconditionstatement</span><span class="sxs-lookup"><span data-stu-id="33307-118">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="33307-119">新しい[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="33307-119">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="33307-120">managementconditionstatement の削除</span><span class="sxs-lookup"><span data-stu-id="33307-120">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="33307-121">なし</span><span class="sxs-lookup"><span data-stu-id="33307-121">None</span></span>|<span data-ttu-id="33307-122">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="33307-122">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="33307-123">managementconditionstatement の更新</span><span class="sxs-lookup"><span data-stu-id="33307-123">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="33307-124">managementconditionstatement</span><span class="sxs-lookup"><span data-stu-id="33307-124">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="33307-125">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33307-125">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="33307-126">getManagementConditionStatementExpressionString 関数</span><span class="sxs-lookup"><span data-stu-id="33307-126">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="33307-127">managementcondition式文字列</span><span class="sxs-lookup"><span data-stu-id="33307-127">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="33307-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33307-128">Not yet documented</span></span>|
|[<span data-ttu-id="33307-129">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="33307-129">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="33307-130">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33307-130">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="33307-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33307-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="33307-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33307-132">Properties</span></span>
|<span data-ttu-id="33307-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33307-133">Property</span></span>|<span data-ttu-id="33307-134">型</span><span class="sxs-lookup"><span data-stu-id="33307-134">Type</span></span>|<span data-ttu-id="33307-135">説明</span><span class="sxs-lookup"><span data-stu-id="33307-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33307-136">id</span><span class="sxs-lookup"><span data-stu-id="33307-136">id</span></span>|<span data-ttu-id="33307-137">String</span><span class="sxs-lookup"><span data-stu-id="33307-137">String</span></span>|<span data-ttu-id="33307-138">管理条件ステートメントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="33307-138">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="33307-139">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="33307-139">System generated value assigned when created.</span></span>|
|<span data-ttu-id="33307-140">displayName</span><span class="sxs-lookup"><span data-stu-id="33307-140">displayName</span></span>|<span data-ttu-id="33307-141">String</span><span class="sxs-lookup"><span data-stu-id="33307-141">String</span></span>|<span data-ttu-id="33307-142">管理条件ステートメントの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="33307-142">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="33307-143">説明</span><span class="sxs-lookup"><span data-stu-id="33307-143">description</span></span>|<span data-ttu-id="33307-144">String</span><span class="sxs-lookup"><span data-stu-id="33307-144">String</span></span>|<span data-ttu-id="33307-145">管理条件ステートメントの管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="33307-145">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="33307-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33307-146">createdDateTime</span></span>|<span data-ttu-id="33307-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33307-147">DateTimeOffset</span></span>|<span data-ttu-id="33307-148">管理条件ステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="33307-148">The time the management condition statement was created.</span></span> <span data-ttu-id="33307-149">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="33307-149">Generated service side.</span></span>|
|<span data-ttu-id="33307-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33307-150">modifiedDateTime</span></span>|<span data-ttu-id="33307-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33307-151">DateTimeOffset</span></span>|<span data-ttu-id="33307-152">管理条件ステートメントが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="33307-152">The time the management condition statement was last modified.</span></span> <span data-ttu-id="33307-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="33307-153">Updated service side.</span></span>|
|<span data-ttu-id="33307-154">式</span><span class="sxs-lookup"><span data-stu-id="33307-154">expression</span></span>|[<span data-ttu-id="33307-155">managementconditionexpression</span><span class="sxs-lookup"><span data-stu-id="33307-155">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="33307-156">管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。</span><span class="sxs-lookup"><span data-stu-id="33307-156">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="33307-157">eTag</span><span class="sxs-lookup"><span data-stu-id="33307-157">eTag</span></span>|<span data-ttu-id="33307-158">String</span><span class="sxs-lookup"><span data-stu-id="33307-158">String</span></span>|<span data-ttu-id="33307-159">管理条件ステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="33307-159">ETag of the management condition statement.</span></span> <span data-ttu-id="33307-160">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="33307-160">Updated service side.</span></span>|
|<span data-ttu-id="33307-161">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="33307-161">applicablePlatforms</span></span>|<span data-ttu-id="33307-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33307-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="33307-163">この管理条件ステートメントの適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="33307-163">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="33307-164">これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。</span><span class="sxs-lookup"><span data-stu-id="33307-164">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33307-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33307-165">Relationships</span></span>
|<span data-ttu-id="33307-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33307-166">Relationship</span></span>|<span data-ttu-id="33307-167">型</span><span class="sxs-lookup"><span data-stu-id="33307-167">Type</span></span>|<span data-ttu-id="33307-168">説明</span><span class="sxs-lookup"><span data-stu-id="33307-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33307-169">managementconditions</span><span class="sxs-lookup"><span data-stu-id="33307-169">managementConditions</span></span>|<span data-ttu-id="33307-170">[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33307-170">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="33307-171">管理条件ステートメントに関連付けられている管理条件。</span><span class="sxs-lookup"><span data-stu-id="33307-171">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33307-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33307-172">JSON Representation</span></span>
<span data-ttu-id="33307-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="33307-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





