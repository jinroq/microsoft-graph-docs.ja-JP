---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261552"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="be2ba-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be2ba-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="be2ba-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be2ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be2ba-105">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="be2ba-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="be2ba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be2ba-106">Properties</span></span>
|<span data-ttu-id="be2ba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be2ba-107">Property</span></span>|<span data-ttu-id="be2ba-108">型</span><span class="sxs-lookup"><span data-stu-id="be2ba-108">Type</span></span>|<span data-ttu-id="be2ba-109">説明</span><span class="sxs-lookup"><span data-stu-id="be2ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be2ba-110">validationName</span><span class="sxs-lookup"><span data-stu-id="be2ba-110">validationName</span></span>|<span data-ttu-id="be2ba-111">String</span><span class="sxs-lookup"><span data-stu-id="be2ba-111">String</span></span>|<span data-ttu-id="be2ba-112">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="be2ba-112">The validation friendly name</span></span>|
|<span data-ttu-id="be2ba-113">state</span><span class="sxs-lookup"><span data-stu-id="be2ba-113">state</span></span>|<span data-ttu-id="be2ba-114">String</span><span class="sxs-lookup"><span data-stu-id="be2ba-114">String</span></span>|<span data-ttu-id="be2ba-115">操作の状態</span><span class="sxs-lookup"><span data-stu-id="be2ba-115">The state of the operation</span></span>|
|<span data-ttu-id="be2ba-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="be2ba-116">mitigationInstruction</span></span>|<span data-ttu-id="be2ba-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be2ba-117">String</span></span>|<span data-ttu-id="be2ba-118">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="be2ba-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="be2ba-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be2ba-119">Relationships</span></span>
<span data-ttu-id="be2ba-120">なし</span><span class="sxs-lookup"><span data-stu-id="be2ba-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be2ba-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be2ba-121">JSON Representation</span></span>
<span data-ttu-id="be2ba-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be2ba-122">Here is a JSON representation of the resource.</span></span>
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



