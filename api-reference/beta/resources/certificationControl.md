---
title: " certificationControl リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535414"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="77170-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77170-103">certificationControl resource type</span></span>

<span data-ttu-id="77170-104">セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。</span><span class="sxs-lookup"><span data-stu-id="77170-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="77170-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77170-105">Property</span></span> |<span data-ttu-id="77170-106">型</span><span class="sxs-lookup"><span data-stu-id="77170-106">Type</span></span> |<span data-ttu-id="77170-107">説明</span><span class="sxs-lookup"><span data-stu-id="77170-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="77170-108">name</span><span class="sxs-lookup"><span data-stu-id="77170-108">name</span></span> | <span data-ttu-id="77170-109">string</span><span class="sxs-lookup"><span data-stu-id="77170-109">string</span></span> | <span data-ttu-id="77170-110">証明書制御名</span><span class="sxs-lookup"><span data-stu-id="77170-110">Certification control name</span></span> |
|<span data-ttu-id="77170-111">url</span><span class="sxs-lookup"><span data-stu-id="77170-111">url</span></span> | <span data-ttu-id="77170-112">string</span><span class="sxs-lookup"><span data-stu-id="77170-112">string</span></span> | <span data-ttu-id="77170-113">Microsoft Service Trust Portal の URL</span><span class="sxs-lookup"><span data-stu-id="77170-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77170-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77170-114">JSON representation</span></span>

<span data-ttu-id="77170-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77170-115">The following is a JSON representation of the resource.</span></span>

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
