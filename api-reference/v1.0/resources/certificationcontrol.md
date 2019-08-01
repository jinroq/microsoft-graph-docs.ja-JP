---
title: certificationControl リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ad7c07d269f9dc627de41db621e4d73f0d2c10b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029905"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="34b62-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34b62-103">certificationControl resource type</span></span>

<span data-ttu-id="34b62-104">セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。</span><span class="sxs-lookup"><span data-stu-id="34b62-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="34b62-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34b62-105">Properties</span></span>

|<span data-ttu-id="34b62-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34b62-106">Property</span></span> |<span data-ttu-id="34b62-107">型</span><span class="sxs-lookup"><span data-stu-id="34b62-107">Type</span></span> |<span data-ttu-id="34b62-108">説明</span><span class="sxs-lookup"><span data-stu-id="34b62-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="34b62-109">name</span><span class="sxs-lookup"><span data-stu-id="34b62-109">name</span></span>|<span data-ttu-id="34b62-110">String</span><span class="sxs-lookup"><span data-stu-id="34b62-110">String</span></span>|<span data-ttu-id="34b62-111">証明書制御名</span><span class="sxs-lookup"><span data-stu-id="34b62-111">Certification control name</span></span> |
|<span data-ttu-id="34b62-112">url</span><span class="sxs-lookup"><span data-stu-id="34b62-112">url</span></span>|<span data-ttu-id="34b62-113">String</span><span class="sxs-lookup"><span data-stu-id="34b62-113">String</span></span>|<span data-ttu-id="34b62-114">Microsoft Service Trust Portal の URL</span><span class="sxs-lookup"><span data-stu-id="34b62-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="34b62-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34b62-115">JSON representation</span></span>

<span data-ttu-id="34b62-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34b62-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
