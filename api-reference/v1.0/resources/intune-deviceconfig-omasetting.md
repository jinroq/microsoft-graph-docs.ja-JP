---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
ms.openlocfilehash: 564912635fbcd5e2846965d3546a3830119db252
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340888"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="1c4c7-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c4c7-103">omaSetting resource type</span></span>

> <span data-ttu-id="1c4c7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c4c7-105">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="1c4c7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c4c7-106">Properties</span></span>
|<span data-ttu-id="1c4c7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c4c7-107">Property</span></span>|<span data-ttu-id="1c4c7-108">種類</span><span class="sxs-lookup"><span data-stu-id="1c4c7-108">Type</span></span>|<span data-ttu-id="1c4c7-109">説明</span><span class="sxs-lookup"><span data-stu-id="1c4c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c4c7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1c4c7-110">displayName</span></span>|<span data-ttu-id="1c4c7-111">文字列</span><span class="sxs-lookup"><span data-stu-id="1c4c7-111">String</span></span>|<span data-ttu-id="1c4c7-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-112">Display Name.</span></span>|
|<span data-ttu-id="1c4c7-113">説明</span><span class="sxs-lookup"><span data-stu-id="1c4c7-113">description</span></span>|<span data-ttu-id="1c4c7-114">String</span><span class="sxs-lookup"><span data-stu-id="1c4c7-114">String</span></span>|<span data-ttu-id="1c4c7-115">説明。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-115">Description.</span></span>|
|<span data-ttu-id="1c4c7-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="1c4c7-116">omaUri</span></span>|<span data-ttu-id="1c4c7-117">文字列</span><span class="sxs-lookup"><span data-stu-id="1c4c7-117">String</span></span>|<span data-ttu-id="1c4c7-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c4c7-119">関係</span><span class="sxs-lookup"><span data-stu-id="1c4c7-119">Relationships</span></span>
<span data-ttu-id="1c4c7-120">なし</span><span class="sxs-lookup"><span data-stu-id="1c4c7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c4c7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c4c7-121">JSON Representation</span></span>
<span data-ttu-id="1c4c7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1c4c7-122">Here is a JSON representation of the resource.</span></span>
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



