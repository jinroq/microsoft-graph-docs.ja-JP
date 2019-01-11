---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 98bd1353156c99861749bdb7eac2e686cf96532e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869791"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="25a49-103">managedAppDiagnosticStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25a49-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="25a49-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25a49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25a49-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25a49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25a49-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25a49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25a49-107">診断状態を表します。</span><span class="sxs-lookup"><span data-stu-id="25a49-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="25a49-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25a49-108">Properties</span></span>
|<span data-ttu-id="25a49-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25a49-109">Property</span></span>|<span data-ttu-id="25a49-110">種類</span><span class="sxs-lookup"><span data-stu-id="25a49-110">Type</span></span>|<span data-ttu-id="25a49-111">説明</span><span class="sxs-lookup"><span data-stu-id="25a49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25a49-112">validationName</span><span class="sxs-lookup"><span data-stu-id="25a49-112">validationName</span></span>|<span data-ttu-id="25a49-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="25a49-113">String</span></span>|<span data-ttu-id="25a49-114">検証のフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="25a49-114">The validation friendly name</span></span>|
|<span data-ttu-id="25a49-115">state</span><span class="sxs-lookup"><span data-stu-id="25a49-115">state</span></span>|<span data-ttu-id="25a49-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="25a49-116">String</span></span>|<span data-ttu-id="25a49-117">操作の状態</span><span class="sxs-lookup"><span data-stu-id="25a49-117">The state of the operation</span></span>|
|<span data-ttu-id="25a49-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="25a49-118">mitigationInstruction</span></span>|<span data-ttu-id="25a49-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="25a49-119">String</span></span>|<span data-ttu-id="25a49-120">検証の失敗を減らすための方法に関する説明</span><span class="sxs-lookup"><span data-stu-id="25a49-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="25a49-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25a49-121">Relationships</span></span>
<span data-ttu-id="25a49-122">なし</span><span class="sxs-lookup"><span data-stu-id="25a49-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25a49-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25a49-123">JSON Representation</span></span>
<span data-ttu-id="25a49-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25a49-124">Here is a JSON representation of the resource.</span></span>
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





