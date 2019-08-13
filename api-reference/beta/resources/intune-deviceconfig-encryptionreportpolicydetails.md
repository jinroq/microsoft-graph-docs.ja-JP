---
title: encryptionReportPolicyDetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7271329a7536a6359bbc9662427e65e21ea39d8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325611"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="f1122-103">encryptionReportPolicyDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1122-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="f1122-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1122-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1122-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1122-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1122-106">暗号化レポートのポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="f1122-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="f1122-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1122-107">Properties</span></span>
|<span data-ttu-id="f1122-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1122-108">Property</span></span>|<span data-ttu-id="f1122-109">型</span><span class="sxs-lookup"><span data-stu-id="f1122-109">Type</span></span>|<span data-ttu-id="f1122-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1122-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1122-111">policyId</span><span class="sxs-lookup"><span data-stu-id="f1122-111">policyId</span></span>|<span data-ttu-id="f1122-112">String</span><span class="sxs-lookup"><span data-stu-id="f1122-112">String</span></span>|<span data-ttu-id="f1122-113">暗号化レポートのポリシー Id</span><span class="sxs-lookup"><span data-stu-id="f1122-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="f1122-114">policyName</span><span class="sxs-lookup"><span data-stu-id="f1122-114">policyName</span></span>|<span data-ttu-id="f1122-115">String</span><span class="sxs-lookup"><span data-stu-id="f1122-115">String</span></span>|<span data-ttu-id="f1122-116">暗号化レポートのポリシー名</span><span class="sxs-lookup"><span data-stu-id="f1122-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1122-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1122-117">Relationships</span></span>
<span data-ttu-id="f1122-118">なし</span><span class="sxs-lookup"><span data-stu-id="f1122-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1122-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1122-119">JSON Representation</span></span>
<span data-ttu-id="f1122-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1122-120">Here is a JSON representation of the resource.</span></span>
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



