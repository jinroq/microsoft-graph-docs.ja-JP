---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b64c1fb0ef49c2d7c47c88137bcca8ef89f6ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343919"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="65298-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65298-103">resourceAction resource type</span></span>

> <span data-ttu-id="65298-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65298-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65298-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="65298-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="65298-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65298-106">Properties</span></span>
|<span data-ttu-id="65298-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65298-107">Property</span></span>|<span data-ttu-id="65298-108">種類</span><span class="sxs-lookup"><span data-stu-id="65298-108">Type</span></span>|<span data-ttu-id="65298-109">説明</span><span class="sxs-lookup"><span data-stu-id="65298-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65298-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="65298-110">allowedResourceActions</span></span>|<span data-ttu-id="65298-111">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="65298-111">String collection</span></span>|<span data-ttu-id="65298-112">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="65298-112">Allowed Actions</span></span>|
|<span data-ttu-id="65298-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="65298-113">notAllowedResourceActions</span></span>|<span data-ttu-id="65298-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="65298-114">String collection</span></span>|<span data-ttu-id="65298-115">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="65298-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="65298-116">関係</span><span class="sxs-lookup"><span data-stu-id="65298-116">Relationships</span></span>
<span data-ttu-id="65298-117">なし</span><span class="sxs-lookup"><span data-stu-id="65298-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65298-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65298-118">JSON Representation</span></span>
<span data-ttu-id="65298-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65298-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



