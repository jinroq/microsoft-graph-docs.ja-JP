---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
ms.openlocfilehash: 7f0cd0d5b11c4d902f51dd422add2373e8e8df9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340685"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="8cd1d-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cd1d-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="8cd1d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8cd1d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cd1d-105">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="8cd1d-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="8cd1d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cd1d-106">Properties</span></span>
|<span data-ttu-id="8cd1d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cd1d-107">Property</span></span>|<span data-ttu-id="8cd1d-108">種類</span><span class="sxs-lookup"><span data-stu-id="8cd1d-108">Type</span></span>|<span data-ttu-id="8cd1d-109">説明</span><span class="sxs-lookup"><span data-stu-id="8cd1d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cd1d-110">validationName</span><span class="sxs-lookup"><span data-stu-id="8cd1d-110">validationName</span></span>|<span data-ttu-id="8cd1d-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8cd1d-111">String</span></span>|<span data-ttu-id="8cd1d-112">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="8cd1d-112">The validation friendly name</span></span>|
|<span data-ttu-id="8cd1d-113">state</span><span class="sxs-lookup"><span data-stu-id="8cd1d-113">state</span></span>|<span data-ttu-id="8cd1d-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8cd1d-114">String</span></span>|<span data-ttu-id="8cd1d-115">操作の状態</span><span class="sxs-lookup"><span data-stu-id="8cd1d-115">The state of the operation</span></span>|
|<span data-ttu-id="8cd1d-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="8cd1d-116">mitigationInstruction</span></span>|<span data-ttu-id="8cd1d-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8cd1d-117">String</span></span>|<span data-ttu-id="8cd1d-118">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="8cd1d-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cd1d-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cd1d-119">Relationships</span></span>
<span data-ttu-id="8cd1d-120">なし</span><span class="sxs-lookup"><span data-stu-id="8cd1d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8cd1d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cd1d-121">JSON Representation</span></span>
<span data-ttu-id="8cd1d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cd1d-122">Here is a JSON representation of the resource.</span></span>
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



