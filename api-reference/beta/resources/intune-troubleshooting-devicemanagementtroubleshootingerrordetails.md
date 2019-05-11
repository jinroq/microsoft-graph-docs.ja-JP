---
title: Devicemanagementトラブルシューティングエラーの詳細リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクト。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50c749e6c6c6ddd59705bbea34f0bbd2488f9a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939785"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="1d2d3-103">Devicemanagementトラブルシューティングエラーの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d2d3-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="1d2d3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d2d3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d2d3-106">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="1d2d3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d2d3-107">Properties</span></span>
|<span data-ttu-id="1d2d3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d2d3-108">Property</span></span>|<span data-ttu-id="1d2d3-109">型</span><span class="sxs-lookup"><span data-stu-id="1d2d3-109">Type</span></span>|<span data-ttu-id="1d2d3-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d2d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d2d3-111">context</span><span class="sxs-lookup"><span data-stu-id="1d2d3-111">context</span></span>|<span data-ttu-id="1d2d3-112">String</span><span class="sxs-lookup"><span data-stu-id="1d2d3-112">String</span></span>|<span data-ttu-id="1d2d3-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d2d3-113">Not yet documented</span></span>|
|<span data-ttu-id="1d2d3-114">エラー</span><span class="sxs-lookup"><span data-stu-id="1d2d3-114">failure</span></span>|<span data-ttu-id="1d2d3-115">String</span><span class="sxs-lookup"><span data-stu-id="1d2d3-115">String</span></span>|<span data-ttu-id="1d2d3-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d2d3-116">Not yet documented</span></span>|
|<span data-ttu-id="1d2d3-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="1d2d3-117">failureDetails</span></span>|<span data-ttu-id="1d2d3-118">String</span><span class="sxs-lookup"><span data-stu-id="1d2d3-118">String</span></span>|<span data-ttu-id="1d2d3-119">問題の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="1d2d3-120">修復</span><span class="sxs-lookup"><span data-stu-id="1d2d3-120">remediation</span></span>|<span data-ttu-id="1d2d3-121">String</span><span class="sxs-lookup"><span data-stu-id="1d2d3-121">String</span></span>|<span data-ttu-id="1d2d3-122">この問題を修復する方法の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="1d2d3-123">リソース</span><span class="sxs-lookup"><span data-stu-id="1d2d3-123">resources</span></span>|<span data-ttu-id="1d2d3-124">[Devicemanagementのトラブルシューティング Errorresource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d2d3-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="1d2d3-125">このエラーについての有用なドキュメントへのリンクを示します。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d2d3-126">関係</span><span class="sxs-lookup"><span data-stu-id="1d2d3-126">Relationships</span></span>
<span data-ttu-id="1d2d3-127">なし</span><span class="sxs-lookup"><span data-stu-id="1d2d3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d2d3-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d2d3-128">JSON Representation</span></span>
<span data-ttu-id="1d2d3-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d2d3-129">Here is a JSON representation of the resource.</span></span>
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




