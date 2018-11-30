---
title: omaSetting リソースの種類
description: OMA 設定の定義。
ms.openlocfilehash: 7ef8617ca4ce10ebeabf0d7a4655688e58925646
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021596"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="7ed44-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ed44-103">omaSetting resource type</span></span>

> <span data-ttu-id="7ed44-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ed44-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ed44-105">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="7ed44-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="7ed44-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ed44-106">Properties</span></span>
|<span data-ttu-id="7ed44-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ed44-107">Property</span></span>|<span data-ttu-id="7ed44-108">型</span><span class="sxs-lookup"><span data-stu-id="7ed44-108">Type</span></span>|<span data-ttu-id="7ed44-109">説明</span><span class="sxs-lookup"><span data-stu-id="7ed44-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed44-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed44-110">displayName</span></span>|<span data-ttu-id="7ed44-111">文字列</span><span class="sxs-lookup"><span data-stu-id="7ed44-111">String</span></span>|<span data-ttu-id="7ed44-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="7ed44-112">Display Name.</span></span>|
|<span data-ttu-id="7ed44-113">説明</span><span class="sxs-lookup"><span data-stu-id="7ed44-113">description</span></span>|<span data-ttu-id="7ed44-114">String</span><span class="sxs-lookup"><span data-stu-id="7ed44-114">String</span></span>|<span data-ttu-id="7ed44-115">説明。</span><span class="sxs-lookup"><span data-stu-id="7ed44-115">Description.</span></span>|
|<span data-ttu-id="7ed44-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="7ed44-116">omaUri</span></span>|<span data-ttu-id="7ed44-117">文字列</span><span class="sxs-lookup"><span data-stu-id="7ed44-117">String</span></span>|<span data-ttu-id="7ed44-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="7ed44-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ed44-119">関係</span><span class="sxs-lookup"><span data-stu-id="7ed44-119">Relationships</span></span>
<span data-ttu-id="7ed44-120">なし</span><span class="sxs-lookup"><span data-stu-id="7ed44-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ed44-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ed44-121">JSON Representation</span></span>
<span data-ttu-id="7ed44-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7ed44-122">Here is a JSON representation of the resource.</span></span>
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



