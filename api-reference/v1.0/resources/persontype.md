---
title: personType リソースの種類
description: 個人の種類を表します。
ms.openlocfilehash: 3938be8d1dd0bf4a4934de4bbcd7862185971128
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021000"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="64e3d-103">personType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64e3d-103">personType resource type</span></span>

<span data-ttu-id="64e3d-104">個人の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="64e3d-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="64e3d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64e3d-105">JSON representation</span></span>

<span data-ttu-id="64e3d-106">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64e3d-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="64e3d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64e3d-107">Properties</span></span>
| <span data-ttu-id="64e3d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64e3d-108">Property</span></span>     | <span data-ttu-id="64e3d-109">型</span><span class="sxs-lookup"><span data-stu-id="64e3d-109">Type</span></span>   |<span data-ttu-id="64e3d-110">説明</span><span class="sxs-lookup"><span data-stu-id="64e3d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64e3d-111">クラス</span><span class="sxs-lookup"><span data-stu-id="64e3d-111">class</span></span>|<span data-ttu-id="64e3d-112">String</span><span class="sxs-lookup"><span data-stu-id="64e3d-112">String</span></span>|<span data-ttu-id="64e3d-113">データ ソースの種類 (Person など)。</span><span class="sxs-lookup"><span data-stu-id="64e3d-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="64e3d-114">サブクラス</span><span class="sxs-lookup"><span data-stu-id="64e3d-114">subclass</span></span>|<span data-ttu-id="64e3d-115">String</span><span class="sxs-lookup"><span data-stu-id="64e3d-115">String</span></span>|<span data-ttu-id="64e3d-116">データ ソースの 2 番目の種類 (OrganizationUser など)。</span><span class="sxs-lookup"><span data-stu-id="64e3d-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
