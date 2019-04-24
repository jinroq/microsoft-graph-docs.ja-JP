---
title: personType リソースの種類
description: 個人の種類を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462460"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="b00ad-103">personType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b00ad-103">personType resource type</span></span>

<span data-ttu-id="b00ad-104">個人の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b00ad-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b00ad-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b00ad-105">JSON representation</span></span>

<span data-ttu-id="b00ad-106">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b00ad-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b00ad-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b00ad-107">Properties</span></span>
| <span data-ttu-id="b00ad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b00ad-108">Property</span></span>     | <span data-ttu-id="b00ad-109">型</span><span class="sxs-lookup"><span data-stu-id="b00ad-109">Type</span></span>   |<span data-ttu-id="b00ad-110">説明</span><span class="sxs-lookup"><span data-stu-id="b00ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b00ad-111">クラス</span><span class="sxs-lookup"><span data-stu-id="b00ad-111">class</span></span>|<span data-ttu-id="b00ad-112">String</span><span class="sxs-lookup"><span data-stu-id="b00ad-112">String</span></span>|<span data-ttu-id="b00ad-113">データ ソースの種類 (Person など)。</span><span class="sxs-lookup"><span data-stu-id="b00ad-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="b00ad-114">サブクラス</span><span class="sxs-lookup"><span data-stu-id="b00ad-114">subclass</span></span>|<span data-ttu-id="b00ad-115">String</span><span class="sxs-lookup"><span data-stu-id="b00ad-115">String</span></span>|<span data-ttu-id="b00ad-116">データ ソースの 2 番目の種類 (OrganizationUser など)。</span><span class="sxs-lookup"><span data-stu-id="b00ad-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
