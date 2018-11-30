---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
ms.openlocfilehash: 8a462b49231323288d66a660c769ce7359cb5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022633"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="7d922-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d922-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="7d922-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d922-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d922-105">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="7d922-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="7d922-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d922-106">Properties</span></span>
|<span data-ttu-id="7d922-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d922-107">Property</span></span>|<span data-ttu-id="7d922-108">型</span><span class="sxs-lookup"><span data-stu-id="7d922-108">Type</span></span>|<span data-ttu-id="7d922-109">説明</span><span class="sxs-lookup"><span data-stu-id="7d922-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d922-110">validationName</span><span class="sxs-lookup"><span data-stu-id="7d922-110">validationName</span></span>|<span data-ttu-id="7d922-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d922-111">String</span></span>|<span data-ttu-id="7d922-112">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="7d922-112">The validation friendly name</span></span>|
|<span data-ttu-id="7d922-113">state</span><span class="sxs-lookup"><span data-stu-id="7d922-113">state</span></span>|<span data-ttu-id="7d922-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d922-114">String</span></span>|<span data-ttu-id="7d922-115">操作の状態</span><span class="sxs-lookup"><span data-stu-id="7d922-115">The state of the operation</span></span>|
|<span data-ttu-id="7d922-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="7d922-116">mitigationInstruction</span></span>|<span data-ttu-id="7d922-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d922-117">String</span></span>|<span data-ttu-id="7d922-118">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="7d922-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d922-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d922-119">Relationships</span></span>
<span data-ttu-id="7d922-120">なし</span><span class="sxs-lookup"><span data-stu-id="7d922-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d922-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d922-121">JSON Representation</span></span>
<span data-ttu-id="7d922-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d922-122">Here is a JSON representation of the resource.</span></span>
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



