---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a5204a4704eefc2d4e7c8e0d5b3b709e1750667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937482"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="bd278-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd278-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="bd278-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd278-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd278-105">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="bd278-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="bd278-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd278-106">Properties</span></span>
|<span data-ttu-id="bd278-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd278-107">Property</span></span>|<span data-ttu-id="bd278-108">種類</span><span class="sxs-lookup"><span data-stu-id="bd278-108">Type</span></span>|<span data-ttu-id="bd278-109">説明</span><span class="sxs-lookup"><span data-stu-id="bd278-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd278-110">validationName</span><span class="sxs-lookup"><span data-stu-id="bd278-110">validationName</span></span>|<span data-ttu-id="bd278-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bd278-111">String</span></span>|<span data-ttu-id="bd278-112">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="bd278-112">The validation friendly name</span></span>|
|<span data-ttu-id="bd278-113">state</span><span class="sxs-lookup"><span data-stu-id="bd278-113">state</span></span>|<span data-ttu-id="bd278-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bd278-114">String</span></span>|<span data-ttu-id="bd278-115">操作の状態</span><span class="sxs-lookup"><span data-stu-id="bd278-115">The state of the operation</span></span>|
|<span data-ttu-id="bd278-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="bd278-116">mitigationInstruction</span></span>|<span data-ttu-id="bd278-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bd278-117">String</span></span>|<span data-ttu-id="bd278-118">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="bd278-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd278-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd278-119">Relationships</span></span>
<span data-ttu-id="bd278-120">なし</span><span class="sxs-lookup"><span data-stu-id="bd278-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd278-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd278-121">JSON Representation</span></span>
<span data-ttu-id="bd278-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd278-122">Here is a JSON representation of the resource.</span></span>
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



