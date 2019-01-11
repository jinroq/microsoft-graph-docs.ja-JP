---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9abc7db7b6d2ad16aa13886905c348e6c8f01b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826475"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="bab94-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bab94-103">omaSetting resource type</span></span>

> <span data-ttu-id="bab94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bab94-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bab94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bab94-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bab94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bab94-107">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="bab94-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="bab94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bab94-108">Properties</span></span>
|<span data-ttu-id="bab94-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bab94-109">Property</span></span>|<span data-ttu-id="bab94-110">種類</span><span class="sxs-lookup"><span data-stu-id="bab94-110">Type</span></span>|<span data-ttu-id="bab94-111">説明</span><span class="sxs-lookup"><span data-stu-id="bab94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bab94-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bab94-112">displayName</span></span>|<span data-ttu-id="bab94-113">文字列</span><span class="sxs-lookup"><span data-stu-id="bab94-113">String</span></span>|<span data-ttu-id="bab94-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="bab94-114">Display Name.</span></span>|
|<span data-ttu-id="bab94-115">説明</span><span class="sxs-lookup"><span data-stu-id="bab94-115">description</span></span>|<span data-ttu-id="bab94-116">String</span><span class="sxs-lookup"><span data-stu-id="bab94-116">String</span></span>|<span data-ttu-id="bab94-117">説明。</span><span class="sxs-lookup"><span data-stu-id="bab94-117">Description.</span></span>|
|<span data-ttu-id="bab94-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="bab94-118">omaUri</span></span>|<span data-ttu-id="bab94-119">文字列</span><span class="sxs-lookup"><span data-stu-id="bab94-119">String</span></span>|<span data-ttu-id="bab94-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="bab94-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bab94-121">関係</span><span class="sxs-lookup"><span data-stu-id="bab94-121">Relationships</span></span>
<span data-ttu-id="bab94-122">なし</span><span class="sxs-lookup"><span data-stu-id="bab94-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bab94-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bab94-123">JSON Representation</span></span>
<span data-ttu-id="bab94-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bab94-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





