---
title: encryptionReportPolicyDetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1484e1ed55abb14daccb61e024dc94eb415e031
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004373"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="632ed-103">encryptionReportPolicyDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="632ed-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="632ed-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="632ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="632ed-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="632ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="632ed-106">暗号化レポートのポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="632ed-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="632ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="632ed-107">Properties</span></span>
|<span data-ttu-id="632ed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="632ed-108">Property</span></span>|<span data-ttu-id="632ed-109">型</span><span class="sxs-lookup"><span data-stu-id="632ed-109">Type</span></span>|<span data-ttu-id="632ed-110">説明</span><span class="sxs-lookup"><span data-stu-id="632ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="632ed-111">policyId</span><span class="sxs-lookup"><span data-stu-id="632ed-111">policyId</span></span>|<span data-ttu-id="632ed-112">String</span><span class="sxs-lookup"><span data-stu-id="632ed-112">String</span></span>|<span data-ttu-id="632ed-113">暗号化レポートのポリシー Id</span><span class="sxs-lookup"><span data-stu-id="632ed-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="632ed-114">policyName</span><span class="sxs-lookup"><span data-stu-id="632ed-114">policyName</span></span>|<span data-ttu-id="632ed-115">String</span><span class="sxs-lookup"><span data-stu-id="632ed-115">String</span></span>|<span data-ttu-id="632ed-116">暗号化レポートのポリシー名</span><span class="sxs-lookup"><span data-stu-id="632ed-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="632ed-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="632ed-117">Relationships</span></span>
<span data-ttu-id="632ed-118">なし</span><span class="sxs-lookup"><span data-stu-id="632ed-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="632ed-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="632ed-119">JSON Representation</span></span>
<span data-ttu-id="632ed-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="632ed-120">Here is a JSON representation of the resource.</span></span>
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





