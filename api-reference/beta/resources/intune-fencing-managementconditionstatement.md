---
title: managementConditionStatement リソースの種類
description: 管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37718b5efaa34680f3b990fe61421d0faf24dac5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979173"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="7ef3b-103">managementConditionStatement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ef3b-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="7ef3b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ef3b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ef3b-106">管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-106">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="7ef3b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ef3b-107">Methods</span></span>
|<span data-ttu-id="7ef3b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ef3b-108">Method</span></span>|<span data-ttu-id="7ef3b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7ef3b-109">Return Type</span></span>|<span data-ttu-id="7ef3b-110">説明</span><span class="sxs-lookup"><span data-stu-id="7ef3b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ef3b-111">ManagementConditionStatements を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ef3b-111">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="7ef3b-112">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ef3b-112">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="7ef3b-113">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-113">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="7ef3b-114">ManagementConditionStatement の取得</span><span class="sxs-lookup"><span data-stu-id="7ef3b-114">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="7ef3b-115">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="7ef3b-115">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="7ef3b-116">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-116">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="7ef3b-117">ManagementConditionStatement の作成</span><span class="sxs-lookup"><span data-stu-id="7ef3b-117">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="7ef3b-118">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="7ef3b-118">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="7ef3b-119">新しい[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-119">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="7ef3b-120">ManagementConditionStatement の削除</span><span class="sxs-lookup"><span data-stu-id="7ef3b-120">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="7ef3b-121">None</span><span class="sxs-lookup"><span data-stu-id="7ef3b-121">None</span></span>|<span data-ttu-id="7ef3b-122">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-122">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="7ef3b-123">ManagementConditionStatement の更新</span><span class="sxs-lookup"><span data-stu-id="7ef3b-123">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="7ef3b-124">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="7ef3b-124">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="7ef3b-125">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-125">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="7ef3b-126">getManagementConditionStatementExpressionString 関数</span><span class="sxs-lookup"><span data-stu-id="7ef3b-126">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="7ef3b-127">Managementcondition式文字列</span><span class="sxs-lookup"><span data-stu-id="7ef3b-127">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="7ef3b-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ef3b-128">Not yet documented</span></span>|
|[<span data-ttu-id="7ef3b-129">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="7ef3b-129">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="7ef3b-130">[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ef3b-130">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="7ef3b-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ef3b-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7ef3b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ef3b-132">Properties</span></span>
|<span data-ttu-id="7ef3b-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ef3b-133">Property</span></span>|<span data-ttu-id="7ef3b-134">型</span><span class="sxs-lookup"><span data-stu-id="7ef3b-134">Type</span></span>|<span data-ttu-id="7ef3b-135">説明</span><span class="sxs-lookup"><span data-stu-id="7ef3b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef3b-136">id</span><span class="sxs-lookup"><span data-stu-id="7ef3b-136">id</span></span>|<span data-ttu-id="7ef3b-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7ef3b-137">String</span></span>|<span data-ttu-id="7ef3b-138">管理条件ステートメントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-138">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="7ef3b-139">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-139">System generated value assigned when created.</span></span>|
|<span data-ttu-id="7ef3b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7ef3b-140">displayName</span></span>|<span data-ttu-id="7ef3b-141">String</span><span class="sxs-lookup"><span data-stu-id="7ef3b-141">String</span></span>|<span data-ttu-id="7ef3b-142">管理条件ステートメントの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-142">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="7ef3b-143">description</span><span class="sxs-lookup"><span data-stu-id="7ef3b-143">description</span></span>|<span data-ttu-id="7ef3b-144">String</span><span class="sxs-lookup"><span data-stu-id="7ef3b-144">String</span></span>|<span data-ttu-id="7ef3b-145">管理条件ステートメントの管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-145">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="7ef3b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef3b-146">createdDateTime</span></span>|<span data-ttu-id="7ef3b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef3b-147">DateTimeOffset</span></span>|<span data-ttu-id="7ef3b-148">管理条件ステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-148">The time the management condition statement was created.</span></span> <span data-ttu-id="7ef3b-149">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-149">Generated service side.</span></span>|
|<span data-ttu-id="7ef3b-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef3b-150">modifiedDateTime</span></span>|<span data-ttu-id="7ef3b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef3b-151">DateTimeOffset</span></span>|<span data-ttu-id="7ef3b-152">管理条件ステートメントが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-152">The time the management condition statement was last modified.</span></span> <span data-ttu-id="7ef3b-153">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-153">Updated service side.</span></span>|
|<span data-ttu-id="7ef3b-154">式</span><span class="sxs-lookup"><span data-stu-id="7ef3b-154">expression</span></span>|[<span data-ttu-id="7ef3b-155">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="7ef3b-155">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="7ef3b-156">管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-156">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="7ef3b-157">eTag</span><span class="sxs-lookup"><span data-stu-id="7ef3b-157">eTag</span></span>|<span data-ttu-id="7ef3b-158">String</span><span class="sxs-lookup"><span data-stu-id="7ef3b-158">String</span></span>|<span data-ttu-id="7ef3b-159">管理条件ステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-159">ETag of the management condition statement.</span></span> <span data-ttu-id="7ef3b-160">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-160">Updated service side.</span></span>|
|<span data-ttu-id="7ef3b-161">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="7ef3b-161">applicablePlatforms</span></span>|<span data-ttu-id="7ef3b-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ef3b-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7ef3b-163">この管理条件ステートメントの適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-163">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="7ef3b-164">これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-164">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ef3b-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7ef3b-165">Relationships</span></span>
|<span data-ttu-id="7ef3b-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7ef3b-166">Relationship</span></span>|<span data-ttu-id="7ef3b-167">型</span><span class="sxs-lookup"><span data-stu-id="7ef3b-167">Type</span></span>|<span data-ttu-id="7ef3b-168">説明</span><span class="sxs-lookup"><span data-stu-id="7ef3b-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef3b-169">managementConditions</span><span class="sxs-lookup"><span data-stu-id="7ef3b-169">managementConditions</span></span>|<span data-ttu-id="7ef3b-170">[Managementcondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ef3b-170">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="7ef3b-171">管理条件ステートメントに関連付けられている管理条件。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-171">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ef3b-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ef3b-172">JSON Representation</span></span>
<span data-ttu-id="7ef3b-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7ef3b-173">Here is a JSON representation of the resource.</span></span>
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





