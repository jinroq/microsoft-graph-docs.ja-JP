---
title: securityBaselineCategoryStateSummary リソースの種類
description: アカウントのセキュリティベースラインのカテゴリコンプライアンスの状態の要約ごとのセキュリティ基準。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd8f40c2997e512f690dcb48908f22b80d7e34c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957055"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a><span data-ttu-id="36710-103">securityBaselineCategoryStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36710-103">securityBaselineCategoryStateSummary resource type</span></span>

> <span data-ttu-id="36710-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36710-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36710-106">アカウントのセキュリティベースラインのカテゴリコンプライアンスの状態の要約ごとのセキュリティ基準。</span><span class="sxs-lookup"><span data-stu-id="36710-106">The security baseline per category compliance state summary for the security baseline of the account.</span></span>


<span data-ttu-id="36710-107">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="36710-107">Inherits from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>

## <a name="methods"></a><span data-ttu-id="36710-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="36710-108">Methods</span></span>
|<span data-ttu-id="36710-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="36710-109">Method</span></span>|<span data-ttu-id="36710-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="36710-110">Return Type</span></span>|<span data-ttu-id="36710-111">説明</span><span class="sxs-lookup"><span data-stu-id="36710-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36710-112">リスト securityBaselineCategoryStateSummaries</span><span class="sxs-lookup"><span data-stu-id="36710-112">List securityBaselineCategoryStateSummaries</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|<span data-ttu-id="36710-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="36710-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) collection</span></span>|<span data-ttu-id="36710-114">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="36710-114">List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects.</span></span>|
|[<span data-ttu-id="36710-115">SecurityBaselineCategoryStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="36710-115">Get securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[<span data-ttu-id="36710-116">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="36710-116">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="36710-117">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="36710-117">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="36710-118">SecurityBaselineCategoryStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="36710-118">Create securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[<span data-ttu-id="36710-119">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="36710-119">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="36710-120">新しい[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="36710-120">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="36710-121">SecurityBaselineCategoryStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="36710-121">Delete securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|<span data-ttu-id="36710-122">None</span><span class="sxs-lookup"><span data-stu-id="36710-122">None</span></span>|<span data-ttu-id="36710-123">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="36710-123">Deletes a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>|
|[<span data-ttu-id="36710-124">SecurityBaselineCategoryStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="36710-124">Update securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[<span data-ttu-id="36710-125">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="36710-125">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="36710-126">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="36710-126">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36710-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36710-127">Properties</span></span>
|<span data-ttu-id="36710-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36710-128">Property</span></span>|<span data-ttu-id="36710-129">型</span><span class="sxs-lookup"><span data-stu-id="36710-129">Type</span></span>|<span data-ttu-id="36710-130">説明</span><span class="sxs-lookup"><span data-stu-id="36710-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36710-131">id</span><span class="sxs-lookup"><span data-stu-id="36710-131">id</span></span>|<span data-ttu-id="36710-132">文字列</span><span class="sxs-lookup"><span data-stu-id="36710-132">String</span></span>|<span data-ttu-id="36710-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="36710-133">Unique identifier of the entity.</span></span> <span data-ttu-id="36710-134">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="36710-134">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="36710-135">secureCount</span></span>|<span data-ttu-id="36710-136">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-136">Int32</span></span>|<span data-ttu-id="36710-137">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-137">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="36710-138">notSecureCount</span></span>|<span data-ttu-id="36710-139">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-139">Int32</span></span>|<span data-ttu-id="36710-140">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-140">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="36710-141">unknownCount</span></span>|<span data-ttu-id="36710-142">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-142">Int32</span></span>|<span data-ttu-id="36710-143">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-143">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="36710-144">errorCount</span></span>|<span data-ttu-id="36710-145">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-145">Int32</span></span>|<span data-ttu-id="36710-146">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承されたエラーデバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-146">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="36710-147">conflictCount</span></span>|<span data-ttu-id="36710-148">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-148">Int32</span></span>|<span data-ttu-id="36710-149">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-149">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="36710-150">notApplicableCount</span></span>|<span data-ttu-id="36710-151">Int32</span><span class="sxs-lookup"><span data-stu-id="36710-151">Int32</span></span>|<span data-ttu-id="36710-152">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された、適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="36710-152">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="36710-153">displayName</span><span class="sxs-lookup"><span data-stu-id="36710-153">displayName</span></span>|<span data-ttu-id="36710-154">String</span><span class="sxs-lookup"><span data-stu-id="36710-154">String</span></span>|<span data-ttu-id="36710-155">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="36710-155">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="36710-156">関係</span><span class="sxs-lookup"><span data-stu-id="36710-156">Relationships</span></span>
<span data-ttu-id="36710-157">なし</span><span class="sxs-lookup"><span data-stu-id="36710-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36710-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36710-158">JSON Representation</span></span>
<span data-ttu-id="36710-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36710-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```




