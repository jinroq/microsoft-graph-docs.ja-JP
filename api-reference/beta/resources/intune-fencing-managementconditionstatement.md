---
title: managementConditionStatement リソースの種類
description: 管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3292dae241a3f79cc7d3417c93ccc1187c8b8d17
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395994"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="83310-103">managementConditionStatement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83310-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="83310-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83310-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83310-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83310-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83310-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83310-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83310-107">管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。</span><span class="sxs-lookup"><span data-stu-id="83310-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="83310-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="83310-108">Methods</span></span>
|<span data-ttu-id="83310-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="83310-109">Method</span></span>|<span data-ttu-id="83310-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="83310-110">Return Type</span></span>|<span data-ttu-id="83310-111">説明</span><span class="sxs-lookup"><span data-stu-id="83310-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83310-112">リスト managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="83310-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="83310-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="83310-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="83310-114">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="83310-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="83310-115">ManagementConditionStatement を取得します。</span><span class="sxs-lookup"><span data-stu-id="83310-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="83310-116">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="83310-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="83310-117">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83310-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="83310-118">ManagementConditionStatement を作成します。</span><span class="sxs-lookup"><span data-stu-id="83310-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="83310-119">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="83310-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="83310-120">新しい[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="83310-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="83310-121">ManagementConditionStatement を削除します。</span><span class="sxs-lookup"><span data-stu-id="83310-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="83310-122">なし</span><span class="sxs-lookup"><span data-stu-id="83310-122">None</span></span>|<span data-ttu-id="83310-123">の[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="83310-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="83310-124">ManagementConditionStatement を更新します。</span><span class="sxs-lookup"><span data-stu-id="83310-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="83310-125">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="83310-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="83310-126">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83310-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="83310-127">getManagementConditionStatementExpressionString 関数</span><span class="sxs-lookup"><span data-stu-id="83310-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="83310-128">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="83310-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="83310-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83310-129">Not yet documented</span></span>|
|[<span data-ttu-id="83310-130">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="83310-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="83310-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="83310-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="83310-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83310-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="83310-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83310-133">Properties</span></span>
|<span data-ttu-id="83310-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83310-134">Property</span></span>|<span data-ttu-id="83310-135">型</span><span class="sxs-lookup"><span data-stu-id="83310-135">Type</span></span>|<span data-ttu-id="83310-136">説明</span><span class="sxs-lookup"><span data-stu-id="83310-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83310-137">id</span><span class="sxs-lookup"><span data-stu-id="83310-137">id</span></span>|<span data-ttu-id="83310-138">String</span><span class="sxs-lookup"><span data-stu-id="83310-138">String</span></span>|<span data-ttu-id="83310-139">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="83310-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="83310-140">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="83310-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="83310-141">displayName</span><span class="sxs-lookup"><span data-stu-id="83310-141">displayName</span></span>|<span data-ttu-id="83310-142">String</span><span class="sxs-lookup"><span data-stu-id="83310-142">String</span></span>|<span data-ttu-id="83310-143">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="83310-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="83310-144">説明</span><span class="sxs-lookup"><span data-stu-id="83310-144">description</span></span>|<span data-ttu-id="83310-145">String</span><span class="sxs-lookup"><span data-stu-id="83310-145">String</span></span>|<span data-ttu-id="83310-146">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="83310-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="83310-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83310-147">createdDateTime</span></span>|<span data-ttu-id="83310-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83310-148">DateTimeOffset</span></span>|<span data-ttu-id="83310-149">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="83310-149">The time the management condition statement was created.</span></span> <span data-ttu-id="83310-150">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="83310-150">Generated service side.</span></span>|
|<span data-ttu-id="83310-151">変更された日時</span><span class="sxs-lookup"><span data-stu-id="83310-151">modifiedDateTime</span></span>|<span data-ttu-id="83310-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83310-152">DateTimeOffset</span></span>|<span data-ttu-id="83310-153">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="83310-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="83310-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="83310-154">Updated service side.</span></span>|
|<span data-ttu-id="83310-155">式</span><span class="sxs-lookup"><span data-stu-id="83310-155">expression</span></span>|[<span data-ttu-id="83310-156">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="83310-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="83310-157">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="83310-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="83310-158">eTag</span><span class="sxs-lookup"><span data-stu-id="83310-158">eTag</span></span>|<span data-ttu-id="83310-159">String</span><span class="sxs-lookup"><span data-stu-id="83310-159">String</span></span>|<span data-ttu-id="83310-160">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="83310-160">ETag of the management condition statement.</span></span> <span data-ttu-id="83310-161">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="83310-161">Updated service side.</span></span>|
|<span data-ttu-id="83310-162">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="83310-162">applicablePlatforms</span></span>|<span data-ttu-id="83310-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="83310-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="83310-164">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="83310-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="83310-165">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="83310-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83310-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83310-166">Relationships</span></span>
|<span data-ttu-id="83310-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83310-167">Relationship</span></span>|<span data-ttu-id="83310-168">型</span><span class="sxs-lookup"><span data-stu-id="83310-168">Type</span></span>|<span data-ttu-id="83310-169">説明</span><span class="sxs-lookup"><span data-stu-id="83310-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83310-170">managementConditions</span><span class="sxs-lookup"><span data-stu-id="83310-170">managementConditions</span></span>|<span data-ttu-id="83310-171">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="83310-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="83310-172">管理条件ステートメントに関連付けられている管理の条件です。</span><span class="sxs-lookup"><span data-stu-id="83310-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83310-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83310-173">JSON Representation</span></span>
<span data-ttu-id="83310-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83310-174">Here is a JSON representation of the resource.</span></span>
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




