---
title: " certificationControl リソースの種類"
description: このリソースには、コンプライアンスが含まれている証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380946"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="85c05-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85c05-103">certificationControl resource type</span></span>

<span data-ttu-id="85c05-104">コンプライアンスを含む証明書のデータに関連付けられているスコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="85c05-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="85c05-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85c05-105">Property</span></span> |<span data-ttu-id="85c05-106">型</span><span class="sxs-lookup"><span data-stu-id="85c05-106">Type</span></span> |<span data-ttu-id="85c05-107">説明</span><span class="sxs-lookup"><span data-stu-id="85c05-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="85c05-108">name</span><span class="sxs-lookup"><span data-stu-id="85c05-108">name</span></span> | <span data-ttu-id="85c05-109">文字列</span><span class="sxs-lookup"><span data-stu-id="85c05-109">string</span></span> | <span data-ttu-id="85c05-110">コントロールの名前を証明</span><span class="sxs-lookup"><span data-stu-id="85c05-110">Certification control name</span></span> |
|<span data-ttu-id="85c05-111">url</span><span class="sxs-lookup"><span data-stu-id="85c05-111">url</span></span> | <span data-ttu-id="85c05-112">文字列</span><span class="sxs-lookup"><span data-stu-id="85c05-112">string</span></span> | <span data-ttu-id="85c05-113">Microsoft サービスの URL は、ポータルを信頼します。</span><span class="sxs-lookup"><span data-stu-id="85c05-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85c05-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85c05-114">JSON representation</span></span>

<span data-ttu-id="85c05-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85c05-115">The following is a JSON representation of the resource.</span></span>

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
