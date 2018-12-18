---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
ms.openlocfilehash: fa1fc438ef97357ebd5f13443077384bc98e24f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314043"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="a85ae-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a85ae-103">omaSetting resource type</span></span>

> <span data-ttu-id="a85ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a85ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a85ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a85ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a85ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a85ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a85ae-107">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="a85ae-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="a85ae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a85ae-108">Properties</span></span>
|<span data-ttu-id="a85ae-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a85ae-109">Property</span></span>|<span data-ttu-id="a85ae-110">種類</span><span class="sxs-lookup"><span data-stu-id="a85ae-110">Type</span></span>|<span data-ttu-id="a85ae-111">説明</span><span class="sxs-lookup"><span data-stu-id="a85ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a85ae-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a85ae-112">displayName</span></span>|<span data-ttu-id="a85ae-113">文字列</span><span class="sxs-lookup"><span data-stu-id="a85ae-113">String</span></span>|<span data-ttu-id="a85ae-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="a85ae-114">Display Name.</span></span>|
|<span data-ttu-id="a85ae-115">説明</span><span class="sxs-lookup"><span data-stu-id="a85ae-115">description</span></span>|<span data-ttu-id="a85ae-116">String</span><span class="sxs-lookup"><span data-stu-id="a85ae-116">String</span></span>|<span data-ttu-id="a85ae-117">説明。</span><span class="sxs-lookup"><span data-stu-id="a85ae-117">Description.</span></span>|
|<span data-ttu-id="a85ae-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="a85ae-118">omaUri</span></span>|<span data-ttu-id="a85ae-119">文字列</span><span class="sxs-lookup"><span data-stu-id="a85ae-119">String</span></span>|<span data-ttu-id="a85ae-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="a85ae-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a85ae-121">関係</span><span class="sxs-lookup"><span data-stu-id="a85ae-121">Relationships</span></span>
<span data-ttu-id="a85ae-122">なし</span><span class="sxs-lookup"><span data-stu-id="a85ae-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a85ae-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a85ae-123">JSON Representation</span></span>
<span data-ttu-id="a85ae-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a85ae-124">Here is a JSON representation of the resource.</span></span>
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





