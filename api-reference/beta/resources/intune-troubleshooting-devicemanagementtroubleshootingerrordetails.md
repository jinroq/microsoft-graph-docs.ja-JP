---
title: deviceManagementTroubleshootingErrorDetails リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクトです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430334"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="1075f-103">deviceManagementTroubleshootingErrorDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1075f-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="1075f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1075f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1075f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1075f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1075f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1075f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1075f-107">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1075f-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="1075f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1075f-108">Properties</span></span>
|<span data-ttu-id="1075f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1075f-109">Property</span></span>|<span data-ttu-id="1075f-110">型</span><span class="sxs-lookup"><span data-stu-id="1075f-110">Type</span></span>|<span data-ttu-id="1075f-111">説明</span><span class="sxs-lookup"><span data-stu-id="1075f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1075f-112">context</span><span class="sxs-lookup"><span data-stu-id="1075f-112">context</span></span>|<span data-ttu-id="1075f-113">String</span><span class="sxs-lookup"><span data-stu-id="1075f-113">String</span></span>|<span data-ttu-id="1075f-114">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1075f-114">Not yet documented</span></span>|
|<span data-ttu-id="1075f-115">failure</span><span class="sxs-lookup"><span data-stu-id="1075f-115">failure</span></span>|<span data-ttu-id="1075f-116">String</span><span class="sxs-lookup"><span data-stu-id="1075f-116">String</span></span>|<span data-ttu-id="1075f-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1075f-117">Not yet documented</span></span>|
|<span data-ttu-id="1075f-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="1075f-118">failureDetails</span></span>|<span data-ttu-id="1075f-119">String</span><span class="sxs-lookup"><span data-stu-id="1075f-119">String</span></span>|<span data-ttu-id="1075f-120">失敗の原因の詳細な説明です。</span><span class="sxs-lookup"><span data-stu-id="1075f-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="1075f-121">改善計画</span><span class="sxs-lookup"><span data-stu-id="1075f-121">remediation</span></span>|<span data-ttu-id="1075f-122">String</span><span class="sxs-lookup"><span data-stu-id="1075f-122">String</span></span>|<span data-ttu-id="1075f-123">この問題を修正する方法についての詳細な説明です。</span><span class="sxs-lookup"><span data-stu-id="1075f-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="1075f-124">resources</span><span class="sxs-lookup"><span data-stu-id="1075f-124">resources</span></span>|<span data-ttu-id="1075f-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1075f-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="1075f-126">この障害に関する役に立つドキュメントにリンクします。</span><span class="sxs-lookup"><span data-stu-id="1075f-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1075f-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1075f-127">Relationships</span></span>
<span data-ttu-id="1075f-128">なし</span><span class="sxs-lookup"><span data-stu-id="1075f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1075f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1075f-129">JSON Representation</span></span>
<span data-ttu-id="1075f-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1075f-130">Here is a JSON representation of the resource.</span></span>
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




