---
title: devicemanagementトラブルシューティングエラーの詳細リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクト。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08ad43b717a5e08229054bc10aa81a0786f4e344
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142582"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="3890c-103">devicemanagementトラブルシューティングエラーの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3890c-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="3890c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3890c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3890c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3890c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3890c-106">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="3890c-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="3890c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3890c-107">Properties</span></span>
|<span data-ttu-id="3890c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3890c-108">Property</span></span>|<span data-ttu-id="3890c-109">型</span><span class="sxs-lookup"><span data-stu-id="3890c-109">Type</span></span>|<span data-ttu-id="3890c-110">説明</span><span class="sxs-lookup"><span data-stu-id="3890c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3890c-111">context</span><span class="sxs-lookup"><span data-stu-id="3890c-111">context</span></span>|<span data-ttu-id="3890c-112">String</span><span class="sxs-lookup"><span data-stu-id="3890c-112">String</span></span>|<span data-ttu-id="3890c-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3890c-113">Not yet documented</span></span>|
|<span data-ttu-id="3890c-114">failure</span><span class="sxs-lookup"><span data-stu-id="3890c-114">failure</span></span>|<span data-ttu-id="3890c-115">String</span><span class="sxs-lookup"><span data-stu-id="3890c-115">String</span></span>|<span data-ttu-id="3890c-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3890c-116">Not yet documented</span></span>|
|<span data-ttu-id="3890c-117">failuredetails</span><span class="sxs-lookup"><span data-stu-id="3890c-117">failureDetails</span></span>|<span data-ttu-id="3890c-118">String</span><span class="sxs-lookup"><span data-stu-id="3890c-118">String</span></span>|<span data-ttu-id="3890c-119">問題の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="3890c-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="3890c-120">修復</span><span class="sxs-lookup"><span data-stu-id="3890c-120">remediation</span></span>|<span data-ttu-id="3890c-121">String</span><span class="sxs-lookup"><span data-stu-id="3890c-121">String</span></span>|<span data-ttu-id="3890c-122">この問題を修復する方法の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="3890c-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="3890c-123">resources</span><span class="sxs-lookup"><span data-stu-id="3890c-123">resources</span></span>|<span data-ttu-id="3890c-124">[devicemanagementのトラブルシューティング errorresource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3890c-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="3890c-125">このエラーについての有用なドキュメントへのリンクを示します。</span><span class="sxs-lookup"><span data-stu-id="3890c-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3890c-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3890c-126">Relationships</span></span>
<span data-ttu-id="3890c-127">なし</span><span class="sxs-lookup"><span data-stu-id="3890c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3890c-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3890c-128">JSON Representation</span></span>
<span data-ttu-id="3890c-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3890c-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




