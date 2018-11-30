---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
ms.openlocfilehash: 7f25a1c16b86a45886cd763c1a8a3aa6142c47e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021814"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="fbdcd-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbdcd-103">mimeContent resource type</span></span>

> <span data-ttu-id="fbdcd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbdcd-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="fbdcd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbdcd-106">Properties</span></span>
|<span data-ttu-id="fbdcd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbdcd-107">Property</span></span>|<span data-ttu-id="fbdcd-108">型</span><span class="sxs-lookup"><span data-stu-id="fbdcd-108">Type</span></span>|<span data-ttu-id="fbdcd-109">説明</span><span class="sxs-lookup"><span data-stu-id="fbdcd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbdcd-110">type</span><span class="sxs-lookup"><span data-stu-id="fbdcd-110">type</span></span>|<span data-ttu-id="fbdcd-111">String</span><span class="sxs-lookup"><span data-stu-id="fbdcd-111">String</span></span>|<span data-ttu-id="fbdcd-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="fbdcd-113">value</span><span class="sxs-lookup"><span data-stu-id="fbdcd-113">value</span></span>|<span data-ttu-id="fbdcd-114">バイナリ</span><span class="sxs-lookup"><span data-stu-id="fbdcd-114">Binary</span></span>|<span data-ttu-id="fbdcd-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbdcd-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbdcd-116">Relationships</span></span>
<span data-ttu-id="fbdcd-117">なし</span><span class="sxs-lookup"><span data-stu-id="fbdcd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbdcd-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbdcd-118">JSON Representation</span></span>
<span data-ttu-id="fbdcd-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-119">Here is a JSON representation of the resource.</span></span>
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



