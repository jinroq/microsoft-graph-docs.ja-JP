---
title: " certificationControl リソースの種類"
description: このリソースには、コンプライアンスが含まれている証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810389"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="bbe6c-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbe6c-103">certificationControl resource type</span></span>

<span data-ttu-id="bbe6c-104">コンプライアンスを含む証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="bbe6c-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="bbe6c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbe6c-105">Property</span></span> |<span data-ttu-id="bbe6c-106">種類</span><span class="sxs-lookup"><span data-stu-id="bbe6c-106">Type</span></span> |<span data-ttu-id="bbe6c-107">説明</span><span class="sxs-lookup"><span data-stu-id="bbe6c-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="bbe6c-108">name</span><span class="sxs-lookup"><span data-stu-id="bbe6c-108">name</span></span> | <span data-ttu-id="bbe6c-109">文字列</span><span class="sxs-lookup"><span data-stu-id="bbe6c-109">string</span></span> | <span data-ttu-id="bbe6c-110">コントロールの名前を証明</span><span class="sxs-lookup"><span data-stu-id="bbe6c-110">Certification control name</span></span> |
|<span data-ttu-id="bbe6c-111">url</span><span class="sxs-lookup"><span data-stu-id="bbe6c-111">url</span></span> | <span data-ttu-id="bbe6c-112">文字列</span><span class="sxs-lookup"><span data-stu-id="bbe6c-112">string</span></span> | <span data-ttu-id="bbe6c-113">Microsoft サービスの URL は、ポータルを信頼します。</span><span class="sxs-lookup"><span data-stu-id="bbe6c-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bbe6c-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbe6c-114">JSON representation</span></span>

<span data-ttu-id="bbe6c-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbe6c-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
