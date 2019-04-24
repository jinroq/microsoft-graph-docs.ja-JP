---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 588338589d90ad54db43810d5fd45541cea483eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459124"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="6be92-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6be92-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="6be92-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6be92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be92-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6be92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be92-106">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="6be92-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="6be92-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be92-107">Properties</span></span>
|<span data-ttu-id="6be92-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be92-108">Property</span></span>|<span data-ttu-id="6be92-109">型</span><span class="sxs-lookup"><span data-stu-id="6be92-109">Type</span></span>|<span data-ttu-id="6be92-110">説明</span><span class="sxs-lookup"><span data-stu-id="6be92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be92-111">validationName</span><span class="sxs-lookup"><span data-stu-id="6be92-111">validationName</span></span>|<span data-ttu-id="6be92-112">String</span><span class="sxs-lookup"><span data-stu-id="6be92-112">String</span></span>|<span data-ttu-id="6be92-113">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="6be92-113">The validation friendly name</span></span>|
|<span data-ttu-id="6be92-114">state</span><span class="sxs-lookup"><span data-stu-id="6be92-114">state</span></span>|<span data-ttu-id="6be92-115">String</span><span class="sxs-lookup"><span data-stu-id="6be92-115">String</span></span>|<span data-ttu-id="6be92-116">操作の状態</span><span class="sxs-lookup"><span data-stu-id="6be92-116">The state of the operation</span></span>|
|<span data-ttu-id="6be92-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="6be92-117">mitigationInstruction</span></span>|<span data-ttu-id="6be92-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6be92-118">String</span></span>|<span data-ttu-id="6be92-119">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="6be92-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="6be92-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6be92-120">Relationships</span></span>
<span data-ttu-id="6be92-121">なし</span><span class="sxs-lookup"><span data-stu-id="6be92-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6be92-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6be92-122">JSON Representation</span></span>
<span data-ttu-id="6be92-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6be92-123">Here is a JSON representation of the resource.</span></span>
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





