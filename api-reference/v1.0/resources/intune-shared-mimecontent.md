---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 53776793fdd057ef057118decf2d72bb0b61a042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307064"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="3a543-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a543-103">mimeContent resource type</span></span>

> <span data-ttu-id="3a543-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a543-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a543-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3a543-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="3a543-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a543-106">Properties</span></span>
|<span data-ttu-id="3a543-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a543-107">Property</span></span>|<span data-ttu-id="3a543-108">種類</span><span class="sxs-lookup"><span data-stu-id="3a543-108">Type</span></span>|<span data-ttu-id="3a543-109">説明</span><span class="sxs-lookup"><span data-stu-id="3a543-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a543-110">type</span><span class="sxs-lookup"><span data-stu-id="3a543-110">type</span></span>|<span data-ttu-id="3a543-111">String</span><span class="sxs-lookup"><span data-stu-id="3a543-111">String</span></span>|<span data-ttu-id="3a543-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="3a543-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="3a543-113">value</span><span class="sxs-lookup"><span data-stu-id="3a543-113">value</span></span>|<span data-ttu-id="3a543-114">バイナリ</span><span class="sxs-lookup"><span data-stu-id="3a543-114">Binary</span></span>|<span data-ttu-id="3a543-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="3a543-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a543-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a543-116">Relationships</span></span>
<span data-ttu-id="3a543-117">なし</span><span class="sxs-lookup"><span data-stu-id="3a543-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a543-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a543-118">JSON Representation</span></span>
<span data-ttu-id="3a543-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a543-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



