---
title: certificationControl リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンス証明書データが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629314"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="fb358-103">certificationControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb358-103">certificationControl resource type</span></span>

<span data-ttu-id="fb358-104">セキュリティで保護されたスコアコントロールに関連付けられたコンプライアンス証明書データを格納します。</span><span class="sxs-lookup"><span data-stu-id="fb358-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="fb358-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb358-105">Properties</span></span>

|<span data-ttu-id="fb358-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb358-106">Property</span></span> |<span data-ttu-id="fb358-107">型</span><span class="sxs-lookup"><span data-stu-id="fb358-107">Type</span></span> |<span data-ttu-id="fb358-108">説明</span><span class="sxs-lookup"><span data-stu-id="fb358-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="fb358-109">name</span><span class="sxs-lookup"><span data-stu-id="fb358-109">name</span></span>|<span data-ttu-id="fb358-110">String</span><span class="sxs-lookup"><span data-stu-id="fb358-110">String</span></span>|<span data-ttu-id="fb358-111">証明書制御名</span><span class="sxs-lookup"><span data-stu-id="fb358-111">Certification control name</span></span> |
|<span data-ttu-id="fb358-112">url</span><span class="sxs-lookup"><span data-stu-id="fb358-112">url</span></span>|<span data-ttu-id="fb358-113">String</span><span class="sxs-lookup"><span data-stu-id="fb358-113">String</span></span>|<span data-ttu-id="fb358-114">Microsoft Service Trust Portal の URL</span><span class="sxs-lookup"><span data-stu-id="fb358-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb358-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb358-115">JSON representation</span></span>

<span data-ttu-id="fb358-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb358-116">The following is a JSON representation of the resource.</span></span>

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
