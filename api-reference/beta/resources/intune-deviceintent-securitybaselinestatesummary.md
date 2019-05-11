---
title: securityBaselineStateSummary リソースの種類
description: アカウントのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c7c1cf31ddca02348eed55b9dc19dd5420b016e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943271"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="ddd70-103">securityBaselineStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddd70-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="ddd70-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddd70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddd70-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ddd70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddd70-106">アカウントのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。</span><span class="sxs-lookup"><span data-stu-id="ddd70-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="ddd70-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddd70-107">Methods</span></span>
|<span data-ttu-id="ddd70-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddd70-108">Method</span></span>|<span data-ttu-id="ddd70-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ddd70-109">Return Type</span></span>|<span data-ttu-id="ddd70-110">説明</span><span class="sxs-lookup"><span data-stu-id="ddd70-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddd70-111">SecurityBaselineStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="ddd70-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="ddd70-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="ddd70-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="ddd70-113">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ddd70-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="ddd70-114">SecurityBaselineStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="ddd70-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="ddd70-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="ddd70-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="ddd70-116">[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ddd70-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddd70-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddd70-117">Properties</span></span>
|<span data-ttu-id="ddd70-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddd70-118">Property</span></span>|<span data-ttu-id="ddd70-119">型</span><span class="sxs-lookup"><span data-stu-id="ddd70-119">Type</span></span>|<span data-ttu-id="ddd70-120">説明</span><span class="sxs-lookup"><span data-stu-id="ddd70-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd70-121">id</span><span class="sxs-lookup"><span data-stu-id="ddd70-121">id</span></span>|<span data-ttu-id="ddd70-122">String</span><span class="sxs-lookup"><span data-stu-id="ddd70-122">String</span></span>|<span data-ttu-id="ddd70-123">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ddd70-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ddd70-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-124">secureCount</span></span>|<span data-ttu-id="ddd70-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-125">Int32</span></span>|<span data-ttu-id="ddd70-126">セキュリティで保護されたデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-126">Number of secure devices</span></span>|
|<span data-ttu-id="ddd70-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-127">notSecureCount</span></span>|<span data-ttu-id="ddd70-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-128">Int32</span></span>|<span data-ttu-id="ddd70-129">セキュリティで保護されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-129">Number of not secure devices</span></span>|
|<span data-ttu-id="ddd70-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-130">unknownCount</span></span>|<span data-ttu-id="ddd70-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-131">Int32</span></span>|<span data-ttu-id="ddd70-132">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-132">Number of unknown devices</span></span>|
|<span data-ttu-id="ddd70-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-133">errorCount</span></span>|<span data-ttu-id="ddd70-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-134">Int32</span></span>|<span data-ttu-id="ddd70-135">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-135">Number of error devices</span></span>|
|<span data-ttu-id="ddd70-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-136">conflictCount</span></span>|<span data-ttu-id="ddd70-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-137">Int32</span></span>|<span data-ttu-id="ddd70-138">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-138">Number of conflict devices</span></span>|
|<span data-ttu-id="ddd70-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ddd70-139">notApplicableCount</span></span>|<span data-ttu-id="ddd70-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd70-140">Int32</span></span>|<span data-ttu-id="ddd70-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ddd70-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddd70-142">関係</span><span class="sxs-lookup"><span data-stu-id="ddd70-142">Relationships</span></span>
<span data-ttu-id="ddd70-143">なし</span><span class="sxs-lookup"><span data-stu-id="ddd70-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddd70-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddd70-144">JSON Representation</span></span>
<span data-ttu-id="ddd70-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddd70-145">Here is a JSON representation of the resource.</span></span>
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




