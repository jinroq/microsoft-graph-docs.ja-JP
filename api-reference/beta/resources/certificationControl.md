---
title: " certificationControl リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 22dc12070a801988d814ba73c6bffe1414bb5218
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012997"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="3971c-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3971c-103">certificationControl resource type</span></span>

<span data-ttu-id="3971c-104">セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。</span><span class="sxs-lookup"><span data-stu-id="3971c-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="3971c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3971c-105">Property</span></span> |<span data-ttu-id="3971c-106">型</span><span class="sxs-lookup"><span data-stu-id="3971c-106">Type</span></span> |<span data-ttu-id="3971c-107">説明</span><span class="sxs-lookup"><span data-stu-id="3971c-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3971c-108">name</span><span class="sxs-lookup"><span data-stu-id="3971c-108">name</span></span> | <span data-ttu-id="3971c-109">string</span><span class="sxs-lookup"><span data-stu-id="3971c-109">string</span></span> | <span data-ttu-id="3971c-110">証明書制御名</span><span class="sxs-lookup"><span data-stu-id="3971c-110">Certification control name</span></span> |
|<span data-ttu-id="3971c-111">url</span><span class="sxs-lookup"><span data-stu-id="3971c-111">url</span></span> | <span data-ttu-id="3971c-112">string</span><span class="sxs-lookup"><span data-stu-id="3971c-112">string</span></span> | <span data-ttu-id="3971c-113">Microsoft Service Trust Portal の URL</span><span class="sxs-lookup"><span data-stu-id="3971c-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3971c-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3971c-114">JSON representation</span></span>

<span data-ttu-id="3971c-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3971c-115">The following is a JSON representation of the resource.</span></span>

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
