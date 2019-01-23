---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 665ca55c67f5facb22eaf976e81737fed3dacf76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407362"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="11cd8-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11cd8-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="11cd8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11cd8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11cd8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11cd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11cd8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11cd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11cd8-107">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="11cd8-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="11cd8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11cd8-108">Properties</span></span>
|<span data-ttu-id="11cd8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11cd8-109">Property</span></span>|<span data-ttu-id="11cd8-110">型</span><span class="sxs-lookup"><span data-stu-id="11cd8-110">Type</span></span>|<span data-ttu-id="11cd8-111">説明</span><span class="sxs-lookup"><span data-stu-id="11cd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11cd8-112">validationName</span><span class="sxs-lookup"><span data-stu-id="11cd8-112">validationName</span></span>|<span data-ttu-id="11cd8-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11cd8-113">String</span></span>|<span data-ttu-id="11cd8-114">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="11cd8-114">The validation friendly name</span></span>|
|<span data-ttu-id="11cd8-115">state</span><span class="sxs-lookup"><span data-stu-id="11cd8-115">state</span></span>|<span data-ttu-id="11cd8-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11cd8-116">String</span></span>|<span data-ttu-id="11cd8-117">操作の状態</span><span class="sxs-lookup"><span data-stu-id="11cd8-117">The state of the operation</span></span>|
|<span data-ttu-id="11cd8-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="11cd8-118">mitigationInstruction</span></span>|<span data-ttu-id="11cd8-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11cd8-119">String</span></span>|<span data-ttu-id="11cd8-120">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="11cd8-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="11cd8-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="11cd8-121">Relationships</span></span>
<span data-ttu-id="11cd8-122">なし</span><span class="sxs-lookup"><span data-stu-id="11cd8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11cd8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11cd8-123">JSON Representation</span></span>
<span data-ttu-id="11cd8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11cd8-124">Here is a JSON representation of the resource.</span></span>
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




