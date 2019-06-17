---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 907f9940b7cbb4a35f69e0792092e14c99aebdae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996296"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="24d4d-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24d4d-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="24d4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24d4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24d4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24d4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24d4d-106">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="24d4d-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="24d4d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24d4d-107">Properties</span></span>
|<span data-ttu-id="24d4d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24d4d-108">Property</span></span>|<span data-ttu-id="24d4d-109">型</span><span class="sxs-lookup"><span data-stu-id="24d4d-109">Type</span></span>|<span data-ttu-id="24d4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="24d4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24d4d-111">validationName</span><span class="sxs-lookup"><span data-stu-id="24d4d-111">validationName</span></span>|<span data-ttu-id="24d4d-112">String</span><span class="sxs-lookup"><span data-stu-id="24d4d-112">String</span></span>|<span data-ttu-id="24d4d-113">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="24d4d-113">The validation friendly name</span></span>|
|<span data-ttu-id="24d4d-114">state</span><span class="sxs-lookup"><span data-stu-id="24d4d-114">state</span></span>|<span data-ttu-id="24d4d-115">String</span><span class="sxs-lookup"><span data-stu-id="24d4d-115">String</span></span>|<span data-ttu-id="24d4d-116">操作の状態</span><span class="sxs-lookup"><span data-stu-id="24d4d-116">The state of the operation</span></span>|
|<span data-ttu-id="24d4d-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="24d4d-117">mitigationInstruction</span></span>|<span data-ttu-id="24d4d-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="24d4d-118">String</span></span>|<span data-ttu-id="24d4d-119">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="24d4d-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="24d4d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24d4d-120">Relationships</span></span>
<span data-ttu-id="24d4d-121">なし</span><span class="sxs-lookup"><span data-stu-id="24d4d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24d4d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24d4d-122">JSON Representation</span></span>
<span data-ttu-id="24d4d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24d4d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```





