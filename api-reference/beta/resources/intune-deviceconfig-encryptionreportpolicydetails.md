---
title: encryptionreportpolicydetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177918"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="4b1e6-103">encryptionreportpolicydetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b1e6-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="4b1e6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b1e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b1e6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b1e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b1e6-106">暗号化レポートのポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="4b1e6-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="4b1e6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1e6-107">Properties</span></span>
|<span data-ttu-id="4b1e6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1e6-108">Property</span></span>|<span data-ttu-id="4b1e6-109">型</span><span class="sxs-lookup"><span data-stu-id="4b1e6-109">Type</span></span>|<span data-ttu-id="4b1e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="4b1e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b1e6-111">policyid</span><span class="sxs-lookup"><span data-stu-id="4b1e6-111">policyId</span></span>|<span data-ttu-id="4b1e6-112">String</span><span class="sxs-lookup"><span data-stu-id="4b1e6-112">String</span></span>|<span data-ttu-id="4b1e6-113">暗号化レポートのポリシー Id</span><span class="sxs-lookup"><span data-stu-id="4b1e6-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="4b1e6-114">policyName</span><span class="sxs-lookup"><span data-stu-id="4b1e6-114">policyName</span></span>|<span data-ttu-id="4b1e6-115">String</span><span class="sxs-lookup"><span data-stu-id="4b1e6-115">String</span></span>|<span data-ttu-id="4b1e6-116">暗号化レポートのポリシー名</span><span class="sxs-lookup"><span data-stu-id="4b1e6-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1e6-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b1e6-117">Relationships</span></span>
<span data-ttu-id="4b1e6-118">なし</span><span class="sxs-lookup"><span data-stu-id="4b1e6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b1e6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b1e6-119">JSON Representation</span></span>
<span data-ttu-id="4b1e6-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b1e6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




