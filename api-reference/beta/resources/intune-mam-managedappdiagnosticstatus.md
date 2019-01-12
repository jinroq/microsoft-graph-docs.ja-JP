---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 210edaf8eb039db928d612337aa7c8e0642c9ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987189"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3d84a-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d84a-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3d84a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d84a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d84a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d84a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d84a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d84a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d84a-107">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3d84a-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="3d84a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d84a-108">Properties</span></span>
|<span data-ttu-id="3d84a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d84a-109">Property</span></span>|<span data-ttu-id="3d84a-110">種類</span><span class="sxs-lookup"><span data-stu-id="3d84a-110">Type</span></span>|<span data-ttu-id="3d84a-111">説明</span><span class="sxs-lookup"><span data-stu-id="3d84a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d84a-112">validationName</span><span class="sxs-lookup"><span data-stu-id="3d84a-112">validationName</span></span>|<span data-ttu-id="3d84a-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3d84a-113">String</span></span>|<span data-ttu-id="3d84a-114">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="3d84a-114">The validation friendly name</span></span>|
|<span data-ttu-id="3d84a-115">state</span><span class="sxs-lookup"><span data-stu-id="3d84a-115">state</span></span>|<span data-ttu-id="3d84a-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3d84a-116">String</span></span>|<span data-ttu-id="3d84a-117">操作の状態</span><span class="sxs-lookup"><span data-stu-id="3d84a-117">The state of the operation</span></span>|
|<span data-ttu-id="3d84a-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3d84a-118">mitigationInstruction</span></span>|<span data-ttu-id="3d84a-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3d84a-119">String</span></span>|<span data-ttu-id="3d84a-120">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="3d84a-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d84a-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d84a-121">Relationships</span></span>
<span data-ttu-id="3d84a-122">なし</span><span class="sxs-lookup"><span data-stu-id="3d84a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d84a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d84a-123">JSON Representation</span></span>
<span data-ttu-id="3d84a-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d84a-124">Here is a JSON representation of the resource.</span></span>
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





