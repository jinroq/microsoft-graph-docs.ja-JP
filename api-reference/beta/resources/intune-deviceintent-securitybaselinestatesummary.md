---
title: securityBaselineStateSummary リソースの種類
description: アカウントのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e77ca9119a2a05b0719cd61bcf71c98a944b1e9e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319336"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="d1871-103">securityBaselineStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1871-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="d1871-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1871-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1871-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1871-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1871-106">アカウントのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。</span><span class="sxs-lookup"><span data-stu-id="d1871-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="d1871-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1871-107">Methods</span></span>
|<span data-ttu-id="d1871-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1871-108">Method</span></span>|<span data-ttu-id="d1871-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1871-109">Return Type</span></span>|<span data-ttu-id="d1871-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1871-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1871-111">SecurityBaselineStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="d1871-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="d1871-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1871-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="d1871-113">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d1871-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d1871-114">SecurityBaselineStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d1871-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="d1871-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1871-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="d1871-116">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1871-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1871-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1871-117">Properties</span></span>
|<span data-ttu-id="d1871-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1871-118">Property</span></span>|<span data-ttu-id="d1871-119">型</span><span class="sxs-lookup"><span data-stu-id="d1871-119">Type</span></span>|<span data-ttu-id="d1871-120">説明</span><span class="sxs-lookup"><span data-stu-id="d1871-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1871-121">id</span><span class="sxs-lookup"><span data-stu-id="d1871-121">id</span></span>|<span data-ttu-id="d1871-122">String</span><span class="sxs-lookup"><span data-stu-id="d1871-122">String</span></span>|<span data-ttu-id="d1871-123">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d1871-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d1871-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="d1871-124">secureCount</span></span>|<span data-ttu-id="d1871-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-125">Int32</span></span>|<span data-ttu-id="d1871-126">セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-126">Number of secure devices</span></span>|
|<span data-ttu-id="d1871-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="d1871-127">notSecureCount</span></span>|<span data-ttu-id="d1871-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-128">Int32</span></span>|<span data-ttu-id="d1871-129">セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-129">Number of not secure devices</span></span>|
|<span data-ttu-id="d1871-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d1871-130">unknownCount</span></span>|<span data-ttu-id="d1871-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-131">Int32</span></span>|<span data-ttu-id="d1871-132">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-132">Number of unknown devices</span></span>|
|<span data-ttu-id="d1871-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="d1871-133">errorCount</span></span>|<span data-ttu-id="d1871-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-134">Int32</span></span>|<span data-ttu-id="d1871-135">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-135">Number of error devices</span></span>|
|<span data-ttu-id="d1871-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d1871-136">conflictCount</span></span>|<span data-ttu-id="d1871-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-137">Int32</span></span>|<span data-ttu-id="d1871-138">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-138">Number of conflict devices</span></span>|
|<span data-ttu-id="d1871-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d1871-139">notApplicableCount</span></span>|<span data-ttu-id="d1871-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-140">Int32</span></span>|<span data-ttu-id="d1871-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1871-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1871-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1871-142">Relationships</span></span>
<span data-ttu-id="d1871-143">なし</span><span class="sxs-lookup"><span data-stu-id="d1871-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1871-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1871-144">JSON Representation</span></span>
<span data-ttu-id="d1871-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1871-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```



