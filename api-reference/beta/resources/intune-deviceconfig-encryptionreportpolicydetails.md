---
title: encryptionreportpolicydetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556299"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="86a1b-103">encryptionreportpolicydetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86a1b-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="86a1b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86a1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a1b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86a1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a1b-106">暗号化レポートのポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="86a1b-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="86a1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86a1b-107">Properties</span></span>
|<span data-ttu-id="86a1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86a1b-108">Property</span></span>|<span data-ttu-id="86a1b-109">型</span><span class="sxs-lookup"><span data-stu-id="86a1b-109">Type</span></span>|<span data-ttu-id="86a1b-110">説明</span><span class="sxs-lookup"><span data-stu-id="86a1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a1b-111">policyid</span><span class="sxs-lookup"><span data-stu-id="86a1b-111">policyId</span></span>|<span data-ttu-id="86a1b-112">String</span><span class="sxs-lookup"><span data-stu-id="86a1b-112">String</span></span>|<span data-ttu-id="86a1b-113">暗号化レポートのポリシー Id</span><span class="sxs-lookup"><span data-stu-id="86a1b-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="86a1b-114">policyName</span><span class="sxs-lookup"><span data-stu-id="86a1b-114">policyName</span></span>|<span data-ttu-id="86a1b-115">String</span><span class="sxs-lookup"><span data-stu-id="86a1b-115">String</span></span>|<span data-ttu-id="86a1b-116">暗号化レポートのポリシー名</span><span class="sxs-lookup"><span data-stu-id="86a1b-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="86a1b-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86a1b-117">Relationships</span></span>
<span data-ttu-id="86a1b-118">なし</span><span class="sxs-lookup"><span data-stu-id="86a1b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86a1b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86a1b-119">JSON Representation</span></span>
<span data-ttu-id="86a1b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86a1b-120">Here is a JSON representation of the resource.</span></span>
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





