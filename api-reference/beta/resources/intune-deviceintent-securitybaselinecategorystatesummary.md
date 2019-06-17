---
title: securityBaselineCategoryStateSummary リソースの種類
description: アカウントのセキュリティベースラインのカテゴリコンプライアンスの状態の要約ごとのセキュリティ基準。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00735cb51952ec9cc8104a1d2f142d74cb773e05
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983450"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a><span data-ttu-id="6a98d-103">securityBaselineCategoryStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a98d-103">securityBaselineCategoryStateSummary resource type</span></span>

> <span data-ttu-id="6a98d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a98d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a98d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a98d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a98d-106">アカウントのセキュリティベースラインのカテゴリコンプライアンスの状態の要約ごとのセキュリティ基準。</span><span class="sxs-lookup"><span data-stu-id="6a98d-106">The security baseline per category compliance state summary for the security baseline of the account.</span></span>


<span data-ttu-id="6a98d-107">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a98d-107">Inherits from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6a98d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a98d-108">Methods</span></span>
|<span data-ttu-id="6a98d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a98d-109">Method</span></span>|<span data-ttu-id="6a98d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a98d-110">Return Type</span></span>|<span data-ttu-id="6a98d-111">説明</span><span class="sxs-lookup"><span data-stu-id="6a98d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a98d-112">リスト securityBaselineCategoryStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6a98d-112">List securityBaselineCategoryStateSummaries</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|<span data-ttu-id="6a98d-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a98d-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) collection</span></span>|<span data-ttu-id="6a98d-114">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6a98d-114">List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects.</span></span>|
|[<span data-ttu-id="6a98d-115">SecurityBaselineCategoryStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="6a98d-115">Get securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[<span data-ttu-id="6a98d-116">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="6a98d-116">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="6a98d-117">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6a98d-117">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="6a98d-118">SecurityBaselineCategoryStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="6a98d-118">Create securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[<span data-ttu-id="6a98d-119">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="6a98d-119">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="6a98d-120">新しい[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a98d-120">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="6a98d-121">SecurityBaselineCategoryStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="6a98d-121">Delete securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|<span data-ttu-id="6a98d-122">None</span><span class="sxs-lookup"><span data-stu-id="6a98d-122">None</span></span>|<span data-ttu-id="6a98d-123">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a98d-123">Deletes a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>|
|[<span data-ttu-id="6a98d-124">SecurityBaselineCategoryStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="6a98d-124">Update securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[<span data-ttu-id="6a98d-125">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="6a98d-125">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="6a98d-126">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a98d-126">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a98d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a98d-127">Properties</span></span>
|<span data-ttu-id="6a98d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a98d-128">Property</span></span>|<span data-ttu-id="6a98d-129">型</span><span class="sxs-lookup"><span data-stu-id="6a98d-129">Type</span></span>|<span data-ttu-id="6a98d-130">説明</span><span class="sxs-lookup"><span data-stu-id="6a98d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a98d-131">id</span><span class="sxs-lookup"><span data-stu-id="6a98d-131">id</span></span>|<span data-ttu-id="6a98d-132">文字列</span><span class="sxs-lookup"><span data-stu-id="6a98d-132">String</span></span>|<span data-ttu-id="6a98d-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6a98d-133">Unique identifier of the entity.</span></span> <span data-ttu-id="6a98d-134">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a98d-134">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-135">secureCount</span></span>|<span data-ttu-id="6a98d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-136">Int32</span></span>|<span data-ttu-id="6a98d-137">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-137">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-138">notSecureCount</span></span>|<span data-ttu-id="6a98d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-139">Int32</span></span>|<span data-ttu-id="6a98d-140">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-140">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-141">unknownCount</span></span>|<span data-ttu-id="6a98d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-142">Int32</span></span>|<span data-ttu-id="6a98d-143">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-143">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-144">errorCount</span></span>|<span data-ttu-id="6a98d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-145">Int32</span></span>|<span data-ttu-id="6a98d-146">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承されたエラーデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-146">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-147">conflictCount</span></span>|<span data-ttu-id="6a98d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-148">Int32</span></span>|<span data-ttu-id="6a98d-149">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-149">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6a98d-150">notApplicableCount</span></span>|<span data-ttu-id="6a98d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98d-151">Int32</span></span>|<span data-ttu-id="6a98d-152">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された、適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6a98d-152">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="6a98d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6a98d-153">displayName</span></span>|<span data-ttu-id="6a98d-154">String</span><span class="sxs-lookup"><span data-stu-id="6a98d-154">String</span></span>|<span data-ttu-id="6a98d-155">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="6a98d-155">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a98d-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a98d-156">Relationships</span></span>
<span data-ttu-id="6a98d-157">なし</span><span class="sxs-lookup"><span data-stu-id="6a98d-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a98d-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a98d-158">JSON Representation</span></span>
<span data-ttu-id="6a98d-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a98d-159">Here is a JSON representation of the resource.</span></span>
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





