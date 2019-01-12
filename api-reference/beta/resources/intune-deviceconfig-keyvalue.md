---
title: keyValue リソースの種類
description: キー値の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5027388b455a41bc5895009a4ce79ca195ab8340
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957880"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="6ad84-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ad84-103">keyValue resource type</span></span>

> <span data-ttu-id="6ad84-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ad84-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ad84-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ad84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ad84-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ad84-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ad84-107">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="6ad84-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="6ad84-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ad84-108">Properties</span></span>
|<span data-ttu-id="6ad84-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ad84-109">Property</span></span>|<span data-ttu-id="6ad84-110">種類</span><span class="sxs-lookup"><span data-stu-id="6ad84-110">Type</span></span>|<span data-ttu-id="6ad84-111">説明</span><span class="sxs-lookup"><span data-stu-id="6ad84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ad84-112">Key</span><span class="sxs-lookup"><span data-stu-id="6ad84-112">key</span></span>|<span data-ttu-id="6ad84-113">String</span><span class="sxs-lookup"><span data-stu-id="6ad84-113">String</span></span>|<span data-ttu-id="6ad84-114">キー。</span><span class="sxs-lookup"><span data-stu-id="6ad84-114">Key.</span></span>|
|<span data-ttu-id="6ad84-115">value</span><span class="sxs-lookup"><span data-stu-id="6ad84-115">value</span></span>|<span data-ttu-id="6ad84-116">文字列</span><span class="sxs-lookup"><span data-stu-id="6ad84-116">String</span></span>|<span data-ttu-id="6ad84-117">値。</span><span class="sxs-lookup"><span data-stu-id="6ad84-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ad84-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ad84-118">Relationships</span></span>
<span data-ttu-id="6ad84-119">なし</span><span class="sxs-lookup"><span data-stu-id="6ad84-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ad84-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ad84-120">JSON Representation</span></span>
<span data-ttu-id="6ad84-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ad84-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





