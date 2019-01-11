---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0b63289b3d7666eb27de7e6dc4e643dd9fa4772
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857044"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="ebd56-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebd56-103">mimeContent resource type</span></span>

> <span data-ttu-id="ebd56-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebd56-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebd56-105">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ebd56-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="ebd56-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebd56-106">Properties</span></span>
|<span data-ttu-id="ebd56-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebd56-107">Property</span></span>|<span data-ttu-id="ebd56-108">種類</span><span class="sxs-lookup"><span data-stu-id="ebd56-108">Type</span></span>|<span data-ttu-id="ebd56-109">説明</span><span class="sxs-lookup"><span data-stu-id="ebd56-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd56-110">type</span><span class="sxs-lookup"><span data-stu-id="ebd56-110">type</span></span>|<span data-ttu-id="ebd56-111">String</span><span class="sxs-lookup"><span data-stu-id="ebd56-111">String</span></span>|<span data-ttu-id="ebd56-112">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ebd56-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="ebd56-113">value</span><span class="sxs-lookup"><span data-stu-id="ebd56-113">value</span></span>|<span data-ttu-id="ebd56-114">バイナリ</span><span class="sxs-lookup"><span data-stu-id="ebd56-114">Binary</span></span>|<span data-ttu-id="ebd56-115">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="ebd56-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd56-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebd56-116">Relationships</span></span>
<span data-ttu-id="ebd56-117">なし</span><span class="sxs-lookup"><span data-stu-id="ebd56-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebd56-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebd56-118">JSON Representation</span></span>
<span data-ttu-id="ebd56-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ebd56-119">Here is a JSON representation of the resource.</span></span>
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



