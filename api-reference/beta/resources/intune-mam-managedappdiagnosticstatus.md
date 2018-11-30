---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
ms.openlocfilehash: 44284b54692e4a123b1837bbfb0f5f04a2b01a2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073942"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="14190-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14190-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="14190-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14190-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14190-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14190-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14190-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="14190-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14190-107">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="14190-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="14190-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14190-108">Properties</span></span>
|<span data-ttu-id="14190-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14190-109">Property</span></span>|<span data-ttu-id="14190-110">型</span><span class="sxs-lookup"><span data-stu-id="14190-110">Type</span></span>|<span data-ttu-id="14190-111">説明</span><span class="sxs-lookup"><span data-stu-id="14190-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14190-112">validationName</span><span class="sxs-lookup"><span data-stu-id="14190-112">validationName</span></span>|<span data-ttu-id="14190-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="14190-113">String</span></span>|<span data-ttu-id="14190-114">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="14190-114">The validation friendly name</span></span>|
|<span data-ttu-id="14190-115">state</span><span class="sxs-lookup"><span data-stu-id="14190-115">state</span></span>|<span data-ttu-id="14190-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="14190-116">String</span></span>|<span data-ttu-id="14190-117">操作の状態</span><span class="sxs-lookup"><span data-stu-id="14190-117">The state of the operation</span></span>|
|<span data-ttu-id="14190-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="14190-118">mitigationInstruction</span></span>|<span data-ttu-id="14190-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="14190-119">String</span></span>|<span data-ttu-id="14190-120">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="14190-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="14190-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14190-121">Relationships</span></span>
<span data-ttu-id="14190-122">なし</span><span class="sxs-lookup"><span data-stu-id="14190-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14190-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14190-123">JSON Representation</span></span>
<span data-ttu-id="14190-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14190-124">Here is a JSON representation of the resource.</span></span>
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





