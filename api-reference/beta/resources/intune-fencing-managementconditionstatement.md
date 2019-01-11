---
title: managementConditionStatement リソースの種類
description: 管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c6281d151555c0c58a0eb608e9dafc754384369f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878401"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="6fc2f-103">managementConditionStatement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6fc2f-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="6fc2f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fc2f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fc2f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fc2f-107">管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>
## <a name="methods"></a><span data-ttu-id="6fc2f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fc2f-108">Methods</span></span>
|<span data-ttu-id="6fc2f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fc2f-109">Method</span></span>|<span data-ttu-id="6fc2f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-110">Return Type</span></span>|<span data-ttu-id="6fc2f-111">説明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fc2f-112">リスト managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="6fc2f-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="6fc2f-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6fc2f-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="6fc2f-114">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="6fc2f-115">ManagementConditionStatement を取得します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="6fc2f-116">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="6fc2f-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="6fc2f-117">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="6fc2f-118">ManagementConditionStatement を作成します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="6fc2f-119">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="6fc2f-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="6fc2f-120">新しい[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="6fc2f-121">ManagementConditionStatement を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="6fc2f-122">なし</span><span class="sxs-lookup"><span data-stu-id="6fc2f-122">None</span></span>|<span data-ttu-id="6fc2f-123">の[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="6fc2f-124">ManagementConditionStatement を更新します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="6fc2f-125">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="6fc2f-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="6fc2f-126">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="6fc2f-127">getManagementConditionStatementExpressionString 関数</span><span class="sxs-lookup"><span data-stu-id="6fc2f-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="6fc2f-128">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="6fc2f-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="6fc2f-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6fc2f-129">Not yet documented</span></span>|
|[<span data-ttu-id="6fc2f-130">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="6fc2f-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="6fc2f-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6fc2f-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="6fc2f-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6fc2f-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6fc2f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fc2f-133">Properties</span></span>
|<span data-ttu-id="6fc2f-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fc2f-134">Property</span></span>|<span data-ttu-id="6fc2f-135">種類</span><span class="sxs-lookup"><span data-stu-id="6fc2f-135">Type</span></span>|<span data-ttu-id="6fc2f-136">説明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc2f-137">ID</span><span class="sxs-lookup"><span data-stu-id="6fc2f-137">id</span></span>|<span data-ttu-id="6fc2f-138">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-138">String</span></span>|<span data-ttu-id="6fc2f-139">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="6fc2f-140">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="6fc2f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6fc2f-141">displayName</span></span>|<span data-ttu-id="6fc2f-142">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-142">String</span></span>|<span data-ttu-id="6fc2f-143">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="6fc2f-144">説明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-144">description</span></span>|<span data-ttu-id="6fc2f-145">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-145">String</span></span>|<span data-ttu-id="6fc2f-146">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="6fc2f-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc2f-147">createdDateTime</span></span>|<span data-ttu-id="6fc2f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc2f-148">DateTimeOffset</span></span>|<span data-ttu-id="6fc2f-149">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-149">The time the management condition statement was created.</span></span> <span data-ttu-id="6fc2f-150">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-150">Generated service side.</span></span>|
|<span data-ttu-id="6fc2f-151">変更された日時</span><span class="sxs-lookup"><span data-stu-id="6fc2f-151">modifiedDateTime</span></span>|<span data-ttu-id="6fc2f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc2f-152">DateTimeOffset</span></span>|<span data-ttu-id="6fc2f-153">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="6fc2f-154">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-154">Updated service side.</span></span>|
|<span data-ttu-id="6fc2f-155">式</span><span class="sxs-lookup"><span data-stu-id="6fc2f-155">expression</span></span>|[<span data-ttu-id="6fc2f-156">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="6fc2f-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="6fc2f-157">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="6fc2f-158">eTag</span><span class="sxs-lookup"><span data-stu-id="6fc2f-158">eTag</span></span>|<span data-ttu-id="6fc2f-159">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-159">String</span></span>|<span data-ttu-id="6fc2f-160">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-160">ETag of the management condition statement.</span></span> <span data-ttu-id="6fc2f-161">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-161">Updated service side.</span></span>|
|<span data-ttu-id="6fc2f-162">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="6fc2f-162">applicablePlatforms</span></span>|<span data-ttu-id="6fc2f-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6fc2f-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="6fc2f-164">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="6fc2f-165">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fc2f-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6fc2f-166">Relationships</span></span>
|<span data-ttu-id="6fc2f-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6fc2f-167">Relationship</span></span>|<span data-ttu-id="6fc2f-168">型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-168">Type</span></span>|<span data-ttu-id="6fc2f-169">説明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc2f-170">managementConditions</span><span class="sxs-lookup"><span data-stu-id="6fc2f-170">managementConditions</span></span>|<span data-ttu-id="6fc2f-171">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6fc2f-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="6fc2f-172">管理条件ステートメントに関連付けられている管理の条件です。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc2f-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fc2f-173">JSON Representation</span></span>
<span data-ttu-id="6fc2f-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-174">Here is a JSON representation of the resource.</span></span>
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





