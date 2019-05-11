---
title: encryptionReportPolicyDetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddca213c3de3c004a19ebc3877aed1542604933e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946645"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="7be0c-103">encryptionReportPolicyDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7be0c-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="7be0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7be0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7be0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7be0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7be0c-106">暗号化レポートのポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="7be0c-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="7be0c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be0c-107">Properties</span></span>
|<span data-ttu-id="7be0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be0c-108">Property</span></span>|<span data-ttu-id="7be0c-109">型</span><span class="sxs-lookup"><span data-stu-id="7be0c-109">Type</span></span>|<span data-ttu-id="7be0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="7be0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be0c-111">policyId</span><span class="sxs-lookup"><span data-stu-id="7be0c-111">policyId</span></span>|<span data-ttu-id="7be0c-112">String</span><span class="sxs-lookup"><span data-stu-id="7be0c-112">String</span></span>|<span data-ttu-id="7be0c-113">暗号化レポートのポリシー Id</span><span class="sxs-lookup"><span data-stu-id="7be0c-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="7be0c-114">policyName</span><span class="sxs-lookup"><span data-stu-id="7be0c-114">policyName</span></span>|<span data-ttu-id="7be0c-115">String</span><span class="sxs-lookup"><span data-stu-id="7be0c-115">String</span></span>|<span data-ttu-id="7be0c-116">暗号化レポートのポリシー名</span><span class="sxs-lookup"><span data-stu-id="7be0c-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be0c-117">関係</span><span class="sxs-lookup"><span data-stu-id="7be0c-117">Relationships</span></span>
<span data-ttu-id="7be0c-118">なし</span><span class="sxs-lookup"><span data-stu-id="7be0c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be0c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7be0c-119">JSON Representation</span></span>
<span data-ttu-id="7be0c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7be0c-120">Here is a JSON representation of the resource.</span></span>
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




