---
title: devicemanagementトラブルシューティングエラーの詳細リソースの種類
description: エラーとその修復に関する詳細情報を含むオブジェクト。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfcbe0688836fa394237f1a25656540e401555f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554066"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="833e0-103">devicemanagementトラブルシューティングエラーの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="833e0-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="833e0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="833e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="833e0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="833e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="833e0-106">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="833e0-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="833e0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="833e0-107">Properties</span></span>
|<span data-ttu-id="833e0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="833e0-108">Property</span></span>|<span data-ttu-id="833e0-109">型</span><span class="sxs-lookup"><span data-stu-id="833e0-109">Type</span></span>|<span data-ttu-id="833e0-110">説明</span><span class="sxs-lookup"><span data-stu-id="833e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="833e0-111">context</span><span class="sxs-lookup"><span data-stu-id="833e0-111">context</span></span>|<span data-ttu-id="833e0-112">String</span><span class="sxs-lookup"><span data-stu-id="833e0-112">String</span></span>|<span data-ttu-id="833e0-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="833e0-113">Not yet documented</span></span>|
|<span data-ttu-id="833e0-114">エラー</span><span class="sxs-lookup"><span data-stu-id="833e0-114">failure</span></span>|<span data-ttu-id="833e0-115">String</span><span class="sxs-lookup"><span data-stu-id="833e0-115">String</span></span>|<span data-ttu-id="833e0-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="833e0-116">Not yet documented</span></span>|
|<span data-ttu-id="833e0-117">failuredetails</span><span class="sxs-lookup"><span data-stu-id="833e0-117">failureDetails</span></span>|<span data-ttu-id="833e0-118">String</span><span class="sxs-lookup"><span data-stu-id="833e0-118">String</span></span>|<span data-ttu-id="833e0-119">問題の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="833e0-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="833e0-120">修復</span><span class="sxs-lookup"><span data-stu-id="833e0-120">remediation</span></span>|<span data-ttu-id="833e0-121">String</span><span class="sxs-lookup"><span data-stu-id="833e0-121">String</span></span>|<span data-ttu-id="833e0-122">この問題を修復する方法の詳細な説明。</span><span class="sxs-lookup"><span data-stu-id="833e0-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="833e0-123">リソース</span><span class="sxs-lookup"><span data-stu-id="833e0-123">resources</span></span>|<span data-ttu-id="833e0-124">[devicemanagementのトラブルシューティング errorresource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="833e0-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="833e0-125">このエラーについての有用なドキュメントへのリンクを示します。</span><span class="sxs-lookup"><span data-stu-id="833e0-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="833e0-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="833e0-126">Relationships</span></span>
<span data-ttu-id="833e0-127">なし</span><span class="sxs-lookup"><span data-stu-id="833e0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="833e0-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="833e0-128">JSON Representation</span></span>
<span data-ttu-id="833e0-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="833e0-129">Here is a JSON representation of the resource.</span></span>
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



